# Due Diligence Decision Log & Audit Trail

**Project:** Krishi Sathi Africa Venture Validation  
**Custodian:** Senior Multidisciplinary Due Diligence Team  
**Policy:** Immutable record of strategic decisions, pivots, and falsifications.

---

## Decision Entries

### [DEC-001] Falsification of Standalone B2C Mobile App Model
- **Date:** October 2026
- **Context:** Initial concept proposed a direct farmer-facing mobile app recommending crops based on user-entered soil and climate parameters.
- **Decision:** **REJECT** direct-to-consumer (B2C) paid mobile app model for smallholders.
- **Evidence Base:** 
  1. Primary surveys (AfSIS, iSDA) confirm <2% of smallholders possess lab soil test metrics ($N, P, K, pH$).
  2. Evaluations from J-PAL / PxD (Kremer et al.) and GSMA AgriTech confirm that farmer willingness-to-pay for standalone digital advice approaches zero.
  3. Rural smartphone penetration in Sub-Saharan Africa remains low (25%–40%), with prohibitive data costs.
- **Adopted Pivot:** Transition to a **B2B2C / Phygital decision-support engine** that ingests spatial open data (iSDAsoil 30m, CHIRPS) via GPS, delivering insights through institutional intermediaries (cooperatives, input distributors, off-takers, NGOs) or lightweight channels (USSD, WhatsApp, extension agents).
- **Condition for Reversal:** Verified empirical field proof that smallholders in a target market willingly pay monthly SaaS fees for standalone digital advice and possess smartphone-based lab testing tools.

### [DEC-002] Rejection of the Kaggle 22-Crop Demonstration Dataset
- **Date:** October 2026
- **Context:** Kaggle's standard Crop Recommendation Dataset (Atharva Ingle) is widely cited in academic prototypes achieving >99% accuracy.
- **Decision:** **PROHIBIT** the use of the Kaggle 22-crop synthetic dataset as the basis for African agronomic recommendations.
- **Evidence Base:**
  1. The dataset contains synthetic Gaussian distributions tailored to Indian agricultural handbook ranges.
  2. It omits core African food-security and commercial smallholder staples (Cassava, Yam, Sorghum, Cowpea, Teff, Plantain).
  3. It predicts ecologically incompatible crops (e.g., jute, apples) in tropical smallholder environments.
- **Adopted Pivot:** Restructure the agronomic knowledge base around regional agroecological zones (AEZs) and national priority value chains using FAO GAEZ v4, national agricultural research datasets, and validated crop calendars.
- **Condition for Reversal:** None. Synthetic Indian data cannot govern African smallholder agricultural decisions.

### [DEC-003] Multi-Market Screening Shortlist Formulation
- **Date:** October 2026
- **Context:** Initial exploratory prompt suggested testing 14+ countries across East, West, North, and Southern Africa.
- **Decision:** Conduct systematic screening across 10 focal countries: **Kenya, Tanzania, Uganda, Ethiopia, Rwanda, Nigeria, Ghana, Côte d'Ivoire, Senegal, Egypt**, and identify the top candidate market using a transparent, multi-criteria weighted scoring model.
- **Evidence Base:** Focus countries represent distinct regional archetypes: East African digital hub (Kenya), East African smallholder diversification (Tanzania), West African mega-market (Nigeria), West African cash crop/co-op hub (Ghana, Côte d'Ivoire), and North African irrigated agribusiness (Egypt).


### [DEC-004] Rejection of Specialty Morel and Cultivated Mushroom Opportunities
- **Date:** October 2026
- **Context:** Mentor proposed investigating high-value specialty crops, specifically mentioning mushrooms and "Gucci" (morel) mushrooms.
- **Decision:** **REJECT** morel (*Morchella*) and cultivated oyster (*Pleurotus*) mushrooms from TerraTact's core product strategy.
- **Evidence Base:**
  1. *Morchella* biology requires temperate cold winter dormancy (<5°C–8°C) and spring thaw triggers that do not exist in tropical or equatorial Sub-Saharan Africa. Open-field morel farming has a 100% biological failure rate.
  2. Cultivated oyster mushrooms fail in smallholder systems due to physical bottlenecks (spawn supply scarcity from distant university labs, 50%+ green mold contamination, 48-hour fresh spoilage, zero cold chain, and absent rural demand).
  3. Software cannot pasteurize straw, eliminate mold, or supply refrigerated trucks. Pushing smallholders into hyper-perishable specialty crops creates catastrophic downside risk.
- **Adopted Pivot:** Maintain core focus on field cereal-legume rotations (Maize, Common Bean, Soybean, Sunflower), where software directly solves information, varietal maturity, and acreage allocation constraints.
- **Condition for Reversal:** Verified demonstration of open-field morel cultivation in tropical lowlands, or third-party cold-chain infrastructure that eliminates perishability risks.

### [DEC-005] Strategic Adoption of Product B: Seasonal Farm Planning
- **Date:** October 2026
- **Context:** Evaluating whether TerraTact should remain a static one-off crop suitability classifier (Product A) or evolve into multi-season farm planning (Product B).
- **Decision:** **ADOPT PRODUCT B** (Seasonal Farm Planning & Crop Portfolio Intelligence).
- **Evidence Base:**
  1. Product A suffers from severe 9-month annual churn between planting dates.
  2. Smallholders face dynamic, multi-season challenges: selecting seed varieties matched to delayed rainfall onset, managing legume nitrogen fixation, and planning dry-season land use.
  3. Cooperatives operate on year-round seasonal workflows (input ordering $\rightarrow$ loan disbursement $\rightarrow$ yield monitoring $\rightarrow$ harvest aggregation $\rightarrow$ warehouse settlement). Product B aligns directly with cooperative operations.
- **Adopted Pivot:** Transition engine architecture to dynamic varietal matching (linking CHIRPS onset tracking to TOSCI maturity days) and multi-season rotation planning.
- **Condition for Reversal:** If cooperative discovery proves that AMCOS managers only want a single pre-season suitability score and reject multi-season features.

### [DEC-006] Re-Affirmation of Tanzania over Kenya, Nigeria, and Ethiopia
- **Date:** October 2026
- **Context:** Re-evaluating country selection from a lower-cost, currency devaluation, and operational perspective.
- **Decision:** **RE-AFFIRM TANZANIA AS RANK 1 ENTRY MARKET** (Score: 4.38/5.00).
- **Evidence Base:**
  1. *Nigeria (Score: 2.88):* Severe currency collapse (>70% drop), 30%+ inflation, fuel subsidy removal tripling transit costs, smallholder purchasing power crushed, and foreign exchange trapped by banking illiquidity.
  2. *Ethiopia (Score: 2.73):* Birr floated in July 2024 (~100% drop), high inflation, state extension monopoly (ATI 8028 hotline), and regional armed conflict.
  3. *Kenya (Score: 3.70):* High tech living costs/salaries in Nairobi, and fatal competitive saturation (DigiFarm, Apollo, PxD, One Acre Fund) locking up cooperative channels.
  4. *Tanzania (Score: 4.38):* Stable 3%–5% inflation, disciplined gradual currency depreciation (~2,600 TZS/\$), Swahili linguistic unity, dense AMCOS cooperative networks, and absence of an entrenched venture-backed digital advisory monopoly.
- **Adopted Pivot:** Retain Southern Highlands of Tanzania as primary pilot beachhead; structure enterprise contracts with food-indexed cess terms to hedge inflation.
- **Condition for Reversal:** Unanimous rejection of B2B2C software licensing by 10 surveyed AMCOS cooperative boards.
