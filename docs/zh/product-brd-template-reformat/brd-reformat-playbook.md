---
tags:
  - brd
  - template-reformat
  - product-rules
  - export
---

# Product BRD Reformat Playbook

這頁是處理 legacy BRD / template reformat 的工作方法，特別適合釐清「a batch of legacy templates/items」和 export 需求。

## Objective

把舊 product BRD / template 轉成一致、可審閱、可追溯、可 export 的 requirement structure，支援 POS configuration、產品治理、migration 或後續 automation。

## When To Use

- Team 提到「old template → reformat」。
- 需要處理「a batch of legacy templates/items」但未確認 item 單位。
- 需要把產品文件變成 structured rules / tracker / export fields。

## Step-by-Step Approach

1. **確認 count unit**
   - product、rider、document、rule、section、export row。
2. **建立 inventory**
   - ID、source file、owner、format、status、open questions。
3. **抽取 facts**
   - 不先改寫意思，先保留 source wording 和位置。
4. **標準化 requirement**
   - 用 must / should / may / exception / open question。
5. **映射到 current POS / sales platform / downstream impact**
   - validation、screen field、document checklist、referral、export field。
6. **review 和 sign-off**
   - product owner、IT/current POS / sales platform owner、compliance 或 underwriting 視規則而定。

## Simple Example

| Old Wording | Standard Requirement | Export / System Impact | Open Question |
|---|---|---|---|
| Applicant should be 18-60 | Applicant must be aged 18 to 60 inclusive at application date | `min_age`, `max_age`, `age_basis` | Applies to rider also? |
| Monthly payment available | Product must support monthly premium mode where eligible | `payment_mode=monthly` | Any minimum premium? |
| Medical may be needed | current POS / sales platform must flag medical referral based on defined underwriting rules | referral trigger | Rule stored in current POS / sales platform or underwriting system? |

## Discovery Questions

- What exactly are a batch of legacy templates/items?
- What is the target output: BRD, Excel tracker, CSV, system import, or approval pack?
- Who owns each product rule?
- Which rules must be configured in current POS / sales platform?
- Do we need source traceability for every reformatted requirement?
- How should missing or ambiguous rules be handled?

## Risk / Compliance Considerations

- Do not silently reinterpret unclear product rules.
- Keep source references for audit and reviewer confidence.
- Suitability, disclosure, underwriting, and premium rules need careful review.
- AI extraction can accelerate drafting, but human sign-off is required.
- Export-ready does not mean business-approved unless approval is recorded.

## Expected Outputs

- BRD inventory tracker.
- Standardized requirement template.
- Open question log with owners.
- Export field mapping.
- Review / approval status.

## Meeting-Ready Wording

> 「開始 reformat 之前，建議先 confirm count unit、target export format、required fields 同 review owner，確保 output 一致同可用。」
