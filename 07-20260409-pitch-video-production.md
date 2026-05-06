---
marp: true
theme: default
paginate: true
size: 16:9
style: |
  section { justify-content: center; }
filename: 07-20260409-pitch-video-production.md
title: 07-行銷素材：AI 募資短片製作
date: 2026-04-09
tags:
  - marp
  - lecture
  - startup
  - video-ai
project: 114-2-資傳人才新創育成
description:
status: active
type: lecture
area: SHU
week: 7
created: 2026-04-14T18:38:00
updated: 2026-04-14T18:40:00
---

# 114-2 資傳人才新創育成
## Week 07: Pitch Video Production
**授課教師**：林展

---

## 為什麼 Pitch 需要「短片」？
在短短 3 分鐘的提案中，影片能跨越文字，快速建立：
1. **情境感**：讓評審看見產品如何在真實生活中解決問題。
2. **信任感**：展示原型 (Prototype) 的運作邏輯。
3. **情緒連結**：透過音樂與視覺敘事，強化品牌 DNA。

---

## 先用品牌 YAML

- 結構化的提示詞規範
- 確保 AI 在產出 Logo、網頁、影片與文案時，視覺與調性能夠高度吻合。

---

## 為什麼 YAML ？

YAML, `Yet Another Markup Language` -> `YAML Ain't a Markup Language`

平常我們用自然語言跟 AI 溝通（e.g：我要一個藍色的、科技感的 Logo），AI 容易有「幻覺」或漏看關鍵字。

---

## 為什麼 YAML ？續

使用 **YAML 格式** 有三大優勢：
- **精準控制**：透過鍵-值（Key-Value）對，強迫 AI 嚴格遵守設定（如指定 HEX 色碼）。
- **跨工具通用**：同樣的一份 YAML ，丟給生成圖片的 Midjourney、架站的 Stitch、或寫文案的 Gemini，產出的風格都會一致。
- **易於管理**：這非常符合 **Personal Knowledge Management (PKM)** 的邏輯，你可以輕易地將這段代碼(Snippet)存在筆記系統(我的愛Obsidian)中，隨時調用。

---

```YAML
Brand_Identity:
  Name: "你的品牌名稱"
  Vibe: ["形容詞 1", "形容詞 2"] # 定義氛圍
  Core_Value: "核心價值主張"

Visual_System:
  Style: "例如：Minimalist, Cyberpunk" # 視覺風格
  Color_Palette:
    Primary: "#HEX色碼"               # 主色
    Secondary: ["#輔助色1", "#2"]     # 輔助色
  Typography: "字體調性建議"           # 字體

Constraints:
  Negative_Prompt: "絕對不要出現的元素" # 排除條件
```

---

## Step 1: 腳本生成 (Scripting)
利用 Gemini 根據你的 YAML 基因產出「廣告腳本」：
> 「請根據我的品牌 YAML [貼入 YAML]，撰寫一段 30 秒的產品預告片腳本。結構包含：痛點畫面 (10s) -> 產品現身 (10s) -> 改變後的未來與 CTA (10s)。」

---

## Step 2: AI 影音工具實戰
* **畫面生成 (Text-to-Video)**：使用 **Runway Gen-3** 或 **Luma Dream Machine** 產出產品意境。
* **虛擬分身 (Avatar)**：使用 **HeyGen** 讓數位創辦人親自解說。
* **配音 (Voiceover)**：使用 **ElevenLabs** 產出具備溫度的旁白。
* **快速剪輯**：使用 **CapCut (剪映)** 的 AI 一鍵成片功能。

---

## 課堂任務：30 秒概念短片
利用這堂課，將你們的視覺規範「動起來」。
* [ ] **視覺風格一致**：色調必須符合 Brand Guideline。
* [ ] **解決方案清晰**：影片結束後，觀眾必須知道你們在賣什麼。
---