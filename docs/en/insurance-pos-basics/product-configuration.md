---
tags:
  - product-configuration
  - product-rules
  - brd
---

# Insurance Product Configuration Basics

Product configuration translates product rules into system behaviour, including eligibility, riders, premium modes, validation rules, document requirements, and referral triggers.

## Why It Matters

Unclear product rules can cause quote errors, blocked applications, NIGO, manual referrals, and slow product launches or product changes.

## Examples

| Rule Type | Example | System Impact |
|---|---|---|
| Eligibility | Applicant age must be 18-60 | POS validates age basis and error messages. |
| Premium mode | Monthly / annual payment available | Impacts illustration, payment, and export fields. |
| Rider rule | Rider only available with selected base plans | Impacts product selection and validation. |
| Underwriting trigger | Medical review needed above threshold | Impacts referral and document checklist. |

## Key Terms

| Term | Meaning |
|---|---|
| Base plan | Main product. |
| Rider | Optional add-on product or benefit. |
| Eligibility rule | Who can buy and when. |
| Validation rule | System check against business rules. |
| Referral rule | When manual review is required. |
| Configuration owner | Team responsible for maintaining system rules. |

## BA / PM Relevance

| Lens | What To Watch |
|---|---|
| BA | Rule wording, exceptions, source traceability, business owner. |
| PM | Product change timeline, vendor dependency, approval path, testing window. |
| FDE | Rule location, data structure, API/import format, test cases. |

## Questions To Ask

- Which rules are configured in the current POS / sales platform versus handled manually?
- Who owns product rule changes: product, IT, vendor, underwriting, or compliance?
- How are riders and eligibility rules tested before launch?
- What happens if BRD wording conflicts with system behaviour?

## Meeting-Ready Wording

> “For BRD/template reformatting, I would separate documentation clean-up from rules that need to become POS configuration, validation logic, or export fields.”

