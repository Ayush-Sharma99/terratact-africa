# TerraTact Africa (formerly Krishi Sathi)
## Agricultural Decision Support, Smallholder Venture Strategy & Market Due Diligence

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Research: Sub-Saharan Africa](https://img.shields.io/badge/Focus-East%20Africa%20%7C%20Tanzania-emerald.svg)](krishi-sathi-africa/research/country_screening.md)
[![Status: Second-Stage Due Diligence](https://img.shields.io/badge/Stage-Pre--Pilot%20Validation-blue.svg)](krishi-sathi-africa/second_stage_research/updated_venture_recommendation.md)

---

## 1. Executive Overview

**TerraTact Africa** is an agricultural venture initiative designed to provide climate-adaptive, season-by-season farm planning and varietal decision support to smallholder farmers in Sub-Saharan Africa.

Originally conceived as an Indian soil-chemistry crop recommendation tool (*Krishi Sathi*), the project has undergone comprehensive, multi-phase venture due diligence, market discovery, competitive intelligence, and economic viability analysis to adapt to the realities of African smallholder agriculture.

This repository houses the complete due diligence, research literature, macroeconomic models, empirical datasets, and mentor briefing deliverables compiled by a multidisciplinary research team operating under institutional investment committee rigor.

---

## 2. Key Due Diligence Findings

| Focus Area | Hypothesis Evaluated | Empirical Finding & Venture Decision |
| :--- | :--- | :--- |
| **Product Core** | Static single-crop recommendation (Product A) | **Pivoted to Dynamic Seasonal Farm Intelligence (Product B).**<br>Static single-crop classification causes severe 9-month annual software churn. Product B solves dynamic varietal matching based on rainfall onset and manages multi-season cereal-legume biological nitrogen fixation ($35\text{--}80\text{ kg N/ha}$). |
| **Target Geography** | Broad African rollout vs. weak-currency markets | **Tanzania Southern Highlands selected as beachhead (Score: 4.38/5.00).**<br>Disproved the "weak currency fallacy": currency collapse in Nigeria ($>70\%$ drop, inflation $>30\%$) and Ethiopia ($\sim 100\%$ devaluation) spiked operational costs and destroyed farmer disposable cash. Tanzania provides macroeconomic stability ($\sim 2,600\text{ TZS/\$}$, $3\%\text{--}5\%$ inflation) and 450+ registered AMCOS cooperatives in Mbeya, Songwe, and Iringa. |
| **Specialty Crops** | Premium "Gucci" / Morel mushrooms (*Morchella*) | **Formally Excluded (Score: 2.05/5.00).**<br>Morels require temperate montane cold dormancy ($<5^\circ\text{C}$ to $8^\circ\text{C}$) and damp spring thaw triggers absent in Sub-Saharan Africa ($100\%$ biological failure). Cultivated oyster mushrooms suffer severe physical bottlenecks (lack of sterile spawn, $>50\%$ green mold contamination, 48-hour shelf life, zero cold chain). Software cannot pasteurize straw or run refrigerated trucks. |
| **Commercial Model** | Direct B2C farmer subscriptions | **B2B2C Institutional Licensing via AMCOS & Off-takers.**<br>Smallholder ability to pay cash for pure software is near zero ($<2\%$ credit card / digital subscription adoption). Monitored licensing at \$1.50–\$2.00 per farmer per season funded through cooperative operational budgets or buyer yield-enhancement premiums. |
| **Rotational Economics** | Continuous maize cultivation | **Legume Diversification Doubles Farm Gross Margins.**<br>Rotating continuous maize into certified Common Beans (Uyole 03) or Inoculated Soybeans doubles gross margins per acre (**TZS 670,347 / \$258 vs. TZS 320,000 / \$123 for maize**) while preserving an inviolable 1.0+ acre maize food security reserve. |

---

## 3. Repository Architecture

```text
Farm/
├── README.md                                 <- Root repository overview and collaborator guide
├── .gitignore                                <- Standard development & credential safeguards
├── skills-lock.json                          <- Skills lockfile
├── .agents/                                  <- Specialized research runtime skills (Gravitas, Deep Research)
└── krishi-sathi-africa/
    ├── README.md                             <- Detailed project index and 10-role framework
    │
    ├── deliverables/                         <- Mentor & Executive Presentation Package
    │   ├── mentor_briefing_report.md         <- Comprehensive venture briefing (~2,500 words)
    │   ├── mentor_presentation_content.md    <- 12-slide presentation deck with speaker notes & visuals
    │   └── verification_and_open_questions.md<- 19-point claim audit and open strategic questions
    │
    ├── second_stage_research/                <- Stage 2 Deep Research: Seasonality, Specialty Crops & Currency
    │   ├── mentor_context_interpretation.md  <- Disambiguation of mentor guidance into falsifiable hypotheses
    │   ├── product_hypothesis_comparison.md  <- Comparative scoring: Product A vs Product B vs Product C
    │   ├── seasonal_farm_planning_research.md<- Dynamic varietal selection & cereal-legume rotation models
    │   ├── mushroom_opportunity_assessment.md<- Agronomic & supply chain audit of mushrooms
    │   ├── country_comparison_updated.md     <- 20-criteria updated national decision model
    │   ├── currency_and_operating_cost_analysis.md <- Devaluation, inflation & the "weak currency fallacy"
    │   ├── updated_venture_recommendation.md <- Formal second-stage venture memorandum
    │   ├── next_validation_plan.md           <- 90-day lean pre-pilot validation plan ($28,500 USD)
    │   ├── seasonal_competitor_matrix.csv    <- 12 direct/adjacent competitors audited for seasonal features
    │   └── crop_and_specialty_opportunity_matrix.csv <- 11 candidate crops/specialties evaluated
    │
    ├── research/                             <- Stage 1 Foundation Due Diligence Reports
    │   ├── methodology.md                    <- Due diligence methodology, source ladder & baseline audit
    │   ├── africa_market_landscape.md        <- 10-country comparative agricultural landscape
    │   ├── country_screening.md              <- 10-criteria weighted decision model & sensitivity analysis
    │   ├── competitor_analysis.md            <- Competitor, substitute & incumbent audit (20+ platforms)
    │   ├── crop_selection.md                 <- Southern Highlands crop economics & maize monoculture trap
    │   ├── data_feasibility.md               <- Spatial, soil (iSDAsoil 30m), weather & satellite data
    │   ├── business_model.md                 <- Commercial models, unit economics & monetization
    │   ├── regulatory_review.md              <- Compliance (TOSCI, TFRA, PDPA 2022)
    │   ├── red_team_review.md                <- Pre-mortem analysis & 3 fatal failure scenarios
    │   └── investment_memo.md                <- Master investment memorandum answering 18 key questions
    │
    ├── data/                                 <- Master Empirical Datasets & Registries
    │   ├── assumption_register.csv           <- 13 logged hypotheses with falsification criteria
    │   ├── source_register.csv               <- 16 peer-reviewed / institutional sources with exact URLs
    │   ├── country_evidence.csv              <- Normalized multi-country agricultural & macroeconomic data
    │   ├── competitor_database.csv           <- Structured audit of African agritech platforms
    │   ├── dataset_inventory.csv             <- Spatial, soil, weather & crop dataset evaluation
    │   └── crop_economics.csv                <- Illustrative crop margins, input costs & farm economics
    │
    ├── strategy/                             <- Go-To-Market & Operational Blueprints
    │   ├── product_positioning.md            <- Strategic whitespace, differentiation & value proposition
    │   ├── technical_architecture.md         <- 4-stage hybrid agronomic/spatial decision engine
    │   ├── go_to_market.md                   <- B2B2C distribution, institutional partnerships & channels
    │   ├── pilot_plan.md                     <- Phased pilot protocol & experimental design
    │   └── execution_roadmap.md              <- 30/60/90-day actionable milestones
    │
    └── validation/                           <- Field Instruments & Governance
        ├── farmer_interview_guide.md         <- Non-leading qualitative discovery questionnaire
        ├── partner_interview_guide.md        <- Institutional (co-op, off-taker, input dealer) discovery
        ├── pilot_metrics.md                  <- Leading/lagging KPI scorecard & go/no-go thresholds
        └── decision_log.md                   <- Immutable audit trail of strategic choices & pivots
```

---

## 4. How to Navigate This Workspace

* **For Mentors & Investors:**  
  Start with the [Mentor Briefing Report](krishi-sathi-africa/deliverables/mentor_briefing_report.md) and the [12-Slide Presentation Content](krishi-sathi-africa/deliverables/mentor_presentation_content.md).
* **For Agricultural & Agronomic Due Diligence:**  
  Review [Seasonal Farm Planning Research](krishi-sathi-africa/second_stage_research/seasonal_farm_planning_research.md), [Crop Selection](krishi-sathi-africa/research/crop_selection.md), and [Mushroom Feasibility Assessment](krishi-sathi-africa/second_stage_research/mushroom_opportunity_assessment.md).
* **For Technical & Data Architecture:**  
  Inspect the [Data Feasibility Analysis](krishi-sathi-africa/research/data_feasibility.md) and [Technical Architecture Blueprint](krishi-sathi-africa/strategy/technical_architecture.md).
* **For Macroeconomic & Market Selection Context:**  
  Consult [Country Comparison Updated](krishi-sathi-africa/second_stage_research/country_comparison_updated.md) and [Currency & Operating Cost Analysis](krishi-sathi-africa/second_stage_research/currency_and_operating_cost_analysis.md).
* **For Field Validation Protocols:**  
  Refer to the [Farmer Interview Guide](krishi-sathi-africa/validation/farmer_interview_guide.md), [Partner Interview Guide](krishi-sathi-africa/validation/partner_interview_guide.md), and the [Next Validation Plan](krishi-sathi-africa/second_stage_research/next_validation_plan.md).

---

## 5. Next Steps: Sprint 1 (Days 1–30)

1. **Academic & Research Institutional Alignment:** Formal outreach to the Tanzania Agricultural Research Institute (**TARI Uyole**, Mbeya) for local varietal trial datasets and agro-ecological zone validation.
2. **Cooperative Field Reconnaissance:** Conducting structured qualitative interviews with AMCOS cooperative leaders across Mbeya and Songwe.
3. **Regulatory Clearance:** Data controller registration filings under the Tanzanian Personal Data Protection Act (PDPA 2022) with the PDPC and BRELA entity incorporation.
