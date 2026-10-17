# Technical Architecture & System Specification

**Engine Name:** Krishi Sathi Decision Core (v1.0 Africa)  
**Deployment Infrastructure:** Serverless AWS / Containerized FastAPI Python  
**Primary Integration:** STAC / GeoTIFF / AWS S3 Open Data Registry  

---

## 1. System Architecture Overview

```text
┌─────────────────────────────────────────────────────────────────────────────┐
│                            DATA INGESTION LAYER                             │
│  [iSDAsoil STAC API]      [CHIRPS Dekadal Rainfall]   [NASA POWER Climate]  │
│  30m chemical/physical     0.05° precipitation         0.5° temperature &   │
│  properties (pH, N, P, K)  historical & onset tracking solar radiation      │
└──────────────────────────────────────┬──────────────────────────────────────┘
                                       │
                                       ▼
┌─────────────────────────────────────────────────────────────────────────────┐
│                       CORE HYBRID DECISION ENGINE                           │
│                                                                             │
│   STAGE 1: AGRONOMIC EXCLUSION FILTER (Deterministic Python Rules)          │
│   ├── Enforces physiological thresholds (TARI/FAO crop rules)               │
│   └── Rejects lethal soil pH (<5.0 without lime) or extreme elevations      │
│                                                                             │
│   STAGE 2: SPATIAL SUITABILITY SCORING (LightGBM ML Classifier)             │
│   ├── Ingests: Topography, dekadal rainfall variance, soil water capacity   │
│   └── Outputs: Multi-crop suitability probability vector $S \in [0, 1]^K$   │
│                                                                             │
│   STAGE 3: ECONOMIC & RISK OPTIMIZATION (SciPy Linear Programming)          │
│   ├── Objective: $\max \sum x_i \cdot \text{NetMargin}_i \cdot S_i$         │
│   ├── Constraints: Food Security (Maize >= 1.0ac), Cash budget, Land size   │
│   └── Outputs: Recommended acreage allocation vector $\vec{x}$              │
│                                                                             │
│   STAGE 4: NATURAL LANGUAGE SWAHILI TRANSLATOR & SAFETY GATE                │
│   ├── Generates Swahili actionable narrative for extension agents/farmers   │
│   └── Enforces Abstention Protocol during extreme weather anomalies         │
└──────────────────────────────────────┬──────────────────────────────────────┘
                                       │
                                       ▼
┌─────────────────────────────────────────────────────────────────────────────┐
│                          DELIVERY & CLIENT CHANNELS                         │
│  [Field Agent Android App]     [USSD / SMS Gateway]   [AMCOS Web Dashboard] │
│  Offline-first SQLite sync      Feature phone access   Cooperative management│
│  used by Co-op Agronomists     via Africa's Talking   member yield monitoring│
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## 2. Model Pipeline & Algorithmic Formulations

### 2.1 Stage 1: Deterministic Exclusion Pseudocode
```python
def check_agronomic_feasibility(soil_data, elevation, slope):
    """
    Enforces non-negotiable physiological limits before ML evaluation.
    """
    excluded_crops = []
    required_amendments = []
    
    # Soil Acidity Threshold
    if soil_data["ph"] < 5.0:
        required_amendments.append({
            "amendment": "Agricultural Lime",
            "rate_kg_acre": 150,
            "rationale": "High acidity / Aluminium toxicity risk"
        })
        excluded_crops.extend(["Common Bean", "Soybean"])
        
    # Elevation Constraints
    if elevation > 2000:
        excluded_crops.append("Lowland Maize")
    if elevation < 1200:
        excluded_crops.append("Irish Potato")
        
    return excluded_crops, required_amendments
```

### 2.2 Stage 3: Constrained Acreage Optimization
Let $K$ be the set of feasible crops. The optimization solves:
$$\max_{\vec{x}} \sum_{i \in K} x_i \cdot \left( \hat{Y}_i \cdot P_i - C_i \right) \cdot S_i$$
Subject to:
1. $\sum_{i \in K} x_i = A_{\text{total}}$ (Total land constraint)
2. $x_{\text{maize}} \ge A_{\text{food\_security}} = \max\left(1.0, 0.25 \times N_{\text{household}}\right)$ (Family subsistence reserve)
3. $\sum_{i \in K} x_i \cdot C_i \le B_{\text{cash}}$ (Farmer working capital budget)
4. $x_i \ge 0 \quad \forall i \in K$
