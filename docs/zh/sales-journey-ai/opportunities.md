---
tags:
  - sales-journey-ai
  - ai-opportunities
  - quick-wins
  - insurance-ai
---

# Sales Journey AI Opportunities in Insurance

這頁整理保險 sales journey 入面可以加 AI 嘅實際位置，並清楚分開低風險 quick wins 同敏感 use cases。

## 概念

Sales Journey AI Opportunities 係指喺保險銷售流程入面，搵出 AI 可以實際幫 agent、sales support、operations、underwriting 或 product team 減少錯漏、加快處理、提升解釋能力嘅位置。

重點唔係「AI 可以做咩」，而係：

```text
邊個 user → 邊個 journey step → 咩 pain point → 用咩 approved data → 人點樣 review → 點樣量度成效
```

## 為什麼對 Client POS / Sales Platform 準備重要

current POS / sales platform 可能係 sales journey 入面嘅主要 front-office platform。AI 如果要落地，通常要同 current POS / sales platform journey、product rules、documents、case status、compliance controls 有關。

所以讀者應該先由低風險、agent-facing、可 review 嘅 use cases 開始講，避免一開始就將 AI product recommendation 或 underwriting decisioning 當 quick win。

## 低風險 Quick Wins

| Use Case | User | AI 幫咩 | 需要咩資料 | Control |
|---|---|---|---|---|
| Agent Knowledge Assistant | Agent | 查產品規則、流程、FAQ | Approved product guides、SOP、FAQ | Source citation、access control、usage log |
| Document Checklist Validator | Agent / operations | 檢查文件是否齊全 | Document checklist、uploaded documents | Confidence threshold、exception queue |
| Quote Explanation Assistant | Agent | 用易明語言解釋 illustration | Illustration output、approved wording | Approved template、disclaimer、agent review |
| Pre-submission Quality Check | Agent / sales support | Submit 前檢查漏欄位和矛盾 | Application fields、product rules、document status | User confirmation、audit trail |
| BRD Rule Extraction | Product / BA team | 從舊 template 抽 product rules | Old BRDs、templates | Source traceability、human sign-off |

## 敏感 Use Cases

| Sensitive Area | 為什麼敏感 | 要先確認 |
|---|---|---|
| Product recommendation | 可能影響 suitability 和 regulated advice | Suitability guardrails、agent review、approval |
| Suitability assessment | 涉及客戶需要和銷售合規 | Compliance sign-off、audit trail |
| Underwriting decisioning | 涉及風險接受、拒保、加費 | Underwriting governance、human decision owner |
| Customer-facing advice | 可能被視為銷售建議 | Approved wording、disclaimer、review process |
| Health / financial data use | 涉及敏感個人資料 | Data access、retention、consent、privacy review |

## BA / PM Relevance

| Lens | 讀者要留意 |
|---|---|
| BA | 將 use case 連到 journey step、pain point、data source、business rule、control。 |
| PM | 確認 owner、priority、pilot scope、timeline、decision gate、risk approval。 |
| FDE | 判斷 data availability、POS integration、logging、prototype feasibility。 |

## 讀者可以問

- 呢個 AI use case 係解決邊個 journey pain point？
- 係 agent-facing、operations-facing、underwriting-facing，定 customer-facing？
- AI 會用咩資料？資料係咪 approved source？
- Output 會由邊個 review？有冇 audit trail？
- 成效用咩 metric 量度？NIGO rate、cycle time、search time、rework？
- 呢個 use case 需要 embedded in current POS / sales platform，定可以先做 side assistant？

## Meeting-Ready Wording

> 「我會建議先由 lower-risk, agent-facing AI use cases 開始，例如 knowledge assistant、document checklist、quote explanation 同 pre-submission quality check。Product recommendation 或 underwriting support 就要再睇 suitability、data privacy、audit trail 同 human review controls。」
