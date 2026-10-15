# Product Backlog
## Loan Application Workflow Domain

Stories use the format **As a [role], I want [feature], so that [benefit].** A Jira ready version is in [jira_backlog_import.csv](jira_backlog_import.csv).

## Summary by release

| Release | Features | Stories | Points |
|---|---|---|---|
| R1 | F9, F1, F2 | 7 | 47 |
| R2 | F3, F4, F5 | 9 | 63 |
| R3 | F6, F12, F7, F10 | 7 | 35 |
| **Total** | | **23** | **145** |

## Definition of Ready (before a story enters a sprint)

* Acceptance criteria agreed with the Product Owner
* Credit, Compliance or Privacy reviewer named if the story touches the credit file, identity or personal data
* French and English text supplied or assigned
* Estimated by the squad

## Definition of Done

* Acceptance criteria met and demonstrated
* Works in English and French
* Meets WCAG 2.1 AA
* Automated tests pass; no open critical or high defects
* Audit logging confirmed where data or status changes

## F9: Identity and beneficial ownership check (Squad A, R1)

| ID | User story | Acceptance criteria | Points |
|---|---|---|---|
| LA01 | As a farm customer, I want to verify my identity online, so that I can start my application without visiting an office. | Identity verified through the approved verification service; failed checks routed to RM; result logged. | 8 |
| LA02 | As a compliance officer, I want beneficial owners of farm corporations captured, so that we know who ultimately owns and controls the business. | All owners with 25% or more captured and verified before checklist is shown. | 8 |

## F1: Loan specific document checklist (Squad A, R1)

| ID | User story | Acceptance criteria | Points |
|---|---|---|---|
| LA03 | As a farm customer, I want a checklist for my exact loan type and farm structure, so that I only send what is needed. | Checklist rules for operating lines and equipment loans, by sole owner, partnership and corporation; approved by Credit. | 8 |
| LA04 | As a Credit adjudicator, I want checklist rules maintained in one table, so that policy changes are made once. | Rules editable by authorized Credit Policy users only; every change logged. | 5 |

## F2: Online application form (Squad A, R1)

| ID | User story | Acceptance criteria | Points |
|---|---|---|---|
| LA05 | As a farm customer, I want to apply online in English or French, so that I can apply in my language at any time. | All screens and messages in both languages; save and return within 30 days. | 8 |
| LA06 | As a farm customer, I want the form to work on my phone, so that I can apply from the farm. | Passes mobile usability test with 5 customers; WCAG 2.1 AA. | 5 |
| LA07 | As an RM, I want to start an application on behalf of a customer, so that customers who prefer help are not left behind. | RM can start, customer can finish or RM completes with customer consent recorded. | 5 |

## F3: Secure document upload portal (Squad A, R2)

| ID | User story | Acceptance criteria | Points |
|---|---|---|---|
| LA08 | As a farm customer, I want to upload documents from my phone or computer, so that everything is in one place. | PDF, JPG, PNG up to 25 MB; upload confirmation shown and emailed. | 8 |
| LA09 | As an RM, I want all customer documents attached to the application, so that I stop searching my inbox. | Documents tagged to checklist item; visible to RM and Credit. | 5 |
| LA10 | As a privacy officer, I want documents stored encrypted in Canada with retention rules, so that customer data is protected. | Encryption at rest and in transit; retention applied by document type. | 5 |

## F4: Automated completeness check (Squad B, R2)

| ID | User story | Acceptance criteria | Points |
|---|---|---|---|
| LA11 | As a farm customer, I want to be told instantly if something is missing, so that I can fix it before I submit. | Missing or expired items flagged on upload; submit blocked until mandatory items present or RM override with reason. | 8 |
| LA12 | As a Credit adjudicator, I want basic document checks (right year, right entity, readable), so that files reach me complete. | Checks year of financial statements, entity name match, file readable; results shown to RM. | 13 |
| LA13 | As an RM, I want to see a completeness score before I review, so that I focus on judgement, not checklists. | Score from 0 to 100% with list of gaps. | 3 |

## F5: Data flow to LOS (Squad B, R2)

| ID | User story | Acceptance criteria | Points |
|---|---|---|---|
| LA14 | As an RM, I want application data sent to the LOS automatically, so that I never retype it. | All mapped fields populate the LOS; validation errors returned to RM within 1 minute. | 13 |
| LA15 | As Lending Operations, I want field level validation on transfer, so that errors are caught before funding. | Invalid postal codes, legal names and amounts rejected with clear message. | 5 |
| LA16 | As the Domain Lead, I want every transfer logged, so that data errors can be traced. | Transfer log with time, fields and result kept for audit. | 3 |

## F6: Customer and RM status tracker (Squad A, R3)

| ID | User story | Acceptance criteria | Points |
|---|---|---|---|
| LA17 | As a farm customer, I want to see where my application is, so that I don't need to call. | Stages: Received, Under RM review, With Credit, Decision, Documents, Funded; updates within 15 minutes. | 8 |
| LA18 | As a farm customer, I want an email or text when my status changes, so that I don't have to keep checking. | Notification preference in English or French; opt out available. | 3 |

## F12: Customer Service Centre status view (Squad A, R3)

| ID | User story | Acceptance criteria | Points |
|---|---|---|---|
| LA19 | As a Customer Service Centre agent, I want to see an application's status, so that I can answer customers on the first call. | Read only status view after identity confirmation of the caller. | 3 |

## F7: E-signature (Squad B, R3)

| ID | User story | Acceptance criteria | Points |
|---|---|---|---|
| LA20 | As a farm customer, I want to sign loan documents electronically, so that I don't drive to an office in seeding season. | E-signature through the approved provider; signed copy stored and sent to customer. | 8 |
| LA21 | As Lending Operations, I want signed documents returned to the loan file automatically, so that funding is not delayed. | Signed package attached to LOS file and status updated to Documents signed. | 5 |

## F10: RM workload dashboard (Squad B, R3)

| ID | User story | Acceptance criteria | Points |
|---|---|---|---|
| LA22 | As an RM, I want a dashboard of my open applications by stage, so that I can plan my week. | Shows count by stage, ageing, and items waiting on the customer. | 5 |
| LA23 | As a lending manager, I want team level views, so that I can balance workload in peak season. | Filter by office and RM; refreshed hourly. | 3 |
