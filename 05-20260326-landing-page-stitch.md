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
filename: 05-20260326-landing-page-stitch.md
title: 05-實戰衝刺：使用 Google Stitch 打造高擬真 Landing Page
date: 2026-03-26
tags:
  - marp
  - lecture
  - startup
  - week05
  - google-stitch
description: 第五週簡報，導入 Google Labs 的最新工具 Stitch，帶領學生從 Vibe Design 進入高擬真 UI 設計。
status: active
type: lecture
project: 114-2-資傳人才新創育成
area: SHU
week: 5
created: 2026-04-14T17:29:00
updated: 2026-04-14T17:32:00
---

![bg left:45%](https://images.unsplash.com/photo-1558655146-d09347e92766?q=80&w=1600&auto=format&fit=crop)

# 114-2 資傳人才新創育成
## Week 05: Google Stitch 視覺縫合實戰
**授課教師**：林展
**日期**：2026 / 03 / 26

---

## 為什麼這週我們要用 Google Stitch？

在上週，我們有了品牌靈魂 (DNA) 與 Logo。
今天我們不只是「填模板」，而是要利用 **Google Stitch** 進行 **「Vibe Design (氛圍設計)」**。

**Stitch 的強大之處：**
1. **AI 原生畫布**：不需從空白開始，直接用自然語言描述目標。
2. **高擬真 (High-Fidelity)**：產出的不只是草圖，而是接近完成品的 UI。
3. **設計即程式碼**：支持匯出到 Figma 或生成前端程式碼。

---

## Step 1: 從 Vibe 開始 (用 YAML 驅動 Stitch)

Stitch 支援從「業務目標」與「感受」出發。
請將上週練習的 YAML 結構稍微進化，直接貼入 Stitch 的 Prompt 框：

```YAML
**請以此設定為基礎，為我生成一個具備視覺張力的 Landing Page 佈局**
```


```yaml
Project: "Landing Page for [Brand Name]"
Target: "Web / Desktop"
Vibe_Design:
  Feel: ["Professional", "Trustworthy", "Minimalist"]
  Objective: "Convert visitors into pre-order subscribers"
UI_Components:
  - Hero section with large headline
  - 3 Feature cards with icons
  - Social proof testimonial block
Brand_Assets: "Use [Primary Color] as main accent"
```
👉 **「請以此設定為基礎，為我生成一個具備視覺張力的 Landing Page 佈局。」**

---

## Step 2: 迭代與分支 (Iteration & Branching)

Stitch 最具特色的功能是 **「分支探索」**：

1. **Experimental Mode**：建議開啟實驗模式 (Gemini 3 Pro)，獲得更細緻的間距與視覺層次。
2. **多向探索**：不滿意某個區塊？點擊該畫面並下指令：「讓這個 Hero Section 看起來更具有未來感」，Stitch 會為你生成新的變體版本，而不會覆蓋原本的設計。
3. **圖片整合**：直接上傳上週生成的 Logo，Stitch 會嘗試將其整合進 UI 佈局中。

---

![bg right:40%](https://images.unsplash.com/photo-1581291518633-83b4ebd1d83e?q=80&w=1600&auto=format&fit=crop)

## Step 3: 從設計到轉換

選定最滿意的版本後，我們要進行「數位落地」：

1. **文字精修**：在畫布上直接修改 AI 生成的預留文字，換成你們最具說服力的 Slogan。
2. **色彩校正**：確保背景、按鈕顏色完全符合你們的 **Brand Guideline**。
3. **輸出準備**：
   * 點擊 **"Export Code"** 查看前端實作方式。
   * 或 **"Paste to Figma"** 進行更細緻的互動設計。

---

## 課堂 Workshop：品牌實體化

**時間限制：90 分鐘**

請各團隊在 **[stitch.withgoogle.com](https://stitch.withgoogle.com/)** 上完成：
* [ ] 一份具備完整視覺流動感的一頁式 UI。
* [ ] 包含至少 3 個主要轉換區塊 (Hero, Features, CTA)。
* [ ] 將設計好的 Canvas 連結或截圖分享至課程平台。

~~(下課前，各組將進行 1 分鐘極速 Pitch 展示視覺成果)~~
**今天不 Pitch，請在 Stitch 畫布上留下你們的設計思維註解。**

---

## 下週預告：市場驗證與數據分析

今天我們完成了「產品的臉面」。
下週我們將探討如何讓這個設計變成真實的流量入口。
* 如果這是 HTML/CSS，我們要如何部署？
* 如何測試哪一種設計「轉換率」更高？

⚠️ **請各團隊務必在 Stitch 中「命名」你們的 Project，以免進度流失！**