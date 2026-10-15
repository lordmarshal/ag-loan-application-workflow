# Feature Specification: F4 Automated Completeness Check
## Loan Application Workflow Domain

| Item | Detail |
|---|---|
| Feature | F4 Automated completeness check |
| Release | R2 (July 14, 2025) |
| Squad | B: Origination Integration |
| Author | Blessing Adeniyi, Domain Lead, with the Squad B Product Owner |
| Reviewed by | Daniel Roy (Credit Adjudication), Compliance and Privacy Office, RM advisory group |
| Status | Approved April 25, 2025 |

## 1. Problem

42% of applications reach the RM incomplete, and 1 in 4 files that reach Credit are sent back with questions. 12 of the 21 days to a decision are spent chasing documents.

## 2. Outcome we want

* First time complete applications rise from 58% to 85% (KR2)
* Files returned by Credit fall from 25% to under 10%

## 3. What it does

When a customer uploads a document, the system checks it against the checklist for their loan type and farm structure and tells them right away what is missing, out of date or unreadable. The customer cannot submit until all mandatory items are present, unless the RM overrides with a written reason.

**It does not** judge creditworthiness, read financial ratios, or recommend a decision.

## 4. Business rules (agreed with Credit)

| Rule | Check | Applies to | If it fails |
|---|---|---|---|
| BR1 | All mandatory checklist items uploaded | All | Item listed as missing; submit blocked |
| BR2 | Financial statements cover the most recent fiscal year | Operating, equipment | Flag "out of date"; submit blocked |
| BR3 | Two most recent years of tax returns or notices of assessment | Operating, equipment | Item listed as missing |
| BR4 | Legal name on documents matches the applicant entity | Corporations, partnerships | Flag for RM review (not blocked) |
| BR5 | File is readable (not blank, corrupt or password locked) | All | Customer asked to upload again |
| BR6 | Equipment quote or bill of sale included | Equipment | Item listed as missing |
| BR7 | Beneficial ownership completed (from F9) | Corporations, partnerships | Submit blocked |

## 5. Acceptance criteria

```gherkin
Scenario: Customer uploads everything required
  Given a sole owner applying for an operating line
  And all mandatory checklist items are uploaded and current
  When the customer views their checklist
  Then every item shows as complete
  And the Submit button is enabled

Scenario: Financial statements are out of date
  Given a corporation applying for an equipment loan
  When the customer uploads financial statements for a fiscal year older than the most recent one
  Then the item is flagged "Out of date: please upload your most recent year"
  And the message is shown in the customer's chosen language
  And the Submit button stays disabled

Scenario: RM overrides a blocked submission
  Given an application with one missing mandatory item
  When the RM chooses Override and enters a reason of at least 30 characters
  Then the application can be submitted
  And the override, reason, RM name and time are recorded in the audit log
```

## 6. Non functional requirements

* Check result shown within 10 seconds of upload
* Messages in English and French
* WCAG 2.1 AA
* Every check result and override logged for audit

## 7. Measures after launch

| Measure | Baseline | Target | How measured |
|---|---|---|---|
| First time complete applications | 58% | 85% | Applications submitted with completeness score 100% |
| Files returned by Credit | 25% | under 10% | LOS return reason codes |
| RM overrides | not applicable | under 5% of submissions | Audit log |

## 8. Risks

* Rules too strict could frustrate customers. **Response:** RM override with reason; monthly review of override reasons with Credit.
* Credit policy changes. **Response:** rules kept in an editable table (story LA04).
