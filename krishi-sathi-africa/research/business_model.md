# Stage 7: Business Models, Monetization Strategy & Unit Economics

**Author:** Multidisciplinary Investment Committee & Agritech Due Diligence Team  
**Date of Assessment:** October 2026  
**Document ID:** KS-BIZ-007  

---

## 1. Comparative Business Model Analysis

To prevent the monetization traps that caused previous agritech platforms to fail, we evaluate five potential commercial models against empirical Sub-Saharan African benchmarks [^1][^2]:

| Business Model | Target Customer | Value Proposition | Farmer Cash Friction | Scalability & Retention | Commercial Verdict |
|---|---|---|:---:|:---:|---|
| **A. Farmer-Paid B2C Subscription** | Rural Smallholder | Standalone crop advice via app/SMS | **Prohibitive** (Zero WTP for pure text advice) | Extremely poor; >90% churn once promotional credits expire | **FATALLY FLAWED (REJECTED)** |
| **B. B2B Input Dealer White-Label** | Chemical/Seed Retailers | Advisory tool for agro-dealers | Zero (Dealer pays) | Compromised; dealers subvert advice to sell high-margin chemicals | **REJECTED (Conflict of Interest)** |
| **C. B2B2C Co-op & Off-Taker Licensing** | **AMCOS Co-ops & Outgrowers** | **Yield consistency, default reduction & volume aggregation** | **Zero direct cash** (Funded via marketing cess) | **High; multi-year enterprise contracts with institutional buyers** | **RECOMMENDED CORE MODEL** |
| **D. B2G National Extension Contract** | Ministry of Agriculture | Modernizing public extension agents | Zero (State pays) | High reach, but vulnerable to political transitions & delayed payments | **SECONDARY (Grant/Pilot Phase)** |
| **E. Embedded Fintech Commission** | Rural Banks (CRDB, NMB) | Alternative credit risk scoring via spatial crop suitability | Zero (Bank pays success fee) | High margin, but requires 18-month banking regulatory approvals | **FUTURE EXPANSION (Phase III)** |

---

## 2. The Core B2B2C Commercial Model: The AMCOS Ecosystem

In Tanzania, **Agricultural Marketing Co-operative Societies (AMCOS)** are the legal, financial, and logistical backbone of smallholder agriculture [^3]. Over 400 AMCOS operate in the Southern Highlands alone, legally chartered under the Tanzania Cooperative Development Commission (TCDC) [^3].

```text
               THE B2B2C VALUE RECOVERY LOOP:
┌─────────────────────────────────────────────────────────────────────────────┐
│ 1. Enterprise Contract: Krishi Sathi licenses its Decision Engine to AMCOS  │
│    Co-operative Management at $2.00 per farmer / season.                    │
├─────────────────────────────────────────────────────────────────────────────┤
│ 2. Co-op Deployment: AMCOS Extension Officers use Krishi Sathi tablet app   │
│    to profile farmer plots & issue Swahili rotation/fertilizer plans.       │
├─────────────────────────────────────────────────────────────────────────────┤
│ 3. Agronomic Outcome: Farmer shifts 40% of acreage from low-margin maize to │
│    certified Common Beans / Soybeans, generating +$130 net income per acre. │
├─────────────────────────────────────────────────────────────────────────────┤
│ 4. Co-op Monetization: AMCOS aggregates 25% higher produce volume and collects│
│    a 2.5% statutory marketing cess on higher-value legume harvests.         │
├─────────────────────────────────────────────────────────────────────────────┤
│ 5. Economic Return: Co-op recovers $8-$12 in incremental marketing revenue  │
│    for every $2.00 invested in Krishi Sathi software -> 4x-6x Co-op ROI!    │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## 3. Unit Economics & Pro-Forma Financial Model (Southern Highlands)

### 3.1 Unit Economic Metrics per Farmer (Annual - 2 Cropping Seasons)

| Metric | Base Case (USD) | Notes & Assumptions |
|---|:---:|---|
| **Annual Contract Value (ACV) per Farmer** | **\$3.50** | \$1.75 per cropping season billed to AMCOS Co-operative |
| **Customer Acquisition Cost (CAC) per Farmer** | **\$1.20** | Institutional sales cycle (\$1,200 per 1,000-member AMCOS) |
| **Cloud Hosting & API Ingestion Cost per User** | **\$0.30** | AWS S3/STAC iSDAsoil queries + serverless inference |
| **Field Agent Training & Support Cost** | **\$0.50** | Co-op agronomist training amortized across member base |
| **Gross Margin per Farmer** | **\$2.70 (77.1%)** | Highly scalable software gross margin structure |
| **LTV / CAC Ratio (3-Year Customer Life)** | **6.75x** | Conservative assumption of 3-year AMCOS contract retention |

### 3.2 3-Year Scaling Trajectory & Break-Even Analysis

```text
┌─────────┬──────────────┬──────────────────┬───────────────┬────────────────┐
│  Year   │ Target AMCOS │ Onboarded Farmers│ Gross Revenue │ Net Operating  │
│         │  Co-ops      │ (Southern Highl.)│    (ARR)      │     Result     │
├─────────┼──────────────┼──────────────────┼───────────────┼────────────────┤
│ Year 1  │   10 co-ops  │   5,000 farmers  │   $17,500     │   -$32,000 *   │
│ Year 2  │   50 co-ops  │  35,000 farmers  │  $122,500     │   +$18,500     │
│ Year 3  │  150 co-ops  │ 120,000 farmers  │  $420,000     │  +$165,000     │
└─────────┴──────────────┴──────────────────┴───────────────┴────────────────┘
(* Year 1 subsidized by catalytic innovation grants; cash-flow positive by Year 2.)
```

---

## 4. References & Sources for Stage 7

[^1]: GSMA AgriTech. (2023). *Financial Sustainability and Monetization in African Digital Agriculture*. London: GSMA.
[^2]: Briter Bridges. (2023). *Africa Agritech Investment and Platform Directory*. Available at: https://briter.co/
[^3]: Tanzania Cooperative Development Commission (TCDC). (2023). *Annual Status Report on Agricultural Marketing Co-operative Societies (AMCOS)*. Dodoma: Ministry of Agriculture.
