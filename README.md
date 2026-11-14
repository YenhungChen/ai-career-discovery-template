# 🧭 AI 職涯探索與雙 AI 協作筆記庫範本

這是一套專為**「還不確定職涯方向、想規劃個人作品集、並系統化產出高品質履歷」**所設計的 Markdown 結構化工作流範本。

透過預先定義好的系統指令（`CLAUDE.md` 與 `AGENTS.md`），讓 AI 從「直接說教的機器人」轉變為**「先深度提問、再逐步收斂」的一對一職涯探索教練**，搭配另一組 AI 進行**「毒舌招募主管審視」與「系統架構繪圖」**，協助你從零打造專屬的職涯藍圖。

---

## ✨ 核心設計理念

1. **先問再給建議，拒絕空泛說教**：透過嚴格的 Prompt 規則，強制 AI 每次只問 1～2 個具體的生活化問題，逐步挖掘你的能量來源、隱性優勢與核心價值觀。
2. **漏斗式三階段推進**：遵循「`01` 自我探索收斂 ➔ `02` 迷你作品驗證 ➔ `03` STAR 履歷轉化」的清晰里程碑，解決「不知道該寫什麼」的焦慮。
3. **低成本試錯與反悔機制**：內建「踩雷封存」規範，若在製作作品階段發現不適合，可一鍵封存舊路線並將經驗轉化為「排除清單」，讓下一次收斂更精準。
4. **雙 AI 角色分工協作**：
   * **Claude Code（主導教練）**：負責一對一引導訪談、優勢提煉與筆記整理。
   * **Codex CLI（審視與繪圖助教）**：負責扮演挑剔的技術招募主管進行文件 Review、資安去識別化檢查，以及生成 Mermaid 系統架構圖。

---

## 📁 資料夾結構說明

```text
ai-career-discovery-template/
├── CLAUDE.md               # 主教練規則（Claude Code 原生支援，其他工具可複製內容使用）
├── AGENTS.md               # OpenAI Codex CLI 自動讀取的審視與繪圖助教規則
├── 01_Discovery_Log.md     # [階段一] 能量盤點、核心優勢、目標方向與排除清單
├── 02_Portfolio_Ideas.md   # [階段二] 獨立作品企劃、技術資產包裝與架構圖
└── 03_Resume_Draft.md      # [階段三] 履歷草稿與 STAR 經歷量化轉化
```

---

## 🚀 快速開始指南（3 步驟）

### 1. 建立你的「私人」筆記庫（⚠️ 極重要）
點擊本頁面右上角的綠色按鈕 **`Use this template`** ➔ **`Create a new repository`**。
> **隱私安全提醒**：因為後續你會在筆記中寫入個人經歷、優勢弱點與履歷草稿，建立新倉庫時**務必將權限設為 `Private`（私人）**！

### 2. 下載到本地電腦並開啟 AI 工具
將你剛建立的私人倉庫 Clone 到本地電腦（建議與工作專案分開存放）：

```bash
git clone git@github.com:你的帳號/你的私人倉庫名稱.git
cd 你的私人倉庫名稱
```

接著使用 **Claude Code（CLI 或 Desktop 桌面版）** 開啟這個資料夾（它會自動讀取根目錄的 `CLAUDE.md`）。

### 3. 啟動第一場職涯探索對話
在 Claude Code 對話框中直接輸入：
> **「嗨，請讀取 `CLAUDE.md` 的角色設定與規範，我們現在開始第一階段的職涯探索吧！」**

---

## 🔄 使用其他 AI 工具？（跨平台轉移對照表）

如果你沒有使用 Claude Code，依然可以完整套用這套範本，只需將 `CLAUDE.md` 的內容複製到你使用的 AI 工具對應規則檔即可：

| 使用的 AI 工具 | 對應的規則檔位置與名稱 | 如何啟動 |
| :--- | :--- | :--- |
| **Claude Code** (CLI / Desktop) | 根目錄 `CLAUDE.md` | **原生支援**，開啟資料夾自動讀取。 |
| **OpenAI Codex CLI** | 根目錄 `AGENTS.md` | **原生支援**，開啟資料夾自動讀取。 |
| **Cursor** | 根目錄 `.cursorrules` | 將 `CLAUDE.md` 內容複製貼上到 `.cursorrules` 即可。 |
| **Windsurf** | 根目錄 `.windsurfrules` | 將 `CLAUDE.md` 內容複製貼上到 `.windsurfrules` 即可。 |
| **GitHub Copilot (VS Code)** | `.github/copilot-instructions.md` | 建立 `.github` 資料夾並將 `CLAUDE.md` 內容貼入該檔。 |
| **Gemini CLI / Code Assist** | 根目錄 `GEMINI.md` | 將 `CLAUDE.md` 內容複製貼上到 `GEMINI.md` 即可。 |
| **網頁版 ChatGPT / Claude / Gemini** | 不需要特定檔名 | 開啟新對話（或建立 Project / Gem），直接**上傳或貼上 `CLAUDE.md` 的純文字內容**即可啟動。 |
