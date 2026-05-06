---
marp: true
theme: default
paginate: true
size: 16:9
style: |
  section {
    justify-content: center;
  }
  code {
    background: #f4f4f4;
  }
filename: 08-supplementary-brand-yaml.md
title: 品牌 YAML：從視覺基因到商業靈魂
date: 2026-04-16
tags:
  - marp
  - lecture
  - startup
  - yaml
description: 將 Logo 提示詞擴展為完整的品牌視覺與溝通規範。
status: active
type: lecture
project: 114-2-資傳人才新創育成
area: SHU
week: 8
created: 2026-04-14T22:45:00
updated: 2026-04-14T22:45:00
---

## 擴展：從 Logo YAML 到品牌 YAML

之前的 YAML 僅定義了圖形特徵。完整的 **「品牌 YAML」** 則涵蓋了視覺、溝通調性與商業核心，確保 AI 在產出網頁與展示影片時，風格不會跑調。

### 品牌 YAML 結構範例

```yaml
Brand_Identity:
  Name: "品牌名稱"
  Core_Value: "品牌核心價值（解決什麼痛點）"
  Slogan: "一句話廣告語"
  Target_Audience: ["目標客群 1", "目標客群 2"]

Visual_System:
  Style: "例如：Minimalist, Tech-futuristic" # 視覺總體風格
  Color_Palette:
    Primary: "#HEX色碼"               # 品牌主色
    Secondary: ["#輔助色1", "#2"]     # 輔助色清單
  Typography:
    Heading: "標題字體建議"
    Body: "內文字體建議"

Content_Vibe:
  Tone: ["Professional", "Friendly"]  # 文案與溝通語氣
  Keywords: ["關鍵字 A", "關鍵字 B"]    # 常用關鍵字

Constraints:
  Negative_Prompt: "絕對不要出現的元素" # 排除條件
```

---

## 如何運用品牌 YAML？

這份結構化的YAML，可使用：

1. **展示影片 (Pitch Video)**：
   將 `Content_Vibe` 與 `Visual_System` 餵給影片 AI，確保背景音樂、畫面剪輯節奏與品牌色調一致。
2. **網頁介面 (Stitch / UI)**：
   將 `Color_Palette` 與 `Typography` 設定直接套入 Google Stitch 的風格編輯器，實現自動化視覺對齊。
3. **商業提案 (Pitch Deck)**：
   利用 `Core_Value` 與 `Target_Audience` 驅動 Gemini 生成簡報大綱，確保邏輯與行銷訴求不脫節。

---

## 課堂練習：更新你的品牌基因

請各團隊根據目前的專案進度，將原本簡單的 Logo 規範擴展為完整的「品牌 YAML」。

**檢查清單：**
- [ ] **色碼精確度**：主色與輔助色的 HEX 碼是否已定稿？
- [ ] **客群定義**：是否能精簡出 2 個核心受眾標籤？
- [ ] **語氣設定**：這會決定下週 Pitch 簡報與今日影片的文案風格。

**請將更新後的 YAML 代碼儲存在你們的專案筆記（如 Obsidian）中，後續產出將以此為準。**