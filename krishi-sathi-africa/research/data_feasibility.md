# Stage 6: Technical Data Feasibility & Staged Architecture

**Author:** Multidisciplinary Investment Committee & Agritech Due Diligence Team  
**Date of Assessment:** October 2026  
**Document ID:** KS-DATA-006  

---

## 1. The Core Data Feasibility Breakthrough: Eliminating Farmer NPK Entry

The baseline audit established that requiring smallholders to manually input laboratory soil metrics ($N, P, K, pH$) creates a **100% barrier to adoption**. 

The technical breakthrough for Krishi Sathi lies in **decoupling recommendation generation from farmer self-reporting** through open-access, continental-scale geospatial APIs:

```text
┌─────────────────────────────────────────────────────────────────────────────┐
│                      THE SPATIAL INFERENCE PIPELINE                         │
│                                                                             │
│  [Farmer Plot Location (GPS coordinate captured via Agent phone or USSD)]    │
│                                   │                                         │
│                                   ▼                                         │
│  [Automated Cloud Query via AWS / STAC API]                                 │
│  ├── iSDAsoil (30m): Extract pH, Total N, Ext. P, Ext. K, Sand/Clay, SOC    │
│  ├── CHIRPS (0.05°): Historical 30-year dekadal rainfall & onset patterns   │
│  ├── NASA POWER (0.5°): Temperature, relative humidity & evapotranspiration │
│  └── SRTM DEM (30m): Elevation, slope gradient & drainage classification    │
│                                   │                                         │
│                                   ▼                                         │
│  [Fused Environmental Feature Vector (Zero farmer data-entry friction)]     │
└─────────────────────────────────────────────────────────────────────────────┘
```

### 1.1 Technical Validation of Key Datasets
1. **iSDAsoil (30m African Soil Map):** Developed by iSDA and World Agroforestry (Hengl et al., *Scientific Reports* 2021) [^1]. Trained on ~150,000 African soil samples using 3D ensemble machine learning. Validated cross-validation $R^2$ exceeds 0.70 for pH and soil texture, providing a highly reliable proxy for field-level chemical constraints without lab testing [^1].
2. **CHIRPS Precipitation:** Blends 0.05° infrared satellite precipitation with ground station networks [^2]. Universally utilized across East Africa for seasonal drought monitoring and onset detection.
3. **Open Access & Commercial Licensing:** Both iSDAsoil (CC BY 4.0) and CHIRPS (Public Domain) permit unrestricted commercial utilization with attribution, eliminating upstream intellectual property risks [^1][^2].

---

## 2. Decision Engine Architecture: Why Pure ML is Unviable

In agricultural advisory, deploying a **black-box supervised ML classifier** (such as standard Random Forest or XGBoost trained purely on synthetic data) is dangerous. Machine learning models:
- Extrapolate poorly outside training distributions.
- Lack deterministic agronomic guardrails (e.g., recommending a crop where soil $pH < 4.5$ guarantees aluminium toxicity).
- Cannot incorporate farm-level economic constraints or food security priorities.

### The Recommended Hybrid System Architecture

Krishi Sathi must be engineered as a **Four-Stage Hybrid Constraint-Optimization Engine**:

```text
┌─────────────────────────────────────────────────────────────────────────────┐
│ STAGE 1: Deterministic Agronomic Exclusion Filter (Hard Rules)              │
│ Checks physiological survival thresholds (FAO GAEZ / TARI Uyole manuals):   │
│ • If Soil pH < 5.0 -> Flag aluminium toxicity; exclude common beans/maize   │
│   unless agricultural lime is applied; suggest acid-tolerant alternatives.  │
│ • If Elevation > 2,000m -> Exclude lowland maize; flag frost hazard.       │
│ • If Slope > 15% -> Require soil conservation terraces before tilling.      │
└─────────────────────────────────────────────────────────────────────────────┘
                                      │
                                      ▼
┌─────────────────────────────────────────────────────────────────────────────┐
│ STAGE 2: Geospatial Suitability Scoring (ML Layer)                          │
│ Evaluates candidate crops surviving Stage 1 against local climatic features:│
│ • Features: Dekadal rainfall distribution, soil water capacity, thermal unit│
│ • Model: Calibrated Gradient Boosting Trees (LightGBM) trained on regional  │
│   TARI trial yield responses -> Outputs Suitability Index $S_i \in [0, 1]$. │
└─────────────────────────────────────────────────────────────────────────────┘
                                      │
                                      ▼
┌─────────────────────────────────────────────────────────────────────────────┐
│ STAGE 3: Household Economic & Risk Optimization (Linear Programming)        │
│ Optimizes acreage allocation vector $\vec{x}$ across crops to maximize      │
│ Expected Net Profit subject to smallholder survival constraints:            │
│   $\max \sum x_i \cdot \text{Margin}_i \cdot S_i$                           │
│   Subject to:                                                               │
│   1. $x_{\text{maize}} \ge \text{Min\_Food\_Security\_Acreage}$ (e.g. 1.0ac)│
│   2. $\sum x_i \cdot \text{Variable\_Cost}_i \le \text{Farmer\_Cash\_Budget}$│
│   3. $\sum x_i = \text{Total\_Farm\_Size}$                                  │
└─────────────────────────────────────────────────────────────────────────────┘
                                      │
                                      ▼
┌─────────────────────────────────────────────────────────────────────────────┐
│ STAGE 4: Swahili Natural-Language Explanation & Safety Protocol             │
│ Translates mathematical output into plain Swahili actionable advice:        │
│ "Kwa shamba lako la ekari 2.5 Mbalizi: Tenga ekari 1.2 kwa Mahindi ya chakula│
│ cha familia, na ekari 1.3 kwa Maharage (Uyole 03). Udongo wako una asidi    │
│ (pH 5.4), hivyo weka mifuko miwili ya chokaa (lime) kabla ya kupanda..."     │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## 3. Evaluation & Validation Protocol

To avoid the data leakage and artificial benchmark traps common in academic papers, the model evaluation must enforce:

1. **Spatial & Temporal Blocked Cross-Validation:** Train on historical seasons (e.g., 2015–2022) across 4 districts, evaluate strictly on out-of-sample holdout districts (spatial cross-validation) and future seasons (temporal holdout). Random $k$-fold cross-validation is strictly prohibited due to spatial autocorrelation.
2. **Abstention Protocol:** If the nearest ground-truth soil or rainfall reference exceeds uncertainty bounds (e.g., cloud cover obscuring optical NDVI, or anomalous rainfall divergence > 2 standard deviations), the system must explicitly **abstain from providing a recommendation** and trigger a notification for manual agronomic review by a local TARI officer.
3. **Safety & Toxicity Guardrails:** Never recommend chemical inputs (herbicides, pesticides) without automated verification of regional regulatory registration (TPRI - Tropical Pesticides Research Institute of Tanzania).

---

## 4. References & Sources for Stage 6

[^1]: Hengl, T., Miller, M.A.E., Križan, J., et al. (2021). "African soil properties and nutrients mapped at 30 m spatial resolution using two-scale ensemble machine learning." *Scientific Reports*, 11, 6130. https://doi.org/10.1038/s41598-021-85601-3.
[^2]: Funk, C., et al. (2015). "The climate hazards infrared precipitation with stations—a new environmental record for monitoring extremes." *Scientific Data*, 2, 150066. https://doi.org/10.1038/sdata.2015.66.
