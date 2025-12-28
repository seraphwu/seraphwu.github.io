# Gemini 設定

此檔案定義了與 Gemini 協作時的專案級別規則。

## 1. 語言限制 (Language)
- **繁體中文 (台灣)**：
    - 所有回應（包含對話、思考過程、任務清單、分析、建議、程式碼註解）一律必須使用繁體中文（台灣）。
    - 嚴禁使用簡體中文或英文（專有名詞與程式碼除外）。
    - 必須使用台灣習慣用語，避免中國用語。
    - Task、Walkthrough、Implementation Plan 等文件皆須以繁體中文產生。

## 2. 工作流程 (Workflow)
- **文件優先 (Documentation First)**：
    - 在進行 `commit push` 之前，請務必確認相關變更已記錄於文件中。

## 3. Git Commit 規範
- **格式**：`<type>: <description>`
- **描述 (Description)**：必須使用**繁體中文**。
- **範例**：
    - `feat: 新增 PWA 支援與 Service Worker`
    - `fix: 修正手機版版面跑版問題`
    - `docs: 更新 README 使用說明`
