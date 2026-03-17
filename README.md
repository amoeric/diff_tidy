# DiffTidy

  Git diff 視覺化分析工具，搭配 AI 自動產生功能摘要與 Code Review。

  ## 功能特色

  - **Diff 瀏覽** — 選擇分支或指定 commit 點，查看檔案變更的詳細差異
  - **AI 摘要分析** — AI 自動分析所有變更，產生結構化功能清單
  - **Code Review** — AI 檢查程式碼品質、潛在問題與改進建議，支援一鍵修正
  - **收藏管理** — 收藏重要的分析項目與討論，支援批次匯出為 JSON / Markdown
  - **Prompt 模板** — 自訂分析 prompt，按專案綁定不同模板
  - **多模型比較** — 並行比較不同 AI 模型的分析結果
  - **自動更新** — 有新版本時自動通知，一鍵更新

  ---

  ## 安裝

  ### 1. 下載

  前往 [Releases](https://github.com/amoeric/diff_tidy/releases/latest)
  頁面，下載最新版本的 `.dmg` 安裝檔。

  ### 2. 安裝

  開啟下載的 `.dmg` 檔案，將 DiffTidy 拖入「應用程式」資料夾。

  ### 3. 首次開啟（重要）

  > DiffTidy 尚未經過 Apple 公證（notarization），macOS
  會顯示「已損毀，無法打開」的警告。
  > 這是正常現象，請依照以下步驟解除限制。

  開啟終端機，執行以下指令：

```bash
xattr -cr /Applications/DiffTidy.app
```
  執行完畢後即可正常開啟 DiffTidy，之後不需要再重複此步驟。

  ---
  系統需求

  - macOS 12.0 (Monterey) 或更新版本
  - Apple Silicon (M1/M2/M3/M4) 或 Intel Mac

  ---
  AI 設定

  DiffTidy 支援兩種 AI 來源：

  - Anthropic API — 透過 API Key 呼叫 Claude，需要 https://console.anthropic.com/
  - Claude CLI — 使用本機安裝的 claude 指令，需要先安裝
  https://docs.anthropic.com/en/docs/claude-code

  首次啟動時會引導你選擇 AI 來源並完成設定。

  ---
  授權

  DiffTidy 為私有軟體，僅提供編譯後的安裝檔供下載使用。
