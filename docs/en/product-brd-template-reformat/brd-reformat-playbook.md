---
tags:
  - brd
  - template-reformat
  - product-rules
  - export
---

# Product BRD Reformat Playbook

A practical playbook for converting legacy product BRDs/templates into structured, reviewable, traceable, and export-ready requirements.

## Objective

Turn old product BRDs/templates into a consistent requirement structure that can support product governance, POS configuration, migration, reporting, or automation.

## When To Use

- When legacy templates need to be reformatted.
- When the batch of legacy templates/items is not yet clearly defined.
- When product documents need to become structured rules, trackers, or export fields.

## Step-by-Step Approach

1. Confirm count unit: product, rider, document, rule, section, export row.
2. Build inventory: ID, source file, owner, format, status, open questions.
3. Extract facts exactly as written before rewriting.
4. Standardise requirement language: must, should, may, exception, open question.
5. Map to POS / downstream impact: validation, screen field, document checklist, referral, export field.
6. Review and sign off with product, system, compliance, or underwriting owners as needed.

## Example

| Old Wording | Standard Requirement | Export / System Impact | Open Question |
|---|---|---|---|
| Applicant should be 18-60 | Applicant must be aged 18 to 60 inclusive at application date | `min_age`, `max_age`, `age_basis` | Applies to rider also? |
| Monthly payment available | Product must support monthly premium mode where eligible | `payment_mode=monthly` | Any minimum premium? |
| Medical may be needed | POS must flag medical referral based on defined underwriting rules | referral trigger | Rule stored in POS or underwriting system? |

## Risk / Compliance Considerations

- Do not silently reinterpret unclear product rules.
- Keep source references for audit and reviewer confidence.
- Suitability, disclosure, underwriting, and premium rules need careful review.
- AI extraction can accelerate drafting, but human sign-off is required.
- Export-ready does not mean business-approved unless approval is recorded.

## Expected Outputs

- BRD inventory tracker.
- Standardised requirement template.
- Open question log with owners.
- Export field mapping.
- Review / approval status.

## Meeting-Ready Wording

> “Before reformatting, we should confirm count unit, target export format, required fields, and review owner so the output is consistent and usable.”

