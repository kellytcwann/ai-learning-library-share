---
tags:
  - product-configuration
  - product-rules
  - brd
---

# Insurance Product Configuration Basics

這頁解釋 product configuration 如何把產品規則轉成系統行為，特別適合連接 current POS / sales platform assessment 和 BRD reformat 工作。

## 概念

Product configuration 是把產品設計和 business rules 轉成系統可執行的設定，例如 eligibility、premium mode、rider rules、document requirements、underwriting triggers。

對 current POS / sales platform assessment 和 BRD reformat 來說，核心問題是：

> 哪些產品規則只是寫在文件，哪些已配置在 current POS / sales platform 或 downstream system？

## 為什麼對保險轉型重要

產品規則如果不清晰，會令 quote 錯、application 被 block、case 變 NIGO、underwriting 多 manual referral，也會拖慢新產品上架和產品變更。

## 簡單例子

| 規則類型 | 例子 | 系統影響 |
|---|---|---|
| Eligibility | Applicant age must be 18-60 | current POS / sales platform 要檢查 age basis 和錯誤提示。 |
| Premium mode | Monthly / annual payment available | 影響 illustration、payment 和 export fields。 |
| Rider rule | Rider only available with selected base plans | 影響 product selection 和 validation。 |
| Underwriting trigger | Medical review needed above threshold | 影響 referral 和 document checklist。 |
| Channel rule | Product available to agency only | 影響 user access 和 sales journey。 |

## Key Terms / 關鍵詞

| 專業詞 | 中文 / 說明 |
|---|---|
| Base plan | 主產品。 |
| Rider | 附加產品或附加保障。 |
| Eligibility rule | 誰可以買、何時可以買。 |
| Validation rule | 系統檢查輸入是否符合規則。 |
| Referral rule | 何時要轉人工審批。 |
| Configuration owner | 負責維護系統規則的人或團隊。 |

## BA / PM Relevance

| Lens | 讀者要留意 |
|---|---|
| BA | 規則 wording、例外、source traceability、business owner。 |
| PM | product change timeline、vendor dependency、approval path、testing window。 |
| FDE | rule location、data structure、API / import format、test cases。 |

## 讀者可以問

- Which rules are configured in current POS / sales platform versus handled manually?
- Who owns product rule changes: product, IT, vendor, underwriting, or compliance?
- How are riders and eligibility rules tested before launch?
- What happens if BRD wording conflicts with system behavior?
- Which rules most often create NIGO, referral, or agent confusion?

## Meeting-Ready Wording

> 「BRD / template reformat 時，我想分清楚邊啲係 documentation clean-up，邊啲要變成 POS configuration、validation logic 或 export fields。」
