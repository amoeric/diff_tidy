# Changelog

## [0.3.0] - 2026-03-19

### Features

- 多專案工作區：支援同時開啟多個 Git 倉庫，透過頁籤切換
- 專案頁籤拖曳排序
- Per-project 設定覆寫（預設目標分支、忽略路徑）
- 多主題系統與 Light/Dark/System 色彩模式切換

### Improvements

- 自訂 overlay title bar，專案頁籤置於視窗最上方

### Bug Fixes

- 切換專案時跳過已載入的 diff，大幅提升切換速度

## [0.2.0] - 2026-03-18

### Features

- 分支選擇器新增重新載入按鈕

### Bug Fixes

- CLI runner PATH 注入 + cwd 隔離，解決 `env: node: No such file or directory` 錯誤
- CLI runner 搜尋已知路徑（nvm、fnm、Volta、Homebrew）解析指令位置，解決 app 找不到 claude
- 子程序工作目錄設為 `/tmp`，防止 macOS TCC 彈出不必要的權限請求（下載項目、文件、桌面、Music 等）
- 討論模式預設不隱藏內容，改為手動切換顯示/隱藏

## [0.1.0] - 2026-03-17

### Features

- AI 驅動的分支 diff 檢視器，支援摘要、Code Review、多模型比較
- 支援 Anthropic API 與 Claude CLI 兩種 AI 提供者
- 互動式摘要 — Markdown 渲染、AI 討論、收藏功能
- Code Review 一鍵修正 + Fix Preview 差異預覽
- Prompt 模板管理 — 自訂分析 prompt，按專案綁定
- 分析結果匯出 JSON/Markdown，收藏頁批次匯出
- 分支選擇器支援 commit hash — combobox + commit 歷史 + 分頁載入
- 分析結果快取，切換分支時自動恢復
- 獨立收藏頁面，搜尋與排序
- 快捷鍵支援（Cmd+Enter 送出討論等）
- 操作導覽、變更紀錄視窗
- Tauri Updater 自動更新
- GitHub 風格水平 tab layout
- Claude.ai 暖色調配色風格
