# Stage 9: Red-Team Review, Failure Modes & Pre-Mortem Analysis

**Author:** Multidisciplinary Investment Committee & Agritech Due Diligence Team  
**Date of Assessment:** October 2026  
**Document ID:** KS-RED-009  

---

## 1. Executive Directive: Arguing Against the Venture

Before capital is committed or engineering time is expended, the due diligence team acts as an adversarial investment committee. **Our mandate is to find the fatal flaws in Krishi Sathi and establish the exact conditions under which the venture will collapse.**

---

## 2. Three Plausible Fatal Failure Scenarios

```text
               THREE FATAL AGRITECH PRE-MORTEM VECTORS:
┌─────────────────────────┬─────────────────────────┬─────────────────────────┐
│       SCENARIO 1        │       SCENARIO 2        │       SCENARIO 3        │
│   The Input Supply      │  The Co-op Sales Cycle  │  The Harvest Glut &     │
│   Chain Disconnect      │  & Cash Burn Trap       │  Off-Taker Default      │
├─────────────────────────┼─────────────────────────┼─────────────────────────┤
│ • Model recommends seed │ • AMCOS co-op decision- │ • Farmers adopt legumes;│
│   & lime correctly.     │   making is seasonal &  │   bumper harvest.       │
│ • Local agro-dealers    │   bureaucratic (12 mo). │ • Off-takers lack cash; │
│   have stock-outs.      │ • Planting window missed│   prices crash 50%.     │
│ • Counterfeit seeds fail│ • Seed capital exhausted│ • Farmers face severe   │
│ • Software blamed.      │   before ARR booked.    │   debt & reject app.    │
└─────────────────────────┴─────────────────────────┴─────────────────────────┘
```

### Scenario 1: The "Input Supply Chain Disconnect" (Execution Blindspot)
- **The Failure Sequence:** Krishi Sathi's hybrid engine accurately recommends planting *Common Bean (Uyole 03)* and applying 150 kg of agricultural lime per acre to neutralize soil acidity in Songwe. However, the local village agro-dealers (*maduka ya pembejeo*) do not have certified Uyole 03 in stock, or local lime quarries have transport delays. Farmers either buy uncertified, diseased local grain masquerading as seed or skip the lime. 
- **The Catastrophe:** Yields collapse due to seed-borne bean common mosaic virus (BCMV) and persistent aluminium toxicity. Farmers and AMCOS co-op leaders hold the software directly responsible. Brand trust is permanently destroyed in Year 1.
- **Early Warning Indicators:** 
  - Agro-dealer stock audits in target wards reveal zero certified legume seed inventory 4 weeks prior to the onset of rains.
- **Mandatory Mitigation:** Krishi Sathi cannot operate as isolated software. It must integrate an **inventory pre-clearance protocol**, only recommending seed varieties and amendments pre-stocked in partnership with local AMCOS depots or vetted distributors (e.g., Beula Seed, Tanseed International).

### Scenario 2: The "Cooperative Bureaucracy & Cash Burn Trap" (Financial Insolvency)
- **The Failure Sequence:** The B2B2C model assumes AMCOS co-operatives will contract Krishi Sathi at \$2.00/farmer. In reality, co-op expenditure decisions require approval during Annual General Meetings (AGMs) and sanction from the District Co-operative Officer (DCO) and the Tanzania Cooperative Development Commission (TCDC).
- **The Catastrophe:** Sales cycles drag from 2 months to 14 months. The venture misses the November planting window, meaning zero software revenue can be recognized for an entire calendar year. The company runs out of runway and collapses into liquidation.
- **Early Warning Indicators:**
  - Inability to secure signed Letters of Intent (LOIs) from at least 3 AMCOS chairpersons within 60 days of field engagement.
- **Mandatory Mitigation:** Structure early pilot deployments under **pre-funded donor/ecosystem innovation vouchers** (e.g., SAGCOT catalytic grants, AGRA innovation funds) to subsidize co-op onboarding during the initial regulatory cycle.

### Scenario 3: The "Harvest Glut & Off-Taker Liquidity Shock" (Economic Collapse)
- **The Failure Sequence:** 2,000 pilot smallholders follow Krishi Sathi’s recommendation, shifting 40% of their land into soybeans. Regional production surges by 1,500 metric tons. However, the commercial poultry feed miller in Dar es Salaam experiences working capital shortages and fails to send trucks to Mbeya. 
- **The Catastrophe:** Farmgate soybean prices plunge from TZS 1,200/kg to TZS 600/kg. Unlike maize, which the household can eat or store for months, soybeans cannot easily be consumed as daily family subsistence. Farmers face severe cash losses and food insecurity.
- **Early Warning Indicators:**
  - Off-takers refuse to sign formal forward-purchase agreements or demand bank guarantees before the planting season begins.
- **Mandatory Mitigation:** **The Off-Taker Pre-Lock Rule:** Krishi Sathi must strictly forbid recommending commercial crop switching unless a verified forward off-take agreement or warehouse receipt system (WRS) contract is registered with the partner AMCOS.

---

## 3. Explicit Venture "Kill Criteria" (When to Terminate the Project)

The investment committee establishes four non-negotiable **Stop Conditions**:

```text
               MANDATORY VENTURE KILL CRITERIA:
[KILL-01] AMCOS REJECTION:
  If 10 surveyed AMCOS cooperative boards unanimously refuse to allocate a 
  $1.50-$2.00 cess per farmer for decision-support software.
  -> ACTION: Terminate commercial software venture immediately.

[KILL-02] SPATIAL INACCURACY THRESHOLD:
  If field ground-truthing of iSDAsoil in Mbeya/Songwe reveals > 35% error in pH
  or texture relative to TARI wet-chemistry lab benchmarks.
  -> ACTION: Halt automated spatial recommendations; require physical testing.

[KILL-03] UNRELIABLE OFF-TAKE:
  If formal forward off-take agreements cannot be established with at least 
  two commercial legume buyers prior to season launch.
  -> ACTION: Do not advise farmers to switch acreage away from maize.

[KILL-04] CURRENCY & INFLATION OVERHEAT:
  If Tanzanian inflation or macro regulations restrict foreign currency 
  repatriation or co-op marketing cess collections.
  -> ACTION: Freeze regional expansion.
```
