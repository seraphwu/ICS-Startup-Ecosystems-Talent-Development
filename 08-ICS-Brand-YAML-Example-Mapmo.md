---
title: ICS 品牌 YAML 標準範例 (Mapmo)
course: ICS Startup Ecosystems & Talent Development
week: 8
date: 2026-04-16
status: active
created: 2026-04-14T22:55:00
updated: 2026-04-14T22:55:00
filename: 08-ICS-Brand-YAML-Example-Mapmo.md
---

# ICS 品牌 YAML 標準範例：Mapmo 專案

這份範例展示了如何將一個地理照片地圖平台（Mapmo）的品牌規範，轉化為結構化的 YAML 代碼。這組代碼可直接供 AI 工具調用，以確保網頁介面、展示影片與行銷素材的視覺一致性。

---

## 品牌基因碼 (Brand YAML Snippet)

```yaml
Brand_Identity:
  Name: "Mapmo"
  Core_Value: "利用 EXIF 數據，讓每一張照片都能在精確的地理位置上說故事。"
  Slogan: "走過的路，讓地圖告訴你。"
  Target_Audience: ["攝影愛好者", "深度旅遊者", "數位遊牧民族"]

Visual_System:
  Style: "Minimalist & Map-centric" # 以地圖為核心的極簡風格
  Color_Palette:
    Primary: "#3B82F6"               # 地圖科技藍
    Secondary: ["#F97316", "#10B981"] # 冒險橘、導航綠
  Typography:
    Heading: "Montserrat / Noto Sans TC Bold"
    Body: "Inter / Noto Sans TC Regular"

Content_Vibe:
  Vibe: ["Adventurous", "Precise", "Clean"] # 冒險感、精確、乾淨
  Tone: "專業且具啟發性"
  Keywords: ["地圖敘事", "地理資訊", "視覺足跡"]

Constraints:
  Negative_Prompt: "No messy layouts, No cluttered icons, No low-contrast text"
```

---

## 應用說明 (Implementation Guide)

### 1. 驅動 Google Stitch (網頁展示)
將 `Color_Palette` 中的 `#3B82F6` 設定為網頁的主色調（Primary Color），並將 `Style` 描述輸入 Stitch 的氛圍設計（Vibe Design）欄位。

### 2. 驅動 AI 影片工具 (展示影片)
在生成 30 秒募資短片時，將 `Content_Vibe` 中的 `Adventurous` (冒險感) 作為配音與背景音樂的風格關鍵字，確保影片節奏輕快且充滿探索感。

### 3. 驅動 Gemini (簡報文案)
在製作 Pitch Deck 時，利用 `Core_Value` 與 `Target_Audience` 要求 AI 生成針對「攝影愛好者」痛點的說服性文案。

---
**授課教師**：林展 (Lin Chan)
**課程單位**：世新大學 資訊傳播學系 (ICS)