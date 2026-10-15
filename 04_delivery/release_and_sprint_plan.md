# Release and Sprint Plan
## Loan Application Workflow Domain

Two squads work in aligned two week sprints. Sprint 1 started January 13, 2025.

## Release calendar

| Release | Sprints | Build window | Go live | Features |
|---|---|---|---|---|
| R1 | 1 to 6 | Jan 13 to Apr 4 | **Apr 7, 2025** | F9, F1, F2 |
| R2 | 7 to 12 | Apr 7 to Jul 11 | **Jul 14, 2025** | F3, F4, F5 |
| R3 | 13 to 19 | Jul 14 to Oct 17 | **Oct 20, 2025** | F6, F12, F7, F10 |
| Stabilize | 20 to 23 | Oct 20 to Dec 12 | | Fixes, tuning, 2026 discovery |

The [product backlog](../03_roadmap_backlog/product_backlog.md) lists feature level stories. Squads split each into smaller stories and tasks in Jira during refinement, so sprint level points are tracked in Jira rather than in this document.

## Each release follows the same path

1. **Refine** with Product Owners, Credit and Compliance reviewers (Definition of Ready)
2. **Build** in sprints with demos every two weeks to the RM advisory group
3. **Privacy and security review** before release
4. **Pilot** with 3 field offices for 2 weeks
5. **Train** RMs and Customer Service Centre agents
6. **Release** to all offices
7. **Measure** against the KRs and feed results into the next quarterly plan

## Pilots

| Release | Pilot offices | Pilot window | Key finding | Change made |
|---|---|---|---|---|
| R1 | Swift Current SK, Red Deer AB, Brandon MB | Mar 17 to Mar 28 | Customers did not understand "beneficial owner" | Added plain language help text in both languages |
| R2 | Same 3 plus Saint Hyacinthe QC | Jun 23 to Jul 4 | Rule BR4 (name match) flagged too many valid farm corporations using trade names | BR4 changed from blocking to "flag for RM review" |
| R3 | 5 offices | Sep 29 to Oct 10 | Customer Service Centre agents could not tell if a status was stale | "Last updated" date and time added to the agent view (LA19) |

## Ceremonies (domain level)

| Ceremony | Who | When |
|---|---|---|
| Quarterly planning | Domain Lead, POs, squads, sponsor, Credit, Compliance | First week of each quarter |
| Product Owner sync | Domain Lead, both POs | Weekly |
| Joint sprint review and demo | Both squads, RM advisory group, Customer Service Centre lead | Every 2 weeks |
| Domain retrospective | Domain Lead, POs, squad leads | Every release |
| KPI review | Domain Lead, Data and Analytics, sponsor | Monthly |

## Dependencies managed by the Domain Lead

| Dependency | From | Needed for | Status |
|---|---|---|---|
| LOS integration API | IT Core Lending team | F5 (R2) | Delivered May 30 |
| Identity verification service contract | Procurement | F9 (R1) | Signed Feb 14 |
| E-signature provider approval | IT Security and Legal | F7 (R3) | Approved Jul 25 |
| French translation capacity | Translation services | All releases | Booked per release |
| Checklist rules sign off | Credit Adjudication | F1 (R1), F4 (R2) | Signed Feb 28 and Apr 25 |
