# TerraTact: Comparative Product Hypothesis Evaluation

**Document ID:** TT-STAGE2-002  
**Author:** Multidisciplinary Venture Strategy & Product Research Team  
**Date:** October 2026  
**Evaluation Framework:** Multi-Criteria Product Strategy Comparison  

---

## 1. Executive Summary: The Three Contending Directions

Following mentor feedback, TerraTact’s product roadmap is evaluated across three distinct strategic formulations:

- **Product A (Crop Suitability Intelligence):** A focused, pre-season decision-support engine matching soil (iSDAsoil 30m), climate, and farm constraints to biologically suitable crops.
- **Product B (Seasonal Farm Planning & Crop Portfolio Intelligence):** A multi-season, year-round planning platform that helps farmers sequence crops, select specific certified seed varieties based on rainfall onset, optimize legume-cereal rotations, and plan dry-season land use.
- **Product C (High-Value Specialty-Crop Intelligence):** A specialized advisory tool directing farmers into high-value niche crops, particularly cultivated edible mushrooms and specialty horticulture.

```text
               THE PRODUCT EVOLUTION SPECTRUM:
┌─────────────────────────┬─────────────────────────┬─────────────────────────┐
│       PRODUCT A         │       PRODUCT B         │       PRODUCT C         │
│   Crop Suitability      │  Seasonal Farm Planning │   Specialty Crops &     │
│     Intelligence        │   & Crop Portfolio      │       Mushrooms         │
├─────────────────────────┼─────────────────────────┼─────────────────────────┤
│ • Pre-season suitability│ • Dynamic multi-season  │ • Niche, high-value     │
│ • Single planting window│ • Seed varietal choice  │   specialty crops       │
│ • "What should I grow?" │ • Rotation & soil health│ • High capital & tech   │
│ • High seasonal churn   │ • Year-round engagement │ • Severe physical supply│
│   between seasons       │ • Co-op yield management│   chain bottlenecks     │
└─────────────────────────┴─────────────────────────┴─────────────────────────┘
```

---

## 2. Multi-Criteria Evaluation Matrix

Each product hypothesis is evaluated on a standardized 1–5 scale across nine core venture dimensions:

| Strategic Dimension | Weight | Product A: Suitability | Product B: Seasonal Planning | Product C: Specialty/Mushrooms |
|---|:---:|:---:|:---:|:---:|
| **1. User Pain Severity & Real-World Urgency** | 15% | 4 (Crop choice matters, but once a year) | **5 (Continuous soil exhaustion & climate shifts)** | 3 (Farmers want income, but lack basics) |
| **2. Demonstrated Demand & Willingness to Pay** | 15% | 3 (Low standalone B2C; moderate co-op value) | **4 (High co-op value for seasonal aggregation)** | 2 (Smallholders lack CapEx for spawn/rooms) |
| **3. Competitive Differentiation Potential** | 15% | 3 (Similar to static extension guides) | **5 (Unconflicted multi-season rotation engine)** | 3 (Specialty apps struggle with niche TAM) |
| **4. Data Feasibility & Technical Access** | 10% | 4 (iSDAsoil + CHIRPS readily available) | **4 (Requires variety calendars + local trial data)** | 1 (Mushroom micro-climate data is proprietary) |
| **5. Implementation Cost & Development Speed** | 10% | **5 (Lowest technical complexity; fast MVP)** | 4 (Requires multi-season state tracking engine) | 2 (Requires specialized physical agronomists) |
| **6. Potential Smallholder Income Impact** | 10% | 4 (Doubles legume margin vs maize) | **5 (Compounds soil fertility + multi-season yields)**| 3 (High unit price, but high failure rate) |
| **7. Adoption & Behavioral Friction** | 10% | 4 (Moderate friction if intermediated) | 3 (Requires seasonal interaction with co-op) | **1 (Severe behavioral shift; sterile handling)** |
| **8. Institutional Distribution Feasibility** | 10% | 4 (Fits AMCOS pre-season planning) | **5 (Directly matches AMCOS seasonal business)** | 2 (AMCOS co-ops do not aggregate mushrooms) |
| **9. Commercial Sustainability & Retention** | 5% | 2 (Severe 9-month churn between seasons) | **5 (Year-round active utility for co-op & farmer)**| 2 (High farmer drop-off post-contamination) |
| **TOTAL WEIGHTED SCORE** | **100%** | **3.60** | **4.50** | **2.05** |

---

## 3. Detailed Hypothesis Breakdown & Analysis

### 3.1 Product A: Crop Suitability Intelligence (Score: 3.60)
- **The Case For:** Focused, technically clean, and relatively quick to build. Ingesting 30m iSDAsoil and CHIRPS rainfall produces an immediate baseline recommendation.
- **The Fatal Flaw:** **Extreme Seasonal Churn.** A farmer only chooses what to plant once (or twice in bimodal areas) per year. Once seeds are in the ground in December, the farmer and cooperative have zero reason to interact with the software until the following November. B2B enterprise software cannot sustain enterprise subscription value with a product used one week a year.

### 3.2 Product B: Seasonal Farm Planning & Crop Portfolio Intelligence (Score: 4.50 — WINNER)
- **The Case For:** Evolves TerraTact from a disposable "crop selector" into an indispensable **multi-season farm intelligence platform**. It answers the real operational questions smallholders face throughout the year:
  1. *Pre-Season (October–November):* "Given delayed rainfall onset, which specific certified seed variety (e.g., short-duration Uyole 03 bean vs. medium-duration SC627 maize) should I plant to avoid terminal drought?"
  2. *Mid-Season (January–February):* "How should I sequence my weeding, top-dressing, and intercropped legume management to maximize soil nitrogen fixation?"
  3. *Post-Harvest (May–June):* "How should I rotate my fields for the upcoming season to break maize stalk borer cycles and rebuild soil organic matter?"
  4. *Dry-Season (July–September):* "Can I utilize residual valley-bottom moisture (*vinyungu*) for a fast 60-day vegetable or cover crop?"
- **Institutional Alignment:** AMCOS cooperatives operate on continuous seasonal cycles (input ordering $\rightarrow$ loan disbursement $\rightarrow$ agronomic monitoring $\rightarrow$ harvest aggregation $\rightarrow$ warehouse receipt settlement). Product B aligns perfectly with the cooperative’s year-round financial workflow.

### 3.3 Product C: High-Value Specialty-Crop & Mushroom Intelligence (Score: 2.05 — REJECTED AS CORE)
- **The Fallacy of High Unit Value:** While gourmet mushrooms (e.g., fresh oyster mushrooms at \$3–\$5/kg, or theoretical dried morels at \$100+/kg) look spectacular in financial spreadsheets, **they fail the physical reality test in African smallholder systems**.
- **The Physical Bottlenecks Software Cannot Solve:**
  1. *Clean Spawn Scarcity:* Mushroom farming requires a sterile laboratory infrastructure to produce contamination-free spawn (*mycelium*). In Tanzania and Kenya, reliable spawn is restricted to university labs (SUA in Morogoro, JKUAT in Juja) with long lead times.
  2. *Sterilization & Contamination:* Substrates (sawdust, maize stover) must be pasteurized or autoclaved using firewood/steam. Contamination by green mold (*Trichoderma*) routinely wipes out 50%–80% of smallholder crops.
  3. *Perishability & Missing Cold Chain:* Fresh oyster mushrooms deteriorate within 48 to 72 hours without refrigeration. Smallholder villages in Mbeya or Songwe have zero cold storage.
  4. *Domestic Market Absence:* Rural and peri-urban Tanzanians do not consume significant volumes of commercial cultivated mushrooms. The only buyers are luxury safari lodges, high-end expatriate restaurants, and Chinese supermarket channels in Dar es Salaam and Nairobi.
- **Venture Verdict:** Smallholders do not fail at mushroom farming because they lack an AI recommendation app; **they fail because they lack sterile labs, subsidized steam pasteurizers, and refrigerated transport**. TerraTact is a software company, not a cold-chain logistics operator. Pushing resource-poor farmers into fragile specialty crops creates catastrophic downside risk.

---

## 4. Strategic Direction & Product Thesis

```text
===============================================================================
                       STRATEGIC PRODUCT DECISION:
            ADOPT PRODUCT B: SEASONAL FARM PLANNING & PORTFOLIO INTELLIGENCE
===============================================================================
TerraTact will NOT launch as a static one-off crop selector (Product A).
TerraTact will NOT pivot into high-risk specialty mushrooms (Product C).

TerraTact will build PRODUCT B: A multi-season farm planning engine that 
empowers cooperatives to optimize:
1. Dynamic Seed & Varietal Selection (matching maturity days to seasonal onset).
2. Sustainable Cereal-Legume Rotation Cycles (restoring soil nitrogen).
3. Household Acreage Optimization (food security reserves + commercial cash crops).
===============================================================================
```
