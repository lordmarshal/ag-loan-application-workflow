# Risk and Compliance Register
## Loan Application Workflow Domain

## Compliance requirements and how the design meets them

| Requirement | What it means for this domain | How it is met | Owner |
|---|---|---|---|
| Know your client and beneficial ownership | Verify who is applying and who owns and controls farm corporations | F9 runs before the checklist; failures routed to RM; results logged | Compliance |
| Privacy (applicable federal privacy law) | Collect only what is needed; protect and retain properly | Privacy impact assessment for each release; data stored in Canada; retention by document type (LA10) | Privacy Office |
| Credit policy | Credit decisions follow policy and are made by authorized people | No automated decisions; checklist rules approved by Credit; RM review gate kept | Credit Policy |
| Record keeping and audit trail | Every decision and change traceable | Logs on uploads, checks, overrides, transfers and status changes | Domain Lead |
| Official languages | Equal service in English and French | Both languages in Definition of Done; translation in every sprint | Domain Lead |
| Accessibility | Usable by customers with disabilities | WCAG 2.1 AA in Definition of Done; tested each release | Squad A PO |
| Information security | Protect customer data and systems | Security review and testing before each release | IT Security |
| Fair and consistent treatment | Every applicant asked for the same things for the same loan | Rules based checklist replaces individual RM lists | Credit Policy |

## Risk register

Probability (P) and Impact (I) scored 1 to 5. Score = P × I.

| ID | Risk | P | I | Score | Response | Owner | Outcome |
|---|---|---|---|---|---|---|---|
| R1 | RMs see the portal as a threat to their customer relationship and keep using email | 4 | 4 | **16** | RM advisory group co designs; RM can start applications for customers (LA07); RM review gate kept | Domain Lead | 89% of applications in portal by Q4 |
| R2 | Older or less digital customers are left behind | 3 | 4 | 12 | RM assisted applications; Customer Service Centre help line; paper option stays | Domain Lead | Paper applications fell to 8% with no complaints trend |
| R3 | LOS integration API late | 3 | 5 | **15** | Early design in Q1; fallback of manual entry for R2 if needed | Squad B PO | Delivered May 30, no fallback needed |
| R4 | Completeness rules too strict, blocking good applications | 3 | 3 | 9 | Pilot; RM override; monthly override review with Credit | Domain Lead | BR4 relaxed after pilot; overrides 3.8% |
| R5 | Privacy impact assessment delays a release | 2 | 4 | 8 | Privacy Office in refinement; PIA started at design | Privacy Office | All PIAs on time |
| R6 | Seasonal peaks overload support during a release | 3 | 3 | 9 | Avoid release in peak weeks where possible; extra support rota | Domain Lead | R2 moved from June 30 to July 14 |
| R7 | French content lags English | 2 | 4 | 8 | Translation booked per sprint; bilingual in Definition of Done | Squad A PO | No release delayed |
| R8 | Identity verification service fails for rural customers with thin credit files | 3 | 3 | 9 | Fallback to in person or RM verified ID | Compliance | 6% of customers used fallback |
