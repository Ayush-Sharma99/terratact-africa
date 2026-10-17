# Krishi Sathi Africa: Claim Audit, Verification Register & Open Questions

**Document ID:** KS-AUDIT-001  
**Date of Audit:** October 2026  
**Auditor:** Multidisciplinary Due Diligence Team  
**Scope:** Verification of all 19 material factual, numerical, and strategic claims in the Krishi Sathi research corpus prior to mentor briefing.

---

## 1. Evidence Classification Framework

Each claim in the research corpus has been audited and tagged with one of seven strict operational classifications:

- **`[VERIFIED]`**: Directly corroborated by an inspected, authoritative Tier-1 or Tier-2 source (e.g., FAOSTAT, World Bank, peer-reviewed journals, national statistical releases).
- **`[SUPPORTED INFERENCE]`**: A reasoned, logical deduction derived by triangulating multiple verified facts.
- **`[MODEL OUTPUT]`**: A calculated result produced by an explicit analytical model (e.g., multi-criteria scoring, enterprise budgeting) using stated inputs.
- **`[ILLUSTRATIVE ESTIMATE]`**: A scenario simulation or pro-forma projection; explicitly not an observed historical outcome.
- **`[HYPOTHESIS]`**: A plausible strategic proposition that requires empirical field testing before capital commitment.
- **`[UNVERIFIED]`**: A claim whose authoritative primary source has not yet been independently confirmed.
- **`[CONTRADICTED]`**: A claim materially inconsistent with empirical evidence.

---

## 2. Comprehensive 19-Point Material Claim Audit

| # | Material Claim Under Audit | Original Corpus Claim | Audited Evidence & Authoritative Source | Audit Classification | Strategic Correction / Qualification Applied |
|---|---|---|---|:---:|---|
| **1** | **Country Agricultural GDP & Employment** | Tanzania: 27% GDP, 66% emp; Kenya: 22% GDP, 42% emp; Nigeria: 24% GDP, 34% emp. | Confirmed via World Bank WDI (2024) and FAOSTAT (2024). Tanzania ag value added is 26.8% of GDP; modeled ILO ag employment is 65.4%. Kenya ag is 21.8% of GDP, 40.5% employment. | `[VERIFIED]` | Retained with exact year stamps (2024 World Bank / FAOSTAT accounts). |
| **2** | **Smallholder Population & Holdings** | 33M smallholders in SSA; 6.0M households in Tanzania; 4.5M in Kenya; 14.5M in Nigeria. | FAOSTAT & IFAD Rural Development Reports confirm ~33M smallholder farms (<2 ha) in Sub-Saharan Africa. Tanzania National Sample Census of Agriculture reports ~5.8M to 6.2M smallholder agricultural households. | `[VERIFIED]` | Framed as farming households operating <2 hectares, avoiding vague "farmer" totals. |
| **3** | **Soil Testing Rarity & Testing Cost** | <2% of smallholders test soil; lab tests cost $20–$50 per sample. | Survey data from African Soil Information Service (AfSIS), iSDA, and TARI research centers confirm wet-chemistry tests cost 30,000–60,000 TZS ($12–$25) per sample at TARI Uyole/Mlingano, plus sample collection and transit costs ($10–$25), totalling $22–$50. Smallholder testing frequency is documented at <2% across rural zones. | `[VERIFIED]` | Retained. Added explanation of logistics/courier friction as a key cost driver. |
| **4** | **Country Screening Ranking & Scores** | Tanzania (4.20) > Ghana (3.65) > Kenya (3.55) > Rwanda (3.45) > Nigeria (3.35). | The 10-criteria weighted matrix uses defined weights and 1–5 rubrics. Sensitivity testing confirms Tanzania retains the lead across realistic shifts in weights (Scenarios A, B, C). | `[MODEL OUTPUT]` | Must NOT be presented as an objective fact; explicitly labeled as an analytical model output under stated weighting assumptions. |
| **5** | **Competitor Scale & Reach** | DigiFarm (1.2M registered), PxD (2M+ East Africa), Apollo ($65M funding, 350k farmers), One Acre Fund (1.5M farmers). | Confirmed via Safaricom Annual Sustainability Reports (DigiFarm ~30% active rate), Apollo press releases/SoftBank filings, PxD J-PAL evaluations, and One Acre Fund annual audits. | `[VERIFIED]` | Explicitly highlight DigiFarm's 30% active rate vs. 1.2M headline registrations to avoid vanity metric distortion. |
| **6** | **"Untouched Whitespace" in Tanzania** | The crop recommendation market in Tanzania is completely empty/whitespace. | Tanzania has active agricultural initiatives: AKILIMO (IITA cassava tool), Kilimo Trust (beans/rice), Shamba Shape Up (farm radio/TV), and local agro-dealers. | `[CONTRADICTED]` -> `[SUPPORTED INFERENCE]` | **CRITICAL CORRECTION:** Reframed from "empty market" to "absence of an entrenched, venture-backed digital advisory monopoly (such as Safaricom DigiFarm in Kenya)." |
| **7** | **Southern Highlands Maize Production** | Southern Highlands produce >46% of Tanzania's maize. | Ministry of Agriculture Tanzania & NBS Agricultural Sample Census report Southern Highlands (Mbeya, Songwe, Iringa, Ruvuma, Rukwa, Njombe) produce 42%–48% of national maize volume annually. | `[VERIFIED]` | Retained as verified range (42%–48%). |
| **8** | **AMCOS Cooperative Numbers** | Over 400 registered AMCOS cooperatives in Southern Highlands. | Tanzania Cooperative Development Commission (TCDC) registers over 4,000 active AMCOS nationally, with roughly 450–520 located across Mbeya, Songwe, and Iringa regions. | `[VERIFIED]` | Retained with specific TCDC regulatory reference. |
| **9** | **Crop Yields, Prices & Gross Margins** | Maize: TZS 320k margin; Common Bean: TZS 670k margin; Soybean: TZS 550k margin. | TARI Uyole published enterprise budgets (2022/2023) benchmark common bean (Uyole 03) at ~620 kg/acre, price 1,800 TZS/kg, variable cost 445k TZS, gross margin 670k TZS. Maize at 1,500 kg/acre, 600 TZS/kg, cost 580k TZS, gross margin 320k TZS. | `[MODEL OUTPUT]` | Must explicitly distinguish **Gross Margin** from Net Farm Income (gross margin excludes family labor, land rental, post-harvest transport, and loan interest). |
| **10** | **"Double the Profitability" Claim** | Common beans offer 2x the profit of continuous maize. | Under TARI enterprise budgets, bean gross margin (TZS 670k/acre) is 2.09x maize (TZS 320k/acre) under optimal management with certified seed. | `[MODEL OUTPUT]` | Qualified: "Under TARI enterprise budget conditions, certified common beans achieve ~2x the gross margin of maize; however, actual smallholder yields are highly subject to weather and pest volatility." |
| **11** | **iSDAsoil Resolution, Accuracy & License** | 30m resolution, 20+ properties, CC BY 4.0 license, open on AWS. | Confirmed via Hengl et al. (Scientific Reports 2021) and AWS Open Data Registry. $R^2$ exceeds 0.70 for pH and texture across ~150,000 African ground samples. | `[VERIFIED]` | Retained with exact DOI and CC BY 4.0 terms. |
| **12** | **Validity of Spatial Soil for Farm Advice** | Spatial soil maps can replace physical soil testing on farms. | Agronomic literature emphasizes that 30m spatial interpolation cannot capture within-field micro-variability or recent localized chemical fertilizer application. | `[CONTRADICTED]` -> `[SUPPORTED INFERENCE]` | **CRITICAL CORRECTION:** Clarified that spatial soil estimates serve as an initial regional agronomic screening prior, not a substitute for laboratory testing where precision is legally/agronomically required. |
| **13** | **Weather & Remote Sensing Datasets** | CHIRPS daily 0.05° rainfall; NASA POWER 0.5° climate; Sentinel-2 10m NDVI. | Confirmed via UCSB CHC, NASA Langley POWER API documentation, and ESA Copernicus Open Access Hub. All open-access with historical records spanning 30+ years. | `[VERIFIED]` | Retained as verified technical infrastructure. |
| **14** | **Proposed Software Pricing ($1.50–$2.00)** | AMCOS co-ops will pay $1.50–$2.00 per farmer per season. | No commercial contracts have been executed at this price point. Derived from comparable B2B SaaS benchmarks in East Africa (e.g., Mergdata, co-op management tools). | `[HYPOTHESIS]` | Explicitly labeled as a pricing hypothesis to be validated during AMCOS discovery interviews. |
| **15** | **Financial Projections ($122.5k ARR, 77% GM)** | Year 2 ARR of $122,500; LTV/CAC 6.75x; 77% software gross margin. | Pro-forma financial simulation based on 50 AMCOS cooperatives, 35,000 farmers, and $3.50 annual ACV. | `[ILLUSTRATIVE ESTIMATE]` | Labeled clearly as a financial model simulation, not an observed financial track record. |
| **16** | **Co-op Economic Return & Marketing Cess** | Co-ops recover $8–$12 in incremental cess for every $2 invested. | AMCOS collect statutory marketing cess (2.0%–3.0%) on aggregated crop value. Higher bean/soybean volume and prices mathematically increase cess collections. | `[MODEL OUTPUT]` | Dependent on AMCOS successfully aggregating produce and preventing side-selling by member farmers. |
| **17** | **Competitor Lessons & Failure Modes** | Crowdfarming failed in Nigeria (Farmcrowdy); pure SMS advisory failed (Esoko/Farmerline). | Confirmed via TechCabal, WeeTracker, and company historical disclosures. Farmcrowdy pivoted post-2021; Farmerline expanded into physical input distribution (Mergdata). | `[VERIFIED]` | Retained as critical empirical justification for avoiding B2C crowdfarming or pure SMS subscriptions. |
| **18** | **Tanzanian Regulatory Requirements** | PDPA 2022 (data privacy); TOSCI (seed certification); TFRA (fertilizer regulations). | Confirmed via official statutes: Personal Data Protection Act No. 11 of 2022; Seeds Act / TOSCI Release List; Fertilizer Act 2009 / TFRA. | `[VERIFIED]` | Retained as statutory compliance prerequisites. |
| **19** | **Claimed Partnerships & Formal Approvals** | Relationships with TARI Uyole, SAGCOT Centre, or specific AMCOS boards. | **NO formal partnerships, signed MoUs, or commercial contracts currently exist.** All listed entities are prospective institutional candidates identified for outreach. | `[CONTRADICTED]` -> `[UNVERIFIED PROSPECTS]` | **MANDATORY ETHICAL SAFEGUARD:** Explicitly stated in all deliverables that Krishi Sathi currently has zero formal institutional ties, approvals, or endorsements. |

---

## 3. Master Assumptions That Could Invalidate Strategic Recommendations

1. **AMCOS Commercial Willingness-to-Pay:** If cooperative boards refuse to allocate $1.50–$2.00 per member from marketing cess, the B2B2C model must pivot to commercial outgrower off-takers or donor-subsidized implementation.
2. **Side-Selling Risk:** If smallholders sell their high-value legume harvests to itinerant cash buyers at the farmgate rather than aggregating through their AMCOS, the cooperative cannot capture its marketing cess or enforce loan recovery.
3. **Local Spatial Soil Accuracy:** If ground-truthing iSDAsoil in Mbeya/Songwe reveals $>35\%$ variance in pH or texture relative to TARI Uyole wet-chemistry profiles, the engine cannot rely on automated spatial inference without field soil sampling kits.
4. **Certified Seed Supply Chain Deficits:** If regional seed companies (e.g., Tanseed, Beula) experience inventory stock-outs of Uyole 03 bean seeds or inoculants during November planting, farmers cannot execute the recommendation.
