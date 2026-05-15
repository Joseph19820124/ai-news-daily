# 每日 AI 新聞 (AI Daily)

> 每日精選 AI 與 Agent 生態最新動態，卡片式排版。每天早上自動更新。

## 線上版本

https://joseph19820124.github.io/ai-news-daily/

## 資料來源

資料來自 [x.deepsrt.cc/index.txt](https://x.deepsrt.cc/index.txt)，每日精選兩個區塊：

- 🤖 **AI 與大模型** — 模型發布、API、訂閱動態
- 🛠️ **開發工具與 Agent 生態** — Agent 工具、IDE、開源框架

## 運作機制

- `index.html` 是純前端網頁，從同源的 `data.txt` 讀取資料並渲染成卡片
- `data.txt` 由一個排程任務每天早上自動拉取最新內容並 commit 到本 repo
- 每張卡片末尾連結到原推文（X / Twitter）

## 技術細節

- 完全 static — 沒有後端、沒有資料庫
- 同源 fetch — 不會踩 CORS
- 升級路徑：若 `data.txt` 載入失敗，前端會 fallback 嘗試直接 fetch 上游

---

Built with Claude.
