---
filename: 08-Spec-Brand-Guideline-Mapping.md
title: 品牌指南結構與 YAML 對照表 (Brand Guideline & YAML Mapping)
course: ICS Startup Ecosystems & Talent Development
week: 8
date: 2026-04-16
status: active
created: 2026-04-14T22:50:00
updated: 2026-04-14T22:55:00
---

# 品牌指南與品牌 YAML 結構對照表

本文件為協助 **ICS (資訊傳播學系)** 的學生，將設計概念轉化為結構性內容。
將品牌指南(Brand Guideline)的項目對應到 YAML 格式結構所整理。

---

## 1. 品牌核心 (Brand Identity / DNA)
定義品牌的核心與市場定位，為 `Brand_Identity` 的資料來源。

* **核心價值 (Core Values)** [YAML: `Core_Value`]：品牌解決問題的核心能力與堅持。
* **品牌標語 (Slogan / Tagline)** [YAML: `Slogan`]：具備記憶點的一句話廣告語。
* **目標受眾 (Target Audience)** [YAML: `Target_Audience`]：核心使用者畫像，決定行銷訴求。
* **品牌使命與願景 (Mission & Vision)**：品牌存在的長期目標。

---

## 2. 視覺系統 (Visual System)
定義外觀規格，為 `Visual_System` 的核心。

* **視覺風格 (Visual Style)** [YAML: `Style`]：整體的視覺調性（如：極簡、科技感、復古）。
* **色彩計畫 (Color Palette)** [YAML: `Color_Palette`]：
    * **主色 (Primary Color)** [YAML: `Primary`]：品牌最核心的 HEX 色碼。
    * **輔助色 (Secondary / Accent Colors)** [YAML: `Secondary`]：用於強調或按鈕的對比色。
* **標準字體 (Typography)** [YAML: `Typography`]：
    * **標題 (Heading)**：展示層級的字體。
    * **內文 (Body)**：具備易讀性的字體。

---

## 3. 溝通與語調 (Communication & Tone)
決定 AI 生成文案與影片時的性格，對應 YAML 的 `Content_Vibe`。

* **品牌氛圍 (Vibe)** [YAML: `Vibe`]：品牌帶給人的第一感官印象（如：專業、熱情、冷靜）。
* **語調 (Tone of Voice)** [YAML: `Tone`]：溝通時的語氣設定。
* **關鍵字 (Keywords)** [YAML: `Keywords`]：品牌溝通中頻繁出現的詞彙。
* **負面排除 (Negative Constraints)** [YAML: `Negative_Prompt`]：絕對禁止出現的視覺元素或用語。

---

## 4. 應用展示與素材 (Applications & Assets)
品牌在真實場景中的具體呈現，對應衝刺週的產出。

* **情境展示圖 (Mockups)**：產品在手機、筆電或實際場景中的樣貌。
* **展示影片 (Pitch Video)**：30 秒的產品核心價值動態呈現。
* **數位門面 (Landing Page)**：利用 Google Stitch 等工具產出的高保真介面。

---

## 品牌 YAML 轉換範例 (Code Snippet)

學生可將上述指南內容，精簡為以下 YAML 格式以供 AI 調用：

```yaml
Brand_Identity:
  Name: "專案名稱"
  Core_Value: "Core Values"
  Slogan: "Slogan / Tagline"
  Target_Audience: ["Audience A", "Audience B"]

Visual_System:
  Style: "Visual Style"
  Color_Palette:
    Primary: "#HEX"
    Secondary: ["#HEX1", "#HEX2"]
  Typography: "Typography Settings"

Content_Vibe:
  Vibe: ["Keyword 1", "Keyword 2"]
  Tone: "Tone of Voice"
  Negative_Prompt: "Negative Constraints"
```

---
**授課教師**：林展 (Lin Chan)
**課程單位**：世新大學 資訊傳播學系 (ICS)