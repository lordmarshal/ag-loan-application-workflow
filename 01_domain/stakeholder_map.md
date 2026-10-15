# Stakeholder Map
## Loan Application Workflow Domain

| Stakeholder | Role | What they care about | Influence | Interest | How the Domain Lead engages |
|---|---|---|---|---|---|
| Karen Whitford | VP Lending Operations, executive sponsor | Faster decisions, cost to serve, customer satisfaction | High | High | Weekly 1:1; monthly domain steering |
| Field Relationship Managers (about 300) | Own the customer relationship, gather applications | Less paperwork, fewer callbacks, looking good to customers | Medium | High | RM advisory group of 12; monthly listening sessions; field ride alongs |
| Credit Adjudication (Daniel Roy, Director) | Make credit decisions | Complete, accurate files; no pressure to rush decisions | High | High | Co designs completeness rules; signs off on anything touching the credit file |
| Credit Policy and Risk | Policy and portfolio risk | Policy followed; no automated credit decisions | High | Medium | Review at quarterly planning; guardrail check on each release |
| Compliance and Privacy Office | KYC, privacy, record keeping | Identity checks, privacy impact assessments, retention | High | Medium | Privacy impact assessment per release; compliance reviewer in refinement for affected stories |
| Customer Service Centre (Regina) | Answers customer calls | Fewer "where is my application?" calls, accurate information to give | Medium | High | Team lead on the RM advisory group; trained before each release |
| Lending Operations (loan administration) | Prepare documents, fund loans | Clean data, e-signature, fewer errors at funding | Medium | High | Process mapping workshops; UAT testers |
| IT Architecture and Security | Platform and security standards | Secure integration with the LOS | High | Medium | Architecture review at feature design; security testing before release |
| Data and Analytics | KPI reporting | Reliable data definitions | Low | Medium | Agree KPI definitions; build domain dashboard |
| Farm customers | Apply for credit | Simple, quick, clear, bilingual | Medium | High | Usability tests each release; CSAT survey |
| Squad Product Owners (2) | Own squad backlogs | Clear priorities, stable scope | Medium | High | Weekly PO sync; joint refinement |

## Power and interest grid

| | **Lower interest** | **Higher interest** |
|---|---|---|
| **Higher influence** | **Keep satisfied:** Credit Policy and Risk, Compliance and Privacy, IT Architecture | **Manage closely:** VP Lending Operations, Credit Adjudication |
| **Lower influence** | **Monitor:** Data and Analytics | **Keep informed and involved:** RMs, Customer Service Centre, Lending Operations, customers, Product Owners |

## The tension the Domain Lead has to manage

* **RMs and customers** want speed and fewer document requests.
* **Credit** wants complete, well supported files and will not accept "fast but thin."
* **Compliance and Privacy** want every identity check done and only necessary data collected.

The Domain Lead's job is to show these are not in conflict: a **complete file the first time** is both faster for the farmer and better for Credit. That shared goal is KR2 (first time complete applications), and it became the domain's north star metric.
