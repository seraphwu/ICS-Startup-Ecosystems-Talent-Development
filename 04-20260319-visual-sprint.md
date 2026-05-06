---
marp: true
theme: default
paginate: true
size: 16:9
style: |
  section {
    justify-content: center;
  }
  table {
    font-size: 0.9em;
    width: 100%;
  }
  .highlight {
    color: #b30000;
    font-weight: bold;
  }
filename: 04-20260319-visual-sprint-v3.md
title: 04-視覺衝刺：AI Logo 與品牌規範
date: 2026-03-19
tags:
  - marp
  - lecture
  - startup
  - week04
  - branding
description: 第四週簡報，帶領學生從品牌名稱出發，使用 AI 生成 Logo 並建立品牌視覺規範。
status: active
type: lecture
project: 114-2-資傳人才新創育成
area: SHU
week: 4
updated: 2026-03-19T01:59:00
version: v3
---

![bg left:45%](https://images.unsplash.com/photo-1618005182384-a83a8bd57fbe?q=80&w=1600&auto=format&fit=crop)

# 114-2 資傳人才新創育成

## Week 04: Visual Sprint 視覺衝刺

**授課教師**：林展
**日期**：2026 / 03 / 19

---

## 課前回顧

上週我們確立了品牌 DNA：
絕大多數團隊已經擁有明確的市場定位、黃金圈，以及決選的品牌名稱。

**【上週缺席團隊】**
接下來 15 分鐘內，使用 AI 輸入你們的產品核心理念，決定出 1 個。沒有名字，今天無法進行視覺化。

其他團隊，我們準備開始進行 Brand Guideline。

---

![bg right:40%](https://images.unsplash.com/photo-1586717791821-3f44a563fa4c?q=80&w=1600&auto=format&fit=crop)

## 本週：<br>Brand Guideline (品牌規範) onepage 版

為什麼新創公司需要 Guideline？
確保未來無論是誰負責發文、架設網站或製作簡報，對外呈現的視覺風格都高度一致。

一份最基礎的商業 Guideline 必須包含：

- **Logo (標誌)**：主視覺圖形。
- **Color Palette (色彩計畫)**：主色與輔助色 (精確的 HEX 色碼)。
- **Typography (字體規範)**：標題與內文的指定字體。

---

## Step 1: AI Logo 提示詞實戰 (Prompting) 1/2

我們不從草稿開始畫，直接讓 AI 提案。

**Midjourney / Recraft ver.**
請打開 Midjourney 或 Recraft。
將 Brand DNA 轉化為 prompt ：

- **基礎 Prompt 結構：**
  `[產業/產品類型] logo, minimalist, flat vector design, [代表品牌靈魂的 1-2 個關鍵字], [1-2 個主要顏色], white background, clean lines, corporate style --no text, realistic shadows, complex details`
- **範例：**`Coffee shop logo, minimalist, flat vector design, energetic, orange and navy blue, white background, clean lines, corporate style --no text`

---

## Step 1: AI Logo 提示詞實戰 (Prompting) 2/2

**Gemini / Copilot / Canva / Ideogram**
請打開 Gemini、Bing Image Creator (Copilot) 或 Canva 內建 AI。
將你的 Brand DNA 轉化為 prompt：

- `[產業/產品類型] logo, minimalist, flat vector design, [代表品牌靈魂的 1-2 個關鍵字], [1-2 個主要顏色], white background, clean lines, corporate style, DO NOT include any text or realistic shadows.`
- **範例：**`Coffee shop logo, minimalist, flat vector design, energetic, orange and navy blue, white background, clean lines, corporate style, DO NOT include any text.`

_(註：若使用 Bing 或 Canva，請將結尾的 --no text... 參數改為自然語言描述，如：do not include any text or realistic shadows)_

---

## 結構化提示詞 (YAML Prompting)

除了白話文，你們也可以嘗試 YAML 格式：

```yaml
Brand_Context:
  Industry: "[你的產業/產品類型]"
  Vibe: ["形容詞 1", "形容詞 2"]
Visual_Requirements:
  Style: "Flat vector design, minimalist, corporate"
  Colors: "[1-2 個主要顏色]"
Negative_Prompt: "NO text, NO letters, NO 3D effects"
```

**「請讀取上方 YAML 設定，嚴格遵守視覺與排除限制，為我生成 4 款 Logo 圖像。」**

---

## 取得 YAML 敘述範本

如果「抽卡」抽到滿意的 Logo，但不知道該如何維持風格？請叫 AI 幫你寫出它的 YAML 規範。

**操作步驟：**
1. **上傳圖片**：將你最滿意的 Logo 圖片丟回 Gemini / ChatGPT / Claude。
2. **下達指令**：
   > 「這是我目前最滿意的品牌 Logo。請分析這張圖的視覺特徵，包含產業風格、色彩比例、線條調性與整體 Vibe，並幫我轉化為一份標準的 **YAML 格式 Prompt**，方便我之後用這份設定生成更多風格統一的輔助圖形。」
---

**進階:**
這是我目前最滿意的品牌 Logo。請分析這張圖的視覺特徵，並嚴格按照以下 YAML 結構輸出，不要新增或刪除任何欄位：
```YAML
Brand_Context:
  Industry: ""        # 判斷最可能的產業類型
  Vibe: []            # 3-5 個精準形容詞

Visual_Requirements:
  Style: ""           # 設計風格（如 flat vector / minimalist 等）
  Shape_Language: ""  # 線條調性（如 geometric / organic / sharp）
  Colors:
    Primary: ""       # 主色 HEX
    Secondary: []     # 輔助色 HEX（1-2 個）
  Composition: ""     # 構圖特徵（如 icon-only / icon+wordmark）

Negative_Prompt: []   # 根據此 Logo 風格，列出應排除的視覺元素
```

請只輸出 YAML，不需要任何說明文字。

---

## 補充：什麼是 YAML 格式？

YAML 是一種結構化的資料編寫方式，原本是工程師寫設定檔的語言，現在則是**控制 AI 產出的方式之一**。

**為什麼不用白話文(自然語言)就好？**
寫了一長串白話文許願**抽卡**，容易漏看關鍵字或隨機發散。YAML 強迫我們用「填表」的邏輯，把需求拆解成精準的條件，能大幅降低 AI 的幻覺！

---

**YAML 基礎語法規則：**

1. **鍵值對應 (Key-Value)**：使用冒號與空格分隔。例如 `Style: "Minimalist"` (注意：冒號後必定要**空一格**)。
2. **層級關係 (縮排)**：用 2 個**空白鍵**縮排來表示從屬關係（⚠️ 絕對不要按 Tab 鍵）。
3. **清單項目 (陣列/列表)**：當一個屬性有多個值時，有兩種常見寫法：
   - **寫法一（減號換行）**：使用 `- ` 換行條列。例如：(注意縮排一致)
     ```yaml
     Vibe:
       - "Professional"
       - "Clean"
     ```
   - **寫法二（中括號單行）**：直接用 `[值1, 值2]` 寫在同一行。例如：
     ```yaml
     Vibe: ["Professional", "Clean"]
     ```

---

![bg right:40%](https://images.unsplash.com/photo-1542744173-8e7e53415bb0?q=80&w=1600&auto=format&fit=crop)

## Step 2: 決策 (Decision)

AI 會產出大量選項，放下個人主觀美感，用商業眼光進行篩選：

- **縮小測試**：將圖片縮小到名片或 APP Icon 的尺寸，圖形是否依然清晰可辨？(如遇到印刷要最小指定高度 x mm)
- **定位吻合度**：符合你們上週設定的「高價/平價」或「專業/親民」定位嗎？
- **可註冊性**：是否過於複雜，或與現有知名品牌高度雷同？

**任務：各團隊收斂至唯一 1 個決選 Logo。**

---

## Step 3: 萃取色彩與字體

選定 Logo 後，請從中提取視覺規範：

- **色彩 (Color)**：使用[線上選色工具](#color-pickers)，從 Logo 中吸取出 1 個主色與 1-2 個輔助色。必須記錄精確的 HEX 色碼 (例如：#FF5733)。
- **字體 (Typography)**：為品牌挑選無版權爭議的商用中/英文字體。
  - **標題字**：具備個性、適合用於 Logo 標準字或海報標題 (如：展示型字體、粗黑體)。
  - **內文字**：清晰、好讀、適合長篇閱讀 (如：標準黑體)。

_數位影像設計/數位圖像製作實務 課程字體包日後整理打包提供_

---

<span id="color-pickers"></span>

## 線上選色工具推薦 (Color Pickers)

要從 AI 生成的 Logo 中精準萃取 HEX 色碼，推薦使用以下三款免費工具：

1. **Canva 內建吸色 (無縫接軌)**
   - **優勢**：等一下排版就要用 Canva。
   - **作法**：Canva 應該不用我教。
2. **Coolors (新創團隊最愛) - 極度推薦**
   - **網址**：[coolors.co/image-picker](https://coolors.co/image-picker)
   - **優勢**：介面極度現代流暢。上傳圖片後能快速點選吸色，並且能將色票匯出成一張非常漂亮的圖片，直接貼進 Brand Guideline 裡。
3. **Adobe Color (業界標準)**
   - **網址**：[color.adobe.com](https://color.adobe.com/)
   - **優勢**：點擊「從影像擷取 (Extract Theme)」標籤頁，上傳 Logo，它會自動為你抓取 5 個完美搭配的主/輔助色，還能切換不同氛圍（亮色、柔和、深色等）。

---

![bg right:40%](https://images.unsplash.com/photo-1522202176988-66273c2fd55f?q=80&w=1600&auto=format&fit=crop)

## 課堂 Workshop：產出品牌一頁書

**時間限制：60 分鐘**
請各團隊使用 Canva、Figma 或任何排版軟體，將今天的戰果排版成一張 A4 大小的「Brand Guideline (品牌規範一頁書)」。
版面上必須具備：

1. 最終決定的品牌名稱與 Slogan。
2. 決選的 Logo 圖形。
3. Color Palette (色塊與 HEX 色碼標示)。
4. Typography (標題與內文的字體名稱及範例句)。

~~(下課前，各組將進行 1 分鐘極速 Pitch 展示視覺成果)~~

---

## 下週預告 (Next Week Preview)：一頁式網站實戰

今天完成了品牌視覺規範，你們的品牌已經具備了專業的外觀。
下週的課堂上，我們將會直接運用今天的成果，帶大家快速架設第一個 **「一頁式網站 (Landing Page)」**。

**下週課堂實作預告 (無須課前作業，我們課堂上搞定)：**

1. **吸睛文案撰寫**：提煉一句話，讓進站的人秒懂你們賣什麼。
2. **痛點與解法對接**：列出目標客群的痛點，以及產品帶來的改變。
3. **行動呼籲 (CTA)**：設計引導使用者留名單或購買的按鈕。

⚠️ **請各團隊務必妥善保存今天的「Brand Guideline 圖檔」與「HEX 色碼」，下週架站馬上就會用到！**
