---
tags:
  - sales-journey-ai
  - ai-governance
  - insurance-ai
---

# Sales Journey AI Notes

這頁幫讀者用保險銷售 journey 角度理解 AI use cases，重點是 pain point、data、human control、metric 和 compliance。

## 概念

Sales Journey AI 是把 AI 放到保險銷售流程中，支援 agent、operations、underwriting 或 product team 做搜尋、摘要、檢查、解釋和下一步建議。

好的 AI use case 不應由技術開始，而應由 pain point 開始：

```text
Pain point → user → data → AI support → human control → metric
```

## 為什麼對保險轉型重要

保險銷售涉及 suitability、披露、客戶資料、健康/財務資訊和 underwriting。AI 可以減少 manual work，但必須有 review、audit trail、approved sources 和清楚責任邊界。

## 簡單例子

| Journey Step | Practical AI Support | Control |
|---|---|---|
| Product query | Agent asks approved product/process questions | Approved sources + citations |
| Illustration | Explain quote outputs in plain language | Approved wording + disclaimer |
| Application | Check missing or inconsistent fields | Agent confirms before submission |
| Document upload | Identify missing KYC/supporting documents | Confidence threshold + exception queue |
| BRD reformat | Extract product rules from old templates | Source traceability + reviewer sign-off |

## Key Terms / 關鍵詞

| 專業詞 | 中文 / 說明 |
|---|---|
| Grounding | AI 回答基於已批准資料，不是自由發揮。 |
| Human-in-the-loop | 人負責確認重要輸出或決策。 |
| Audit trail | 保留輸出、來源、使用者、時間等記錄。 |
| Data readiness | 資料是否可用、結構化、準確、被批准使用。 |
| Suitability guardrail | 防止 AI 越過合規和銷售建議控制。 |

## BA / PM Relevance

| Lens | 讀者要做什麼 |
|---|---|
| BA | 把 AI idea 連到 journey step、pain point、data source、control。 |
| PM | 定義 pilot scope、owner、approval path、success metric。 |
| FDE | 判斷是否需要 POS integration、logging、data pipeline 或 prototype。 |

## 讀者可以問

- Which journey pain point would this AI use case solve?
- What data would the AI use, and is it approved?
- Who reviews the output before it affects customer or case handling?
- What metric would prove value: NIGO rate, cycle time, search time, rework?
- Does this need to be inside current POS / sales platform, or can it start as a side assistant?

## Meeting-Ready Wording

> 「我建議每個 AI idea 都先用 user pain point、data readiness、human review point、compliance risk 同 measurable outcome 去評估，再決定 priority。」
