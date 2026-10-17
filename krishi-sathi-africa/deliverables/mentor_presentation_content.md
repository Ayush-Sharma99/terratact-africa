# Mentor Presentation Content: Krishi Sathi Africa Due Diligence & Strategy

**Document Type:** Authoritative Presentation Markdown (Slide-by-Slide Deck Source)  
**File Name:** `mentor_presentation_content.md`  
**Target Duration:** 10–12 Minutes Presentation + Discussion  
**Audience:** Mentor / Strategic Venture Advisor  
**Visual Style:** Restrained, editorial, research-driven agritech aesthetic (warm earth tones, forest green, slate gray, clean typography)  
**Date:** October 2026  

---

# Slide 1 — Krishi Sathi Africa

**Purpose:**  
Introduce Krishi Sathi as a research-backed agricultural decision-support initiative exploring a strategic entry into Sub-Saharan Africa.

**Key message:**  
We are investigating whether and how an early-stage crop recommendation concept can evolve into a commercially viable, high-impact decision-support venture in an African farming market.

**On-slide content:**  
- **Project Focus:** Transforming an algorithmic crop classifier into an agronomic decision engine.
- **The Core Question:** Can spatial data and cooperative distribution solve the smallholder crop-choice problem?
- **Due Diligence Scope:** 10-country screening, 20+ competitor audits, and field data feasibility.
- **Current Milestone:** Pre-validation strategy review and proposed pilot roadmap.

**Evidence and citations:**  
- Krishi Sathi Due Diligence Workspace (`krishi-sathi-africa/`), October 2026.
- FAOSTAT (2024): Sub-Saharan Africa agricultural livelihoods overview [https://www.fao.org/faostat/].

**Recommended visual:**  
- *Visual Type:* Editorial title card with a subtle dual-layer background: a stylized satellite NDVI contour overlay paired with a clean project hierarchy diagram.
- *Underlying Data:* None (Branding/Title card).
- *Caveat:* Avoid generic stock photos of smiling farmers with smartphones.

**Speaker notes:**  
"Welcome. Today I’m presenting our venture discovery and due-diligence findings for Krishi Sathi Africa. Krishi Sathi began as a machine-learning concept designed to recommend suitable crops based on soil and weather data. Over the past several weeks, our team conducted a rigorous, skeptical due-diligence exercise to test whether this idea has real commercial and agronomic viability in Africa. Rather than rushing to launch an app, we treated our starting assumptions as unverified hypotheses. Today, I’ll walk you through what the agricultural data actually shows, why our original concept had to pivot, why Tanzania has emerged as our leading country candidate, and the specific validation plan we are proposing."

**Transition:**  
"To understand why we pivoted, we first have to examine the original concept and why conventional machine learning fails when taken to the field."

---

# Slide 2 — From Crop Prediction to Decision Support

**Purpose:**  
Explain the structural breakdown of conventional crop prediction models and the necessity of transitioning to holistic decision support.

**Key message:**  
Classroom machine learning models that predict single crops from farmer-entered soil chemistry fail in Africa because smallholders do not have soil tests, while farming requires risk-hedged systems.

**On-slide content:**  
- **The "Ideal Soil Test" Fallacy:** $<2\%$ of African smallholders have lab soil tests; tests cost \$20–\$50 per sample.
- **Agronomic Blindspots:** Synthetic Kaggle models predict Indian crops (jute, apples); they omit African staples (cassava, sorghum, cowpea).
- **Monoculture vs. Reality:** Algorithms optimize for a single crop; smallholders practice intercropping to hedge climate risk.
- **The Solution:** Shift from pure ML classification to a **hybrid agronomic-economic decision engine**.

**Evidence and citations:**  
- Kaggle Crop Recommendation Dataset (Atharva Ingle, 2020) [https://www.kaggle.com/datasets/atharvaingle/crop-recommendation-dataset].
- AfSIS / iSDA Soil Survey Data: $<2\%$ smallholder testing frequency [https://doi.org/10.1038/s41598-021-85601-3].
- J-AIT (Kumar et al., 2021): Critique of ML in smallholder cropping systems [https://doi.org/10.1016/j.jait.2021.03.004].

**Recommended visual:**  
- *Visual Type:* Conceptual architecture comparison diagram (Before vs. After).
- *Left Panel (Before):* Black-box ML model taking 7 numerical NPK inputs $\rightarrow$ Output: Single crop label (Fragile, disconnected).
- *Right Panel (After):* Hybrid engine combining open spatial data $\rightarrow$ Agronomic constraints $\rightarrow$ Economic optimization $\rightarrow$ Diversified acreage plan.
- *Data Status:* Conceptual architectural framework based on audited research literature.

**Speaker notes:**  
"Most crop recommendation projects online use Atharva Ingle’s Kaggle dataset, achieving 99% accuracy by predicting crops from nitrogen, phosphorus, potassium, and pH. But in Sub-Saharan Africa, fewer than two percent of smallholders have ever tested their soil because a single test costs up to fifty dollars. Furthermore, smallholders don’t plant single-crop monocultures—they practice mixed cropping to hedge against rainfall failure. A system that tells a subsistence farmer to replace all their food crops with a cash crop without considering food security is dangerously flawed. We realized Krishi Sathi had to evolve from a basic classifier into a decision-support engine that handles soil data automatically and balances food security with commercial cash crops."

**Transition:**  
"Having recognized the need for a practical decision-support tool, we turned our attention to the African agricultural landscape to understand where this problem is most acute."

---

# Slide 3 — The Smallholder Reality: High Stakes, High Friction

**Purpose:**  
Demonstrate the macroeconomic and human significance of smallholder farming while illustrating the catastrophic downside of poor crop decisions.

**Key message:**  
Over 33 million smallholders produce 70% of Sub-Saharan Africa's food supply under 95% rain-fed conditions, where a single miscalculated planting decision can result in family debt and food insecurity.

**On-slide content:**  
- **Economic Pillar:** Agriculture generates 20%–35% of national GDP and employs $>60\%$ of the rural workforce in target markets.
- **Climate Vulnerability:** 95% of smallholder farming is rain-fed, making seasonal rainfall onset timing life-or-death.
- **The Monoculture Trap:** Farmers continuously grow low-margin staples (e.g., maize), exhausting soil nitrogen and suffering harvest price gluts.
- **The Friction:** High inorganic fertilizer costs (Urea/DAP $>45\%$ of OpEx) combined with volatile farmgate prices crush net margins.

**Evidence and citations:**  
- FAOSTAT (2024): Sub-Saharan Africa smallholder farming accounts [https://www.fao.org/faostat/].
- World Bank WDI (2024): Agriculture as % of GDP and employment [https://data.worldbank.org/indicator/NV.AGR.TOTL.ZS].
- Funk et al. (2015): CHIRPS precipitation and rain-fed vulnerability [https://doi.org/10.1038/sdata.2015.66].

**Recommended visual:**  
- *Visual Type:* Regional comparative bar chart showing Agricultural Share of GDP vs. Agricultural Share of Employment across candidate countries.
- *Underlying Data:* Tanzania (27% GDP / 66% Emp), Ethiopia (33% / 60%), Kenya (22% / 42%), Nigeria (24% / 34%), Ghana (21% / 35%).
- *Source:* World Bank Development Indicators (2024).
- *Units:* Percentage of total national accounts. Observed macroeconomic data.

**Speaker notes:**  
"Across Sub-Saharan Africa, agriculture is not just an industry—it is the primary employer and economic backbone, supporting over thirty-three million smallholder households. But these farmers operate on a knife's edge. Ninety-five percent of production is rain-fed. In regions like East Africa, farmers are trapped in continuous maize monoculture. Repetitive maize planting strips the soil of nutrients and acidifies the land. Farmers spend up to half their working capital on chemical fertilizers, only to harvest at the exact same time as everyone else, crashing local prices. When a smallholder makes a wrong crop choice, they cannot pivot next quarter—they face a year of debt and food insecurity."

**Transition:**  
"Before assuming this represented an untouched commercial opportunity, we systematically mapped the existing solutions and competitors across the continent."

---

# Slide 4 — The Competitive Landscape: This Is Not an Empty Market

**Purpose:**  
Dispel the assumption that agricultural advisory in Africa is an untouched whitespace by presenting the existing ecosystem of commercial, donor, and informal players.

**Key message:**  
The African agritech sector is populated by well-funded platforms and established informal alternatives, meaning Krishi Sathi must find a genuine, defensible niche.

**On-slide content:**  
- **Bundled Credit & Inputs:** Safaricom DigiFarm (1.2M registered; Kenya) and Apollo Agriculture (\$65M raised; Kenya/Zambia).
- **Public & Donor Advisory:** AKILIMO (IITA cassava agronomy; Nigeria/Tanzania) and Precision Development (PxD; 2M+ farmers in East Africa).
- **Hardware Soil Tech:** AgroCares (NIR scanner), restricted by \$3,000 device capex and \$10–\$15 testing fees.
- **The True Incumbent:** Local agro-dealers (*maduka ya pembejeo*) who advise $>80\%$ of farmers but have severe commercial conflicts of interest.

**Evidence and citations:**  
- GSMA AgriTech (2023): State of Digital Agriculture in Africa [https://www.gsma.com/mobilefordevelopment/agritech/].
- Safaricom Sustainability Report (2023): DigiFarm adoption metrics [https://www.safaricom.co.ke/about/sustainability/digifarm].
- J-PAL / PxD (Kremer et al., 2022): Mobile-based agricultural extension evidence [https://www.povertyactionlab.org/evaluation/mobile-based-agricultural-advisory-services].

**Recommended visual:**  
- *Visual Type:* 2x2 Positioning Matrix.
- *Axes:* X-axis = Solution Breadth (Single-Crop / Narrow Advisory vs. Holistic Farm Decision Support); Y-axis = Commercial Model (Conflicted Input Sales / Credit vs. Unconflicted Independent Advisory).
- *Placements:* Agro-dealers & Apollo in bottom-left/top-left; AKILIMO in bottom-center; DigiFarm in top-left; Krishi Sathi plotted in the top-right whitespace (Holistic + Unconflicted).

**Speaker notes:**  
"A mentor will rightfully ask: 'Aren't there already dozens of agritech startups in Africa?' The answer is yes. In Kenya, Safaricom's DigiFarm has over a million registered farmers, and Apollo Agriculture has raised sixty-five million dollars. But when you look closely at what these platforms actually do, they are primarily input distributors and credit lenders. Their advisory is an auxiliary tool to sell seeds, chemicals, and loans. In the public sector, IITA built AKILIMO, but it only addresses cassava. And the biggest incumbent of all is the local village agro-dealer, who gives advice purely to clear high-margin chemical stock from their shelves. The whitespace is an unconflicted decision tool that helps farmers diversify their crop portfolio without being tied to a specific chemical brand."

**Transition:**  
"To determine where this whitespace could realistically be captured without competing head-on with established giants, we conducted an objective multi-country screening."

---

# Slide 5 — Screening African Markets: A Structured Decision Model

**Purpose:**  
Present the 10-criteria screening methodology used to evaluate candidate markets and justify our focus.

**Key message:**  
Using a weighted multi-criteria model evaluating farmer problem severity, competitive whitespace, data availability, and unit economics, Tanzania ranked first among ten candidate countries.

**On-slide content:**  
- **Top Evaluated Markets:** Tanzania (`4.20`), Ghana (`3.65`), Kenya (`3.55`), Rwanda (`3.45`), Nigeria (`3.35`).
- **Core Weights:** Problem Severity (15%), Demand/WTP (15%), Agronomic Data (15%), Whitespace (10%), Partner Access (10%).
- **Why Kenya Ranked Lower (3.55):** Saturated by well-funded incumbents (DigiFarm, PxD, KALRO, Apollo, One Acre Fund); high customer acquisition costs.
- **Why Nigeria Ranked Lower (3.35):** Massive smallholder base, but severe currency devaluation (70%+), 30%+ inflation, and post-crowdfarming farmer skepticism.

**Evidence and citations:**  
- Krishi Sathi Country Screening Model (`research/country_screening.md`), October 2026.
- Briter Bridges (2023): Agritech in Africa Market Dynamics & Capital Flows [https://briter.co/].
- World Bank Global Findex (2024): Financial inclusion benchmarks [https://www.worldbank.org/en/publication/globalfindex].

**Recommended visual:**  
- *Visual Type:* Horizontal stacked bar comparison showing composite scores across the five finalist countries with color-coded criteria contributions.
- *Underlying Data:* Tanzania (4.20), Ghana (3.65), Kenya (3.55), Rwanda (3.45), Nigeria (3.35).
- *Source:* Krishi Sathi Weighted Decision Model (2026).
- *Caveat:* Explicitly labeled as an analytical model output under stated weighting assumptions, not an immutable fact.

**Speaker notes:**  
"We evaluated ten countries across East, West, North, and Southern Africa using a ten-criteria weighted scoring framework. We didn't just look for where agriculture is big—we looked at competitive whitespace, currency stability, and operational feasibility. Kenya is often the default choice for East African tech, but it scored third because the market is hyper-saturated. Safaricom DigiFarm and Apollo have already captured the primary channels, and donor-funded PxD provides free advice. Nigeria has massive population scale, but the macroeconomic environment—with severe currency depreciation and inflation—creates immense friction for an early-stage venture. Tanzania emerged as our highest-ranked candidate with a score of 4.20 out of 5."

**Transition:**  
"Let’s look specifically at why Tanzania provides such a compelling foundation for our initial investigation."

---

# Slide 6 — Why Tanzania Is the Leading Strategic Hypothesis

**Purpose:**  
Detail the specific agricultural, linguistic, and competitive factors supporting Tanzania as the initial target country.

**Key message:**  
Tanzania combines massive agricultural dependence (27% GDP), 6 million smallholder households, and Swahili linguistic cohesion with an absence of dominant digital advisory monopolies.

**On-slide content:**  
- **Economic Scale:** Agriculture represents 27% of GDP and employs 66% of the national workforce (6.0M smallholder households).
- **Linguistic Unity:** 100% national Swahili comprehension eliminates the multi-dialect localization friction seen in Nigeria or Ghana.
- **Digital Growth:** Mobile money account penetration stands at 55% (M-Pesa, Tigo Pesa, Airtel Money) and is expanding rapidly.
- **The Competitive Advantage:** Unlike Kenya, Tanzania has **no entrenched venture-backed digital advisory monopoly**.
- **Important Caveat:** Bureaucratic approvals with national research bodies (TARI) require disciplined local navigation.

**Evidence and citations:**  
- World Bank (2024): Tanzania Economic Update [https://www.worldbank.org/en/country/tanzania/publication/tanzania-economic-update].
- NBS Tanzania (2023): National Sample Census of Agriculture [https://www.nbs.go.tz/].
- TCDC (2023): Annual Cooperative Status Report [https://www.ushirika.go.tz/].

**Recommended visual:**  
- *Visual Type:* Strategic Country Scorecard highlighting key macro metrics (GDP share, smallholder population, mobile money adoption) alongside a checklist of competitive whitespace indicators.
- *Underlying Data:* Observed national statistics from NBS Tanzania and World Bank Global Findex (2024).
- *Caveat:* Highlight that government research collaboration requires formal MoUs.

**Speaker notes:**  
"Tanzania offers a unique combination of structural advantages. First, agriculture is central to the economy—accounting for twenty-seven percent of GDP and two-thirds of all jobs. Second, unlike West Africa, where you might have to localize software into five or six languages, Tanzania has universal Swahili literacy, allowing us to build a single, culturally cohesive conversational engine. Third, mobile money is widespread, with over half the adult population actively using mobile wallets. But most crucially, the competitive field is open. There is no dominant player like DigiFarm locking up cooperative distribution in Tanzania. It gives an agile entrant the room to establish trusted relationships."

**Transition:**  
"Within Tanzania, launching nationwide would be a mistake. We needed to identify a specific, high-potential agricultural corridor as our beachhead."

---

# Slide 7 — Proposed Beachhead: The Southern Highlands

**Purpose:**  
Present the Southern Highlands (Mbeya, Songwe, Iringa) as the recommended regional pilot territory and define the local farming system.

**Key message:**  
The Southern Highlands produce nearly half of Tanzania's maize under reliable rainfall, but farmers are trapped in an acidic, nitrogen-depleted monoculture cycle that crop diversification can break.

**On-slide content:**  
- **The National Breadbasket:** Southern Highlands produce 42%–48% of Tanzania's national maize crop.
- **Agroecological Fit:** Dependable unimodal rainfall (800–1,400 mm; Nov–May); elevations of 1,200m–2,200m.
- **The Severe Agronomic Constraint:** Acute soil acidity ($pH < 5.2$) and nitrogen depletion in ferralsols limit maize yields to $<1.8\text{ t/ha}$.
- **Anchor Institutions:** Home to **TARI Uyole Centre** in Mbeya and over **450 registered AMCOS cooperatives** in the SAGCOT corridor.
- **Integrity Note:** Krishi Sathi currently has no formal agreements with TARI or AMCOS; these are prospective targets.

**Evidence and citations:**  
- SAGCOT (2023): Southern Agricultural Growth Corridor Investment Blueprint [https://www.sagcot.co.tz/].
- TARI Uyole (2023): Soil Fertility Guidelines for the Southern Highlands [https://www.tari.go.tz/uyole].
- Ministry of Agriculture Tanzania: National Crop Production Statistics [https://www.kilimo.go.tz/].

**Recommended visual:**  
- *Visual Type:* Regional Map of Tanzania highlighting the Southern Highlands (Mbeya, Songwe, Iringa) along the SAGCOT transport corridor, annotated with rainfall bands, elevation contours, and AMCOS cooperative cluster locations.
- *Data Source:* SAGCOT Centre and Ministry of Agriculture GIS databases.
- *Caveat:* Geographic boundary illustration; pilot is strictly focused on Mbeya Rural and Mbozi districts.

**Speaker notes:**  
"We selected the Southern Highlands—specifically Mbeya, Songwe, and Iringa—as our pilot beachhead. This region is the breadbasket of Tanzania, producing nearly half the country’s maize. It has reliable unimodal rainfall, unlike the drought-prone arid regions in the north. But agronomically, the soil is exhausted. Decades of continuous maize farming have depleted soil nitrogen and caused severe soil acidification, with pH dropping below 5.2. Maize yields have stagnated below two tons per hectare. This region is also home to TARI Uyole, one of East Africa’s premier agricultural research stations, and more than 450 active agricultural marketing cooperatives, giving us a dense institutional network to approach for our pilot."

**Transition:**  
"Now let's examine what product Krishi Sathi could actually build to help these farmers escape the monoculture trap."

---

# Slide 8 — What Krishi Sathi Could Actually Build: Decision Workflow

**Purpose:**  
Illustrate the end-to-end decision-support workflow from farmer plot GPS to an actionable, plain-Swahili diversification plan.

**Key message:**  
Krishi Sathi combines automated spatial soil and climate data with economic optimization to generate a plain-Swahili acreage allocation plan that protects household food security while maximizing cash income.

**On-slide content:**  
- **Step 1: Plot GPS Capture:** Extension agent records plot coordinates via tablet app (zero farmer NPK entry).
- **Step 2: Automated Cloud Ingestion:** System queries iSDAsoil (30m soil properties) and CHIRPS (rainfall onset).
- **Step 3: Agronomic Screening:** Deterministic rules check pH, elevation, and drainage thresholds (TARI guidelines).
- **Step 4: Economic Optimization:** Constrained linear program reserves $\ge 1.0$ acre for food security (maize), allocating remainder to high-margin legumes.
- **Step 5: Swahili Action Plan:** Generates plain-language advice: *"Allocate 1.2 acres to Maize, 1.3 acres to Uyole 03 Beans; apply lime to address acidity."*

**Evidence and citations:**  
- Krishi Sathi Technical Architecture Specification (`strategy/technical_architecture.md`), October 2026.
- FAO GAEZ v4: Agro-ecological zoning and crop suitability methodology [https://gaez.fao.org/].
- TARI Uyole: Crop Enterprise Budgets and Management Guidelines [https://www.tari.go.tz/].

**Recommended visual:**  
- *Visual Type:* Process Flow Diagram showing the 5-step operational pipeline from Field Agent Input $\rightarrow$ Cloud Geospatial Ingestion $\rightarrow$ Optimization Core $\rightarrow$ Swahili Output Interface.
- *Callout Box:* Screenshot mockup of the proposed Swahili tablet interface showing an acreage allocation pie chart (60% Mahindi / 40% Maharage) and simple input checklists.
- *Data Status:* Proposed system architecture and interface specification.

**Speaker notes:**  
"Here is how the system would actually work in practice. A cooperative extension agent visits a member farmer and records their field boundary using our offline-capable tablet app. The farmer does not need to enter chemical soil numbers. The system automatically queries continental 30-meter soil maps and satellite rainfall records. It checks agronomic rules—for example, if the soil is too acidic, it alerts the farmer that lime is required. Then, an economic optimization model calculates the best land allocation. It strictly reserves at least one acre for maize so the family’s food supply is never compromised, and allocates the remaining acreage to high-value legumes like common beans. The output is a clear, actionable plan in plain Swahili delivered directly to the farmer."

**Transition:**  
"A crucial technical question is whether open geospatial data is reliable enough to generate these recommendations."

---

# Slide 9 — Data Feasibility and Agronomic Reliability

**Purpose:**  
Explain the geospatial datasets powering the engine, their scientific validation, and their operational limitations.

**Key message:**  
By utilizing continental 30m open spatial soil mapping (iSDAsoil) and satellite rainfall tracking (CHIRPS), we eliminate farmer data-entry friction, using spatial estimates as an agronomic screening prior.

**On-slide content:**  
- **iSDAsoil (30m Resolution):** Continent-scale digital soil map (CC BY 4.0 open access); predicts pH, nitrogen, phosphorus, potassium, organic carbon, and texture across Africa.
- **Scientific Validation:** Developed by iSDA and World Agroforestry (Hengl et al., *Scientific Reports* 2021); validated on ~150,000 African soil samples ($R^2 > 0.70$ for pH and texture).
- **Climate Monitoring:** CHIRPS 0.05° daily precipitation tracks seasonal rainfall onset and detects dry spells.
- **Essential Technical Caveat:** Spatial soil estimates provide an agronomic *prior*, not a laboratory assay. They identify regional acidity trends but do not replace physical testing for large capital investments.

**Evidence and citations:**  
- Hengl, T., et al. (2021): African soil properties mapped at 30 m spatial resolution, *Scientific Reports* [https://doi.org/10.1038/s41598-021-85601-3].
- iSDAsoil Open Access Platform on AWS Registry of Open Data [https://www.isda-africa.com/isdasoil/].
- Funk, C., et al. (2015): CHIRPS precipitation dataset, *Scientific Data* [https://doi.org/10.1038/sdata.2015.66].

**Recommended visual:**  
- *Visual Type:* Side-by-Side Spatial Data Comparison.
- *Left Image:* 30m pixel grid of iSDAsoil pH predictions over the Mbeya/Songwe highland corridor, illustrating localized acidity variations ($pH < 5.2$ in red/orange).
- *Right Image:* CHIRPS dekadal rainfall onset tracking chart comparing historical 30-year average onset dates vs. current season anomalies.
- *Data Source:* iSDAsoil AWS open data repository and UCSB CHC.

**Speaker notes:**  
"How do we know the soil data is credible? We leverage iSDAsoil, an extraordinary open-access dataset published in *Scientific Reports* in 2021. It mapped the entire African continent at 30-meter resolution using machine learning trained on 150,000 real soil samples. It provides reliable field-level estimates of soil pH, nitrogen, phosphorus, and organic carbon. We pair this with CHIRPS, the gold-standard satellite rainfall dataset used by USAID and FEWS NET to track rainfall onset. But we must be scientifically honest: a 30-meter satellite map cannot detect if a farmer dumped fertilizer in one corner of their plot yesterday. It serves as an agronomic screening prior to identify broad soil constraints, backed by an automated safety rule that abstains whenever climate forecasts show extreme anomalies."

**Transition:**  
"Even the best agronomic engine will fail without a viable commercial model. Let's look at how this creates value and generates revenue."

---

# Slide 10 — Business Model: B2B2C Cooperative Licensing

**Purpose:**  
Present the institutional B2B2C business model partnering with Agricultural Marketing Co-operative Societies (AMCOS).

**Key message:**  
Rather than trying to charge low-income smallholders directly, Krishi Sathi licenses its platform to cooperatives at \$1.50–\$2.00 per member per season, delivering an estimated 4x–6x return through marketing cess.

**On-slide content:**  
- **Why B2C Fails:** Smallholder willingness to pay for standalone text advice approaches zero; direct billing has $>90\%$ churn.
- **The B2B2C Mechanism:** License software directly to AMCOS cooperatives to equip their extension staff and lead farmers.
- **The Co-op Value Proposition:** By shifting members into high-value certified beans/soybeans, the AMCOS aggregates higher tonnage and collects its statutory marketing cess (2%–3%).
- **Modeled Unit Economics:** Proposed fee of **\$1.75/member/season (\$3.50/year)**; estimated 50 co-ops in Year 2 (35,000 farmers) yields **\$122,500 ARR at 77% gross margin**.
- **Commercial Status:** Pro-forma financial simulation; pricing and willingness to pay are hypotheses to be validated in field interviews.

**Evidence and citations:**  
- TARI Uyole (2023): Enterprise Budgets for Common Beans (Gross Margin: TZS 670k/acre vs. TZS 320k for maize) [https://www.tari.go.tz/uyole].
- TCDC (2023): Cooperative Marketing Cess Regulations [https://www.ushirika.go.tz/].
- Krishi Sathi Business Model & Unit Economics (`research/business_model.md`), October 2026.

**Recommended visual:**  
- *Visual Type:* Value Creation & Flow of Funds Diagram.
- *Flow:* Krishi Sathi licenses software to AMCOS (\$1.75/season) $\rightarrow$ Co-op extension advises farmer $\rightarrow$ Farmer gross margin increases (+\$135/acre) $\rightarrow$ Produce aggregated at AMCOS $\rightarrow$ AMCOS earns incremental marketing cess (\$8–\$12/member).
- *Data Status:* Modeled financial simulation based on TARI gross margin benchmarks.

**Speaker notes:**  
"Our business model is built on one hard lesson from African agritech: never try to charge smallholders directly for software. Smallholders have zero willingness to pay for digital advice, and churn rates exceed ninety percent once promotional credits end. Instead, we propose a B2B2C model licensing directly to Agricultural Marketing Co-operative Societies, or AMCOS. In Tanzania, cooperatives earn their revenue by aggregating member produce and collecting a two-to-three percent statutory marketing fee. When a farmer switches an acre from maize to certified common beans, their net gross margin doubles from \$123 to \$258. For the cooperative, aggregating more high-value legumes generates eight to twelve dollars in extra marketing fees. A software license of two dollars per member delivers an immediate four-to-six-times return for the cooperative."

**Transition:**  
"While this model is compelling on paper, our due diligence surfaced several critical risks that could derail the venture."

---

# Slide 11 — Major Risks and How We Propose to Test Them

**Purpose:**  
Demonstrate intellectual honesty by presenting the primary fatal failure modes and specific pre-pilot mitigation plans.

**Key message:**  
The venture faces significant execution risks—including cooperative sales cycles, seed supply chain bottlenecks, and spatial data calibration—which must be de-risked before committing capital.

**On-slide content:**  
- **Co-op Sales Cycle Drag:** AMCOS governance requires Annual General Meeting (AGM) approvals, risking 12-month sales delays.
- **Input Supply Chain Deficits:** Recommending certified legume seed (Uyole 03) fails if local agro-dealers suffer stock-outs.
- **Harvest Price Gluts:** If thousands of farmers expand legume acreage simultaneously, local markets may crash without forward buyers.
- **Spatial Map Variance:** iSDAsoil accuracy in volcanic soils must be ground-truthed against local laboratory benchmarks.
- **Venture Kill Criteria:** Project terminates if co-op boards unanimously reject paying software fees, or if spatial error exceeds 35%.

**Evidence and citations:**  
- Krishi Sathi Red-Team Review & Failure Analysis (`research/red_team_review.md`), October 2026.
- TechCabal (2022): Lessons from Nigerian crowdfarming failures [https://techcabal.com/].
- Krishi Sathi Decision Log & Kill Criteria (`validation/decision_log.md`), October 2026.

**Recommended visual:**  
- *Visual Type:* Risk Matrix & Mitigation Table displaying the 4 primary risk categories (Commercial, Operational, Agronomic, Technical), their severity/probability rating, early warning indicator, and planned mitigation action.
- *Format:* Clean 4-row structured scorecard with traffic-light status indicators.

**Speaker notes:**  
"A good investment committee looks for how an initiative might fail. We conducted an aggressive red-team pre-mortem and identified four primary risks. First, cooperative bureaucracy: AMCOS boards operate on slow, seasonal meeting cycles, which could burn our runway before we recognize revenue. Second, input availability: recommending certified Uyole 03 bean seed is useless if local village agro-dealers are stocked out or selling counterfeit seeds. Third, off-take risk: if hundreds of farmers expand soybean production and the commercial feed millers don't show up with trucks, prices will crash. And fourth, spatial accuracy in volcanic highland soils. We have established explicit 'kill criteria': if cooperative boards refuse to pay for software, or if local seed cannot be pre-stocked, we stop the project."

**Transition:**  
"To resolve these uncertainties systematically, we have designed an actionable 90-day reconnaissance and validation roadmap."

---

# Slide 12 — The Next 90 Days and Decisions for Discussion

**Purpose:**  
Outline the immediate operational milestones and present clear, strategic questions for mentor guidance.

**Key message:**  
Our immediate focus is a low-cost, 90-day field reconnaissance sprint in Mbeya to validate cooperative demand and local data before building production software.

**On-slide content:**  
- **Month 1 (Reconnaissance):** Meet TARI Uyole leadership; conduct 25 structured AMCOS interviews; audit local seed inventories.
- **Month 2 (Data & Prototype):** Ingest spatial APIs; benchmark iSDAsoil against 200 TARI soil profiles; build offline Swahili agent prototype.
- **Month 3 (Pilot Structuring):** Secure pilot agreements with 3 AMCOS cooperatives (500 farmers) for the upcoming *Masika* rains.
- **Key Mentor Questions:** Is the maize monoculture problem narrow enough? Is Tanzania the right first market? Is B2B2C cooperative licensing realistic?

**Evidence and citations:**  
- Krishi Sathi 30/60/90-Day Execution Roadmap (`strategy/execution_roadmap.md`), October 2026.
- Pilot Field Validation Protocol (`strategy/pilot_plan.md`), October 2026.
- Partner Discovery Questionnaire (`validation/partner_interview_guide.md`), October 2026.

**Recommended visual:**  
- *Visual Type:* 90-Day Gantt / Milestone Roadmap showing the three 30-day workstreams (Field Discovery, Data Pipeline, Pilot Structuring) converging on a Stage-Gate Investment Review prior to the November planting season.
- *Data Status:* Operational execution timeline.

**Speaker notes:**  
"Here is what we propose to do over the next ninety days. We are not spending money on large engineering teams or building complex apps right now. Month One is pure field reconnaissance: traveling to Mbeya, meeting with TARI Uyole researchers to negotiate a data collaboration, and interviewing twenty-five AMCOS cooperative chairpersons to test their willingness to pay. Month Two is data calibration: testing iSDAsoil against real local soil archives and building a lightweight Swahili tablet prototype. Month Three is pilot structuring: signing up three cooperatives to run a controlled 500-farmer trial during the upcoming planting season. I would value your guidance on three core questions: Is focusing strictly on maize-to-legume diversification the right entry point? Is Tanzania the best place to start? And how can we best structure cooperative contracts to avoid long bureaucratic delays?"

**Transition:**  
"Thank you. I look forward to your feedback and advice on our strategic direction."
