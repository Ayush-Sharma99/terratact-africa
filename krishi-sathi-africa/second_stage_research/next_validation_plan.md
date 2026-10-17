# Phased Validation Program, Stakeholder Discovery & 30/60/90-Day Roadmap

**Document ID:** TT-STAGE2-010  
**Author:** Head of Operations, Field Agronomy & Venture Research  
**Date:** October 2026  
**Execution Territory:** Mbeya, Songwe & Iringa (Southern Highlands, Tanzania)  
**Target Milestone:** Controlled 500-Farmer Field Pilot across 3 AMCOS Cooperatives  

---

## 1. Validation Philosophy: Testing Behavior, Not Opinions

The validation plan does not ask smallholders or cooperative leaders hypothetical questions like: *"Would you like an AI app that doubles your income?"* (to which the answer is always politely yes). 

Instead, the program executes **non-leading ethnographic and behavioral discovery** designed to reveal:
- What smallholders actually did with their acreage last season and why.
- Where their input cash was lost (fertilizer, counterfeit seed, pest shocks).
- How cooperatives make financial software decisions and allocate statutory cess revenues.
- Whether local seed distributors physically have certified legume seeds in rural depots.

```text
               PHASED VALIDATION PROGRESSION:
┌─────────────────────────┬─────────────────────────┬─────────────────────────┐
│     SPRINT 1 (Days 1-30)│    SPRINT 2 (Days 31-60)│    SPRINT 3 (Days 61-90)│
├─────────────────────────┼─────────────────────────┼─────────────────────────┤
│ • TARI Uyole formal MoU │ • Ingest spatial APIs   │ • 3-day Lead Farmer     │
│ • 25 AMCOS interviews   │ • Calibrate iSDAsoil vs.│   tablet training       │
│ • Seed inventory audit  │   200 TARI soil profiles│ • Pre-stock co-op depots│
│ • Commercial off-taker  │ • Build Swahili Android │   with certified seed   │
│   forward contract LOIs │   offline prototype     │ • Enumerate 500 farmers │
│ • BRELA/PDPA compliance │ • Sign 3 AMCOS MoUs     │ • Launch Masika pilot   │
└─────────────────────────┴─────────────────────────┴─────────────────────────┘
                                      │
                                      ▼
┌─────────────────────────────────────────────────────────────────────────────┐
│ 6-MONTH CONTROLLED FIELD TRIAL (December 2026 – June 2027)                  │
│ 350 Treatment Smallholders vs. 150 Matched Control Smallholders.            │
│ Measure: Adoption rate, yield differentials, loan recovery, co-op renewal.  │
│ Gate Decision: Scale to 50 co-ops, iterate product, or terminate venture.   │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## 2. Stakeholder Discovery Program & Non-Leading Interview Guides

### 2.1 AMCOS Cooperative Leadership Discovery (25 Interviews)
- **Target:** Board Chairpersons, Secretaries, and Cooperative Managers in Mbeya Rural, Mbozi, and Rungwe districts.
- **Key Questions:**
  1. *Financial Mechanics:* "Last season, how much total marketing cess did the AMCOS collect, and what percentage of that came from maize versus beans or other crops?"
  2. *Credit Default Drivers:* "When members fail to repay their seasonal input loans, what is the primary cause: weather failure, poor crop selection, or side-selling to cash buyers?"
  3. *Software Budgeting:* "What specific process does the board follow to approve an operational expense of TZS 4,000–5,000 (\$1.50–\$2.00) per member, and does it require District Co-operative Officer (DCO) sanction?"
  4. *Lead Farmer Capability:* "How many extension officers or lead farmers does the co-op currently deploy, and what tools do they use to track member plots?"

### 2.2 Smallholder Farmer Discovery (50 Interviews)
- **Target:** Commercializing smallholders (1.5–3.5 acres) cultivating maize in target AMCOS villages.
- **Key Questions:**
  1. *Acreage History:* "Walk me through how you divided your land last season: how many acres of maize did you harvest, and how many bags did your family consume versus sell?"
  2. *Soil Exhaustion Reality:* "How much fertilizer did you apply per acre five years ago compared to last season, and what has happened to your harvest volume over that time?"
  3. *Varietal Decision-Making:* "When the rains start late in December, do you change the seed variety you buy at the store, or do you plant your usual seed and hope the rains last?"
  4. *Downside Risk Perception:* "If someone guaranteed to buy 5 bags of soybeans at a fixed price, would you reduce your maize acreage by one acre, or is having maize in your granary non-negotiable?"

### 2.3 Local Seed Distributors & Agro-Dealers (15 Audits)
- **Target:** Wholesale agro-dealers and distributors (Tanseed International, Beula Seed, regional depots) in Mbeya and Vwawa.
- **Key Questions:**
  1. *Physical Inventory Realities:* "How many 2kg and 10kg bags of certified Uyole 03 bean seed do you typically have in your warehouse 2 weeks before the planting rains?"
  2. *Inoculant Handling:* "Do you stock *Rhizobium* inoculants for soybeans, and how do you store them to prevent heat spoilage in rural shops?"
  3. *Counterfeit Margins:* "What percentage of legume seed sold in village retail shops is uncertified grain sorted from open markets, and why do farmers buy it?"

### 2.4 Commercial Off-Takers & Grain Processors (5 Interviews)
- **Target:** Animal feed millers (Dar es Salaam, Arusha), regional grain aggregators, and the National Food Reserve Agency (NFRA).
- **Key Questions:**
  1. *Procurement Targets:* "What is your annual volume requirement for non-GMO soybeans and common beans, and what moisture content/quality standards do you enforce?"
  2. *Forward Contracts:* "Would your company sign a forward-purchase agreement with an AMCOS cooperative guaranteeing a minimum floor price if acreage and planting dates were digitally verified?"

---

## 3. Data Validation & Model Calibration Protocol

Before deploying recommendations to farmers, the data science team must complete two empirical calibration steps:

1. **iSDAsoil Ground-Truthing:** Extract 30m soil pH, organic carbon, and texture predictions for 200 historical sampling coordinates across Mbeya, Songwe, and Iringa. Compare predictions against physical wet-chemistry laboratory records from TARI Uyole.
   - *Tolerance Threshold:* Mean Absolute Error (MAE) for soil pH must be $<0.4$ pH units. If error exceeds $0.4$, the model must apply regional calibration offsets.
2. **Rainfall Onset Dynamic Testing:** Backtest the CHIRPS dekadal rainfall onset algorithm against historical Southern Highland seasons (1995–2025). Verify that the algorithm accurately identifies early versus delayed onset dates and correlates with historical regional maize-bean yield anomalies.

---

## 4. 30 / 60 / 90-Day Operational Execution Roadmap

### Sprint 1: Days 1 to 30 (Reconnaissance, Stakeholder Interviews & Legal Formation)
- [ ] Establish operational field base in Mbeya town.
- [ ] Conduct formal executive meeting with TARI Uyole Centre Director; negotiate research data-sharing MoU.
- [ ] Execute 25 structured AMCOS cooperative leadership discovery interviews.
- [ ] Audit certified legume seed inventory with Tanseed International and Beula Seed Company.
- [ ] Interview 2 commercial poultry feed millers in Dar es Salaam to establish forward off-take parameters.
- [ ] Submit Tanzanian subsidiary incorporation documents to BRELA; initiate PDPA compliance filings.
- [ ] **Stage-Gate Review 1:** Confirm cooperative willingness to pay and certified seed availability.

### Sprint 2: Days 31 to 60 (Data Ingestion, Model Calibration & App Prototyping)
- [ ] Implement cloud API connector querying iSDAsoil 30m and CHIRPS rainfall for Southern Highland coordinates.
- [ ] Complete cross-validation benchmark of iSDAsoil against 200 TARI soil profile archives.
- [ ] Code the Stage 1 Agronomic Exclusion Rules and Stage 3 Constrained Acreage Optimizer in Python.
- [ ] Build offline-first Swahili Android tablet prototype for cooperative extension officers.
- [ ] Negotiate and sign formal pilot agreements with 3 selected AMCOS boards (target: 500 member farmers).
- [ ] **Stage-Gate Review 2:** Verify that the software prototype operates reliably offline on a low-cost Android tablet.

### Sprint 3: Days 61 to 90 (Lead Farmer Training, Pre-Stocking & Pilot Enrolment)
- [ ] Conduct intensive 3-day train-the-trainer workshops for 10 AMCOS Lead Farmers on tablet operation and farmer consultation.
- [ ] Pre-clear and physically inspect certified Uyole 03 seed and agricultural lime batches in AMCOS village depots.
- [ ] Enumerate 500 pilot smallholders; capture plot GPS boundaries; generate customized Swahili acreage diversification plans.
- [ ] Configure Africa’s Talking SMS gateway for automated planting window notifications.
- [ ] Dispatch seasonal onset SMS alerts upon confirmed initiation of *Masika* rains; initiate planting supervision.
- [ ] **Stage-Gate Review 3:** Confirm 100% of pilot plots mapped and certified seeds delivered to depots before planting rains start.

---

## 5. Controlled Field Pilot Design (Months 4 to 9 / Dec 2026 – Jun 2027)

To isolate the causal economic impact of TerraTact, the trial executes a **quasi-experimental matched-cohort evaluation**:
- **Treatment Cohort ($N = 350$ Farmers):** Receives TerraTact Swahili multi-season diversification plans, dynamic planting window SMS alerts, and co-op pre-cleared certified seeds (Uyole 03 bean / Uyole Soya) with lime.
- **Control Cohort ($N = 150$ Farmers):** Matched smallholders within the same cooperative wards who continue standard farming practices (unassisted continuous maize monoculture).
- **Measurement Timeline:** Baseline survey (Month 3) $\rightarrow$ In-season agronomic monitoring (Months 4–6) $\rightarrow$ Endline harvest weighbridge audit & economic survey (Month 9).

---

## 6. Pre-Established Go / No-Go Decision Scorecard

At the conclusion of the harvest in June 2027, the venture committee evaluates results against four strict criteria:

| Metric ID | Indicator | Target Goal | Minimum Acceptable | Red Flag / Halt |
|---|---|:---:|:---:|:---:|
| **GATE-01** | **Recommendation Adoption Rate** | $\ge 70\%$ of farmers | $50\%$ of farmers | $< 40\%$ (Farmers reject plan) |
| **GATE-02** | **Household Net Income Differential** | $\ge +35\%$ vs Control | $\ge +20\%$ vs Control | $< +10\%$ (No economic impact) |
| **GATE-03** | **Cooperative Enterprise Renewal** | $\ge 2$ of 3 Co-ops renew | $1$ Co-op renews | $0$ Co-ops renew (Commercial failure) |
| **GATE-04** | **Input Loan Repayment Rate** | $\ge 92\%$ loan recovery | $\ge 82\%$ loan recovery | $< 75\%$ (Credit risk unmanaged) |

---

## 7. Preliminary 90-Day Validation Budget

The initial 90-day field reconnaissance sprint requires a lean seed budget of **\$28,500 USD**:

```text
               90-DAY PRE-PILOT RECONNAISSANCE BUDGET (USD):
┌─────────────────────────────────────────────────────────────┬──────────────┐
│ Expense Category & Operational Scope                        │ Budget (USD) │
├─────────────────────────────────────────────────────────────┼──────────────┤
│ 1. Local Field Personnel (Lead Agronomist + 2 Enumerators)  │   $4,200     │
│ 2. Ground Travel & 4WD Fuel Logistics (Mbeya/Songwe TANZAM) │   $5,800     │
│ 3. TARI Uyole Research Collaboration & Benchmark Data Fee   │   $3,500     │
│ 4. Stakeholder Discovery & Co-op Workshop Logistics (Mbeya) │   $4,000     │
│ 5. Legal Entity Incorporation (BRELA) & Data Protection Reg │   $2,500     │
│ 6. Tablet Hardware (5 Low-Cost Samsung Android Field Tablets)│   $1,250     │
│ 7. Cloud Geospatial Infrastructure & SMS Gateway Testing    │   $1,750     │
│ 8. Contingency & Unforeseen Rural Logistics Buffer (20%)    │   $5,500     │
├─────────────────────────────────────────────────────────────┼──────────────┤
│ TOTAL 90-DAY PRE-PILOT SEED ALLOCATION                      │  $28,500 USD │
└─────────────────────────────────────────────────────────────┴──────────────┘
```
