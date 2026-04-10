# HSIL Hackathon 2026 — Claude Code Toolkit

> 為 HSIL Hackathon 2026 台灣站參賽者打造的 Claude Code 開源工具包
> An open-source Claude Code toolkit for HSIL Hackathon 2026 Taiwan Hub participants

**由聯合通科技 (Cloud Communication Technology Ltd.) 簡承哲專案經理製作**
在 AI 的協助下，期望提升所有參賽團隊的整體 Pitch 品質與競爭力。

---

## What is this? / 這是什麼？

這個專案提供 **13 個** [Claude Code](https://claude.ai/code) Skills（自訂指令），涵蓋從選題研究到 Pitch 演練的完整流程。任何人 clone 這個專案後，用 Claude Code 開啟，即可直接使用所有 `/` 指令。

**不需要安裝任何套件。Clone → 開 Claude Code → 開始用。**

---

## Quick Start / 快速開始

```bash
# 1. Clone 專案
git clone https://github.com/anthropic-fans/hsil-hackathon-toolkit.git
cd hsil-hackathon-toolkit

# 2. 開啟 Claude Code（以下任一方式）
claude                    # CLI
# 或在 VS Code / JetBrains 中開啟此資料夾

# 3. 輸入 / 查看所有可用指令
```

### 什麼是 Claude Code？

[Claude Code](https://claude.ai/code) 是 Anthropic 推出的 AI 程式設計與工作助手，可以在終端機、VS Code、JetBrains 或桌面版使用。本工具包利用 Claude Code 的 **Custom Slash Commands** 功能，讓你用 `/指令名` 就能啟動預設好的 AI 工作流程。

---

## Available Skills / 可用工具（13 個）

### 研究階段 — 選題、調研、理解使用者

| 指令 | 說明 | 對應評審項目 |
|------|------|------------|
| `/brainstorm` | 腦力激盪：探索 11 個參考方向、HMW 問題發想、概念評估矩陣、電梯簡報 | Problem, Solution |
| `/deep-research` | 深度研究：5 階段結構化研究（問題全景→現有解方→台灣脈絡→市場→AI 可行性） | Problem, Opportunity |
| `/user-persona` | 使用者人物誌：Persona 建立、旅程地圖、同理心地圖 | Problem, Solution |

### 分析階段 — 市場、策略、技術、法規

| 指令 | 說明 | 對應評審項目 |
|------|------|------------|
| `/market-analysis` | 市場分析：TAM/SAM/SOM（雙方法）+ 競爭矩陣 + 定位圖 + Porter's 5 Forces | Opportunity, Competition |
| `/swot-canvas` | SWOT 與商業畫布：SWOT 交叉策略 + Business Model Canvas + 台灣商業模式參考 + 單位經濟計算 | Business Model, Competition |
| `/tech-arch` | 技術架構：AI 技術選型 + 系統架構圖 + 台灣健康資料源盤點 + 合規設計 | Solution (技術可行性) |
| `/regulatory-check` | 法規檢查：SaMD 分類、PDPA 個資、跨境傳輸、健保法規、遠距醫療 | Q&A 準備 |

### 簡報階段 — 投影片內容與視覺化

| 指令 | 說明 | 對應評審項目 |
|------|------|------------|
| `/pitch-deck-guide` | 投影片教練：8 頁逐頁引導，每頁附範本、常見錯誤、時間分配 | 全部 8 項 |
| `/data-story` | 數據故事力：將數據轉化為有感描述、視覺化建議、投影片文案 | Presentation |
| `/pitch-timer` | 簡報計時：字數分析、時間預估、講稿優化、轉場語句 | Presentation |

### 演練階段 — 模擬評審與問答

| 指令 | 說明 | 對應評審項目 |
|------|------|------------|
| `/pitch-simulation` | 模擬評審：10 項標準逐項打分 + 三種評審視角 + 5 題模擬 Q&A + 改善建議 | 全部 10 項 |
| `/qa-prep` | 問答準備：ARC 回答框架 + 5 類問題預測 + 團隊分工建議 | Q&A |

---

## Recommended Workflow / 建議工作流程

```
  ┌─────────────────────────────────────────────────────┐
  │  Day 1 上午 — 選題與研究                              │
  │                                                     │
  │  /brainstorm      探索方向、發想概念、選定題目          │
  │  /deep-research   深入研究選定的健康議題                │
  │  /user-persona    建立目標使用者人物誌                  │
  ├─────────────────────────────────────────────────────┤
  │  Day 1 下午 — 分析與設計                              │
  │                                                     │
  │  /market-analysis  市場規模 + 競品分析                 │
  │  /swot-canvas      SWOT + 商業模式設計                 │
  │  /tech-arch        技術架構設計                        │
  │  /regulatory-check 法規合規快速檢查                    │
  ├─────────────────────────────────────────────────────┤
  │  Day 2 上午 — 簡報製作                                │
  │                                                     │
  │  /pitch-deck-guide 逐頁建立 8 頁投影片                 │
  │  /data-story       數據故事化 + 視覺化建議              │
  │  /pitch-timer      檢查時間分配                        │
  ├─────────────────────────────────────────────────────┤
  │  Day 2 下午 — 演練與上台                              │
  │                                                     │
  │  /pitch-simulation 模擬評審打分（反覆練習）              │
  │  /qa-prep          準備評審 Q&A                        │
  └─────────────────────────────────────────────────────┘
```

---

## How to Work with Claude / 如何與 Claude 協作

### 基本操作

```bash
# 啟動 Claude Code
claude

# 使用 Skill（輸入 / 開頭即可）
> /brainstorm

# 提供上下文（可以直接描述，不需特殊格式）
> /deep-research 我想研究台灣偏鄉的遠距心理健康服務

# 串連多個 Skill
> /market-analysis  （先跑完）
> /pitch-deck-guide （再用市場數據做投影片）
```

### 高效協作技巧

**1. 給 Claude 足夠的上下文**
```
好：「我們的方案是用 LLM 幫助偏鄉居民進行初步症狀分類，目標是減少不必要的轉診。
     團隊有 1 位醫師、2 位工程師、1 位設計師。」

不好：「幫我做一個醫療 AI。」
```

**2. 迭代改善**
```
第一輪：/pitch-deck-guide → 產出初版內容
第二輪：/pitch-simulation → 取得評分和回饋
第三輪：/pitch-deck-guide → 根據回饋修改
第四輪：/pitch-simulation → 再次評分，確認進步
```

**3. 善用 Skills 之間的串接**
每個 Skill 結束時都會建議「下一步」用哪個 Skill，形成自然的工作流。

**4. 將產出儲存到檔案**
```
> 請把這份研究報告存到 research/topic-analysis.md
> 請把投影片大綱更新到 templates/pitch-deck-outline.md
```

**5. 團隊分工**
- 不同隊員可以同時用不同的 Skill
- 研究員跑 `/deep-research`
- 商業分析跑 `/market-analysis`
- 簡報負責人跑 `/pitch-deck-guide`
- 最後集合用 `/pitch-simulation` 做整合評估

### Claude Code 常用操作

| 操作 | 指令 |
|------|------|
| 查看所有可用指令 | 輸入 `/` |
| 讀取檔案 | 直接說「讀取 XXX 檔案」 |
| 儲存產出 | 直接說「存到 XXX.md」 |
| 搜尋網路 | Claude 會自動搜尋相關資料 |
| 切換快速模式 | `/fast` |

---

## Pitch Deck Template / 投影片模板

`templates/pitch-deck-outline.md` 提供可直接填寫的 8 頁大綱模板。

---

## Scoring Criteria / 評分標準

| # | 項目 | 0 分 | 1 分 | 2 分 |
|---|------|------|------|------|
| 1 | Problem Definition & Solution Framing | 定義不清楚 | 有定義但框架不夠好 | 定義清楚、有衡量、框架有效 |
| 2 | Value Proposition & Innovation | 不具創新或不清楚 | 有創新但價值主張薄弱 | 創新解方 + 獨特價值主張 |
| 3 | Opportunity | 無清楚市場 | 有辨識但未驗證 | 市場定義清楚 + 需求證據 |
| 4 | Competitive Landscape | 不了解競爭 | 有競爭意識但差異化有限 | 清楚競爭 + 強定位差異化 |
| 5 | Business Model | 無可行模式 | 有模式但缺細節 | 清晰可行可擴展 |
| 6 | GTM Strategy | 無計畫 | 有輪廓但缺深度 | 清晰可執行對應策略 |
| 7 | Ask | 無需求 | 理解不夠具體 | 資金+里程碑+條款令人信服 |
| 8 | Team | 無專業或角色不清 | 技能角色部分吻合 | 技能互補角色清楚 |
| 9 | Presentation | 混亂不清 | 大致清楚有缺口 | 清晰自信令人信服 |
| 10 | Q&A | 無法有效回答 | 部分模糊不一致 | 回應令人信服 |
| | **總分** | | | **/20** |

---

## About HSIL Hackathon / 關於比賽

- **主辦**: Harvard T.H. Chan School of Public Health — Health Systems Innovation Lab
- **共同主辦**: 台大公衛學院 Health Economics & AI Lab
- **日期**: 2026/4/10-11
- **地點**: 國立臺灣大學公共衛生學院
- **主題**: 運用 AI 打造高價值醫療體系 (Building High-Value Health Systems: Leveraging AI)
- **官網**: https://hsilhackathontaiwan.com/

---

## Requirements / 需求

- [Claude Code](https://claude.ai/code) — CLI、Desktop App、VS Code 或 JetBrains 皆可
- 不需要額外安裝任何套件，**clone 即可使用**

## Optional MCP Servers / 選裝 MCP 伺服器

以下 MCP servers 可進一步強化研究能力（非必要）：

| MCP Server | 用途 | 安裝 |
|-----------|------|------|
| Healthcare MCP | FDA、WHO、PubMed、臨床試驗、ICD-10 | [GitHub](https://github.com/Cicatriiz/healthcare-mcp-public) |
| PubMed MCP | 醫學文獻搜尋與摘要 | `npm: @cyanheads/pubmed-mcp-server` |
| Gamma MCP | AI 簡報生成 | Claude.ai 內建，需認證 |
| Mermaid MCP | 流程圖、架構圖生成 | [GitHub](https://github.com/hustcc/mcp-mermaid) |
| AntV Chart MCP | 25+ 種圖表生成 | [GitHub](https://github.com/antvis/mcp-server-chart) |

---

## Author / 作者

**簡承哲 (Cheng-Che Chien)** — 專案經理
聯合通科技 Cloud Communication Technology Ltd.

本工具包在 Claude (Anthropic) 的協助下開發，旨在透過 AI 賦能提升 HSIL Hackathon 所有參賽團隊的 Pitch 品質與創新能力。

---

## License / 授權

本作品採用 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0) 授權。

你可以自由地使用、修改、分發本工具包，唯須：
- 保留原始版權聲明與授權條款
- 標示修改之處

本工具包以「AS IS」提供，不附帶任何明示或暗示的擔保。
詳見 [LICENSE](./LICENSE) 與 [NOTICE](./NOTICE) 檔案。

## Acknowledgments / 致謝

### 公共領域方法論
本工具包使用的商業與設計框架（Porter's Five Forces、SWOT、Business Model Canvas、Design Thinking、TAM/SAM/SOM 等）為廣泛使用的公共知識。

### 推薦的外部開源工具
| 工具 | 授權 | 作者 |
|------|------|------|
| [Healthcare MCP](https://github.com/Cicatriiz/healthcare-mcp-public) | MIT | Forrest Babola |
| [PubMed MCP](https://github.com/cyanheads/pubmed-mcp-server) | Apache 2.0 | cyanheads |
| [Mermaid MCP](https://github.com/hustcc/mcp-mermaid) | MIT | hustcc |
| [AntV Chart MCP](https://github.com/antvis/mcp-server-chart) | MIT | Ant Group / AntV |

### 評分標準
評分標準內容引用自 [HSIL Hackathon 2026 官方網站](https://hsilhackathontaiwan.com/)，
主辦單位為 Harvard T.H. Chan School of Public Health — Health Systems Innovation Lab。

---

## Contributing / 貢獻

歡迎提交 PR 改善 Skills 內容！特別歡迎：
- 新增更多健康議題的研究模板
- 改善評審模擬的真實度
- 新增其他語言支援
- 分享你的使用經驗與建議
