---
filename: 11-supplement-PROJECT-STRUCTURE.md
title: 專案筆記與資料夾結構總覽 (Workspace Structure Guide)
course: ICS Startup Ecosystems & Talent Development
week: 11
date: 2026-05-07
status: active
version: 1
project: 114-2-資傳人才新創育成
area: SHU
created: 2026-05-06T20:58:00
updated: 2026-05-06T20:58:00
---

# 專案筆記目錄架構 (Workspace Structure)

這份清單統整了從 Week 01 到 Week 11，各團隊必須在專案協作平台（如 Notion、Obsidian 或 GitHub）中建立並妥善保存的核心資產。這將是期末 Demo Day 與後續申請 SBIR 補助的基石。

---

### 📂 01_商業定位與品牌基因 (Strategy & Brand DNA)
這個資料夾存放專案最核心的商業價值與品牌定位邏輯。
* **📄 PMF_產品商業價值評估表.md** (W02)：記錄目標受眾、核心功能、視覺呈現與溝通語言的現況與目標轉換。
* **📄 品牌命名與黃金圈.md** (W02, W03)：包含備選名稱清單、決選名單、Slogan 以及品牌的 Why、How、What。
* ⭐ **📄 品牌基因_YAML.md** (W08)：驅動所有 AI 工具的核心代碼，涵蓋 `Brand_Identity`（品牌身分）、`Visual_System`（視覺系統）、`Content_Vibe`（溝通語調）與 `Constraints`（排除條件）。
* ⭐ **📄 商業模式_YAML.md** (W08)：`Business_Model` 結構，明列營收來源（Revenue Streams）、價值主張與成本結構。

### 📂 02_視覺規範與數位門面 (Visual & UI)
這個資料夾管理所有對外的設計準則與網頁資產。
* **📄 Brand_Guideline.md** (W04)：包含決選 Logo 圖形、精確的 HEX 色碼，以及中英文字體規範。
* **📄 Landing_Page_數位門面.md** (W05, W08)：包含驅動 Google Stitch 的提示詞設定，以及在 W08 衝刺後產出的高擬真 UI 預覽連結與截圖。

### 📂 03_行銷素材與簡報 (Marketing & Pitch)
這個資料夾準備用於說服投資人或使用者的動態與靜態素材。
* **📄 募資短片腳本與成片.md** (W07, W08)：利用 AI 產出的 30 秒短片腳本（痛點 > 解法 > 未來），以及在 W08 縫合產出的最終產品展示短片檔案。
* **📄 期中_Pitch_Deck.md** (W09)：基於 Guy Kawasaki 10 頁框架所製作的簡報大綱與 PDF 檔案，涵蓋痛點、解法、市場規模、團隊等。

### 📂 04_企業設立與資金計畫 (Company & Funding)
這個資料夾負責將專案轉化為具備法律實體與營運資金的企業。
* **📄 企業行政與資金_YAML.md** (W10)：
  * `Company_Setup`：記錄 3 個不撞名的正式公司預查名稱、營業項目代碼與企業組織型態。
  * `Funding_Strategy`：記錄鎖定的政府補助案與青年創業貸款評估目標。
* **📄 SBIR_計畫書框架_YAML.md** (W10)：涵蓋 `Proposal_Core` (痛點與創新點)、`Technical_Specs` (技術與產出物) 與 `Expected_Outcomes` (預期產值)。

### 📂 05_智財防禦與法律聲明 (IP & Legal)
這個資料夾存放保護數位資產與品牌心血的法務文件。
* **📄 智財保護策略_YAML.md** (W11)：記錄商標的目標類別、檢索系統查核狀態、目前使用的商標符號，以及專利申請潛力。
* **📄 品牌資產與商標管理_YAML.md** (W11)：詳細記錄 Logo 的 AI 工具提示詞與人類實質修改過程，用以主張著作權。
* **📄 COPYRIGHT.md** (W11)：針對專案中純 AI 生成素材的權利歸屬聲明，明確劃分人機協作的免責與版權主張。