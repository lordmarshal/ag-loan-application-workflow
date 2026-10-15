# Domain Charter
## Loan Application Workflow Domain

| Item | Detail |
|---|---|
| Organization | Prairie Harvest Credit (fictional national agriculture lender), Regina, Saskatchewan |
| Domain | Loan Application Workflow: everything from a customer's first request for credit to a complete file ready for a credit decision, and the status updates until funding |
| Domain Lead | Blessing Adeniyi, PMP |
| Executive sponsor | Karen Whitford, Vice President, Lending Operations |
| Period covered | January to December 2025 |

## 1. What a domain is, and what the Domain Lead owns

A domain is one area of the business that is owned end to end by one accountable leader, supported by cross functional delivery squads. The Domain Lead does not write code or approve credit. The Domain Lead owns **the outcome**: a loan application process that is fast, accurate, compliant and easy for farmers and staff.

The Domain Lead is accountable for:
* The domain **vision, roadmap and priorities**
* The **business process** (current state, future state, procedures)
* **Outcome measures** (KPIs and OKRs) and reporting on them
* Aligning **stakeholders**: lending operations, field relationship managers (RMs), credit, risk, compliance, privacy, IT and the Customer Service Centre
* Guiding the **Product Owners** of the two squads so their backlogs serve the domain goals
* Making sure every change respects **credit policy, privacy, KYC and record keeping** requirements

## 2. Vision

> *A farmer can apply for credit in under 30 minutes, knows exactly what documents are needed, and always knows where their application stands. Our people spend their time on advice and judgement, not chasing paperwork or retyping data.*

## 3. In scope

* Application intake for operating lines and equipment loans in 2025 (land and real estate loans planned for 2026)
* Document checklists, upload and completeness checks
* Flow of application data into the loan origination system (LOS)
* Application status visibility for customers, RMs and the Customer Service Centre
* E-signature of loan documents
* Full service in English and French

## 4. Out of scope

* Credit adjudication rules and the credit decision itself (owned by Credit; always made by a person)
* Pricing and product design
* Loan servicing after funding
* Replacing the loan origination system

## 5. Baseline (Q4 2024)

| Measure | Baseline |
|---|---|
| Applications per year | about 14,000 (peaks February to April and September to November) |
| Time from application to credit decision | 21 business days average |
| Applications complete the first time | 58% |
| Follow up requests per incomplete application | 3.4 on average |
| RM admin time per application | 6.5 hours |
| Data entry error rate in LOS | 7% of files |
| "Where is my application?" calls to the Customer Service Centre | about 2,300 a month |
| Customer satisfaction with the application experience | 68% |

## 6. 2025 objectives and key results (OKRs)

**Objective 1: Make applying fast and simple for farmers**
* KR1: Cut time to credit decision from 21 to 10 business days
* KR2: Raise first time complete applications from 58% to 85%
* KR3: Raise application CSAT from 68% to 80%

**Objective 2: Give our people time back for advice**
* KR4: Cut RM admin time per application from 6.5 to 4 hours
* KR5: Cut LOS data entry errors from 7% to under 2%

**Objective 3: Nobody has to ask where their application is**
* KR6: Cut status calls to the Customer Service Centre by 50%

## 7. Teams

| Team | Focus | Members |
|---|---|---|
| Squad A: Digital Intake | Customer facing application, checklist, upload, status tracker | Product Owner, UX designer, 4 developers, QA analyst, business analyst |
| Squad B: Origination Integration | Data into the LOS, completeness rules, e-signature, RM tools | Product Owner, 4 developers, QA analyst, data analyst |
| Domain support | Lending process, change management, reporting | Domain Lead, process analyst, change and training specialist |

## 8. Guardrails (non negotiable)

1. No automated credit decisions. The system checks completeness; a credit professional decides.
2. Privacy impact assessment completed before any new customer data is collected.
3. Identity and beneficial ownership checks (KYC) are never skipped to save time.
4. Every customer facing screen and message is available in English and French at the same time.
5. Accessibility to WCAG 2.1 AA.

## 9. Governance

| Forum | Frequency | Purpose |
|---|---|---|
| Quarterly planning | Every quarter | Set priorities and capacity for both squads |
| Domain steering | Monthly | Sponsor, Credit, Risk, Compliance, IT review OKRs and decisions |
| Product Owner sync | Weekly | Domain Lead and both POs align backlogs and dependencies |
| Stakeholder demo | Every 2 weeks | Show working software to lending and field staff |
