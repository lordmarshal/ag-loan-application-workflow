# Feature Prioritization (WSJF)
## Loan Application Workflow Domain

Scored at Q1 2025 quarterly planning with the sponsor, both Product Owners, Credit, Compliance and the RM advisory group.

## How WSJF works

**Weighted Shortest Job First** ranks features by the value of doing them sooner divided by their size.

* **Cost of Delay** = Business Value + Time Criticality + Risk Reduction
* **WSJF** = Cost of Delay ÷ Job Size
* Each factor is scored relative to the others on the scale 1, 2, 3, 5, 8, 13, 20.

The higher the WSJF, the sooner it should be built, **unless a dependency forces a different order.**

## Scores

| Rank | ID | Feature | Business value | Time criticality | Risk reduction | Cost of delay | Job size | WSJF | Release |
|---|---|---|---|---|---|---|---|---|---|
| 1 | F1 | Loan specific document checklist | 13 | 13 | 8 | 34 | 5 | **6.8** | R1 |
| 2 | F4 | Automated completeness check | 20 | 8 | 13 | 41 | 8 | **5.1** | R2 |
| 3 | F9 | Identity and beneficial ownership check | 8 | 13 | 20 | 41 | 8 | **5.1** | R1 |
| 4 | F12 | Customer Service Centre status view | 5 | 8 | 2 | 15 | 3 | **5.0** | R3 |
| 5 | F2 | Online application form (operating and equipment) | 13 | 13 | 5 | 31 | 8 | **3.9** | R1 |
| 6 | F6 | Customer and RM status tracker | 8 | 8 | 3 | 19 | 5 | **3.8** | R3 |
| 7 | F3 | Secure document upload portal | 13 | 8 | 8 | 29 | 8 | **3.6** | R2 |
| 8 | F5 | Data flow to LOS (no retyping) | 13 | 5 | 13 | 31 | 13 | **2.4** | R2 |
| 9 | F7 | E-signature for loan documents | 8 | 5 | 5 | 18 | 8 | **2.3** | R3 |
| 10 | F10 | RM workload dashboard | 5 | 3 | 2 | 10 | 5 | **2.0** | R3 |
| 11 | F11 | Pre filled operating line renewals | 8 | 2 | 1 | 11 | 8 | **1.4** | 2026 |
| 12 | F8 | Land and real estate loan applications | 8 | 3 | 3 | 14 | 13 | **1.1** | 2026 |

## Why the release order is not exactly the WSJF order

* **F4 (completeness check) needs F3 (upload portal)** to have documents to check, so both go in R2.
* **F12 (Customer Service Centre view) needs F6 (status tracker)** data, so both go in R3.
* **F9 (identity check) is a compliance guardrail.** It must be live before any customer submits an application online, so it goes in R1 regardless of score.
* **F8 (land loans)** has high value per loan but complex rules (appraisals, environmental reviews) and low WSJF. Moved to 2026 so 2025 could focus on the highest volume products, operating lines and equipment loans, which are about 78% of applications.

## The Domain Lead's role here

The Domain Lead runs the scoring session, makes sure each group's view is heard (Credit tends to score risk reduction high, RMs score time criticality high), challenges inflated scores with data from discovery, and explains the final order to everyone, including what did **not** make 2025 and why.
