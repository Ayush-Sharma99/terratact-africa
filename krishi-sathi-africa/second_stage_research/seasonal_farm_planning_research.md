# Seasonal Farm Planning, Varietal Selection & Agronomic Sustainability

**Document ID:** TT-STAGE2-003  
**Author:** Multidisciplinary Agronomy, Ag-Economics & Climate Modeling Team  
**Date:** October 2026  
**Geographic Scope:** East & Southern Africa Focus (Tanzania Southern Highlands & Regional Corridors)  

---

## 1. Deconstructing "Seasonal Farm Intelligence"

Smallholder agriculture in Sub-Saharan Africa is not a static, one-time decision. It is an ongoing, multi-season sequence of risk-management choices governed by climate variability, soil exhaustion, input cash flows, and changing market prices [^1][^2].

When smallholders ask:  
*"What should I plant in the coming season, using which locally available variety, given my land, the rainfall outlook, my cash budget, and potential buyers—and what should I plant after harvest?"*  
...they are asking for **dynamic seasonal farm planning**, not a generic crop classification label.

```text
               THE YEAR-ROUND DYNAMIC FARMING CYCLE:
┌─────────────────────────┬─────────────────────────┬─────────────────────────┐
│  PRE-SEASON (Oct - Nov) │  IN-SEASON (Dec - Apr)  │  POST-HARVEST (May - Sep│
├─────────────────────────┼─────────────────────────┼─────────────────────────┤
│ • Onset date tracking   │ • Staggered weeding     │ • Harvest aggregation   │
│ • Varietal maturity pick│ • Legume intercropping  │ • Soil organic cover    │
│   (short vs long cycle) │ • Soil moisture checks  │ • Residual moisture use │
│ • Seed inventory audit  │ • Micro-dosing top dress│ • Crop rotation plan    │
│ • Acreage allocation    │ • FAW pest scouting     │   for next season       │
└─────────────────────────┴─────────────────────────┴─────────────────────────┘
```

---

## 2. Crop Calendars and Dynamic Planting Windows

### 2.1 The Limits of Static Crop Calendars (FAO Baseline)
The Food and Agriculture Organization (FAO) maintains national and zonal crop calendars for 44 African countries [^3]. For Tanzania's Southern Highlands, the static FAO calendar benchmarks:
- **Maize:** Planting: November 15 – December 31; Harvesting: May 1 – June 30.
- **Common Beans:** Season 1 Planting: November 15 – December 15; Harvesting: February 15 – March 15. Season 2 (*Vuli* / Residual): Planting: February 15 – March 15; Harvesting: May 15 – June 15.
- **Soybeans:** Planting: December 1 – December 31; Harvesting: April 15 – May 30.

**The Failure of Static Calendars:** In a changing climate, rainfall onset in the Southern Highlands fluctuates by up to **4 to 6 weeks** from historical averages due to Indian Ocean Dipole (IOD) and El Niño-Southern Oscillation (ENSO) anomalies [^4]. 

If a farmer plants a long-duration maize variety (140 days) following a static calendar when the rains are delayed until late December, the crop will experience terminal drought during the critical grain-filling stage in April.

### 2.2 Dynamic Varietal Selection: The Core Technical Innovation
TerraTact’s decision engine introduces **Dynamic Varietal Matching**, linking satellite rainfall onset tracking (CHIRPS) to certified varietal maturity days (TOSCI / TARI catalogues) [^4][^5]:

```text
┌─────────────────────────────────────────────────────────────────────────────┐
│                   DYNAMIC SEED VARIETAL DECISION LOGIC:                     │
│                                                                             │
│  [CHIRPS / TMA Onset Tracking for Southern Highlands Corridor]              │
│                                   │                                         │
│         ┌─────────────────────────┴─────────────────────────┐               │
│         ▼                                                   ▼               │
│  EARLY ONSET (Before Dec 5)                         DELAYED ONSET (After Dec 20)  │
│  • Full 140-150 day window                          • Shortened 90-110 day window │
│  • Recommend: Medium/Late Hybrid                    • Exclude: Late Hybrid Maize  │
│    Maize (SC627 / UH6303)                           • Recommend: Short-Duration   │
│  • Expected Yield: 2.2-2.8 t/acre                   • Seed Varieties:             │
│  • High gross margin potential                        - Bean: Uyole 03 (75 days)  │
│                                                       - Maize: UH615 (105 days)   │
│                                                       - Cowpea: Tumaini (70 days) │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## 3. Agronomic Sustainability: Crop Rotation and Soil Restoration

### 3.1 The Cereal-Legume Nitrogen Fixing Dynamics
Continuous maize monoculture extracts between 60 and 90 kg of Nitrogen ($N$) per hectare per season from Southern Highland soils. Because smallholders can rarely afford recommended application rates (typically applying $<40\text{ kg N/ha}$ instead of the recommended $100–120\text{ kg N/ha}$), the soil operates at a severe chronic nutrient deficit [^2][^6].

Integrating certified legumes into a structured rotation cycle creates massive biological benefits [^6][^7]:
- **Biological Nitrogen Fixation (BNF):** Inoculated soybeans (*Glycine max*) and common beans (*Phaseolus vulgaris*) fix between **35 and 80 kg of atmospheric $N_2$ per hectare** via symbiotic *Rhizobium* bacteria [^6].
- **Fertilizer Substitution Value:** A maize crop planted in rotation after an inoculated soybean or bean harvest yields **15% to 30% higher grain volume** while requiring 40% less synthetic top-dressed Urea, directly saving the farmer TZS 70,000–120,000 per acre in variable chemical costs [^6][^7].
- **Pest and Disease Disruption:** Rotating cereals with non-host legumes breaks the lifecycle of the parasitic witchweed (*Striga asiatica*), maize stalk borer (*Busseola fusca*), and the fungal pathogen causing maize lethal necrosis disease (MLND) [^7].

---

## 4. Competitive Audit of Existing Planning Tools

We systematically investigated whether existing digital tools already solve multi-season farm planning:

| Tool / Platform | Developer / Backer | Actual Supported Capabilities | Operating Geography | Why It Does Not Solve TerraTact's Problem |
|---|---|---|---|---|
| **FAO Crop Calendar** [^3] | FAO | Static country/zonal planting and harvesting tables. | Pan-African | Static historical guidelines; zero dynamic weather adaptation; zero farm-level economic optimization. |
| **AKILIMO Scheduled Planting** [^8] | IITA / ACAI | Dynamic planting and harvesting date optimization for cassava roots. | Nigeria, Tanzania, Ghana | **Restricted strictly to cassava** to manage starch factory supply; does not plan multi-crop rotations or legume diversification. |
| **TMA Dekadal Bulletins** [^9] | Tanzania Met Authority | 10-day rainfall summaries and national agro-meteorological advisories. | Tanzania | Broadcast PDF bulletins; non-interactive; cannot generate farm-specific field acreage plans. |
| **Digital Green / Farmer.Chat** [^10] | Digital Green | LLM conversational chatbot answering farmer queries on agronomy. | Kenya, Ethiopia | General conversational advice; does not optimize constrained mathematical acreage allocations or track co-op inventory. |
| **Farmforce / Croplands** [^11] | Commercial AgTech | Enterprise farm management, traceability, and GlobalGAP compliance. | Pan-African (Exporters) | Expensive B2B SaaS built for large commercial export plantations; inaccessible to smallholder cooperatives. |

---

## 5. The Underserved Core: TerraTact's Differentiated Value

TerraTact does not claim that crop calendars are new. The genuine, underserved whitespace is:

```text
┌─────────────────────────────────────────────────────────────────────────────┐
│                     TERRATACT'S DIFFERENTIATED NICHE:                       │
│                                                                             │
│  "Dynamic, localized varietal matching and multi-season rotation planning,  │
│   constrained by smallholder food security and pre-verified against         │
│   cooperative seed inventory."                                              │
│                                                                             │
│  1. Dynamic: Adjusts varietal recommendation to real-time rainfall onset.   │
│  2. Grounded: Exclusively recommends certified varieties in local depots.   │
│  3. Sustainable: Enforces cereal-legume rotations to restore soil nitrogen. │
│  4. De-risked: Pre-locks forward off-take contracts before switching crops. │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## 6. References & Empirical Sources

[^1]: World Bank. (2023). *Tanzania Economic Update: Transforming Agriculture for Resilient Livelihoods*. Washington, DC: World Bank Group.
[^2]: Tanzania Agricultural Research Institute (TARI) Uyole. (2023). *Soil Fertility and Fertilizer Management in the Southern Highlands of Tanzania*. Mbeya: TARI.
[^3]: Food and Agriculture Organization (FAO). (2024). *FAO Crop Calendar Database*. Rome: FAO. Available at: https://www.fao.org/agriculture/crop-calendar/
[^4]: Funk, C., et al. (2015). "The climate hazards infrared precipitation with stations—a new environmental record for monitoring extremes." *Scientific Data*, 2, 150066. https://doi.org/10.1038/sdata.2015.66.
[^5]: Tanzania Official Seed Certification Institute (TOSCI). (2023). *National List of Registered and Certified Crop Varieties in Tanzania*. Morogoro: TOSCI.
[^6]: International Institute of Tropical Agriculture (IITA). (2022). *Biological Nitrogen Fixation and Legume Agronomy in East African Smallholder Systems*. Ibadan: IITA.
[^7]: CIMMYT. (2023). *Cereal-Legume Diversification and Conservation Agriculture in Eastern and Southern Africa*. Nairobi: CIMMYT.
[^8]: AKILIMO / IITA. (2022). *Scheduled Planting and Harvest Tool: Operational Synthesis*. Available at: https://www.akilimo.org/
[^9]: Tanzania Meteorological Authority (TMA). (2024). *National Agro-Meteorological Dekadal Bulletins and Climate Outlook*. Dodoma: TMA. Available at: https://www.meteo.go.tz/
[^10]: Digital Green. (2024). *Farmer.Chat: Generative AI for Agricultural Extension*. Available at: https://www.digitalgreen.org/farmerchat/
[^11]: Farmforce. (2023). *First-Mile Traceability and Smallholder Management SaaS*. Available at: https://www.farmforce.com/
