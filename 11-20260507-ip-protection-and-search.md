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
    font-size: 0.8em;
    width: 100%;
  }
  .highlight {
    color: #b30000;
    font-weight: bold;
  }
filename: 11-20260507-ip-protection-and-search.md
title: 11-智財保護與檢索實戰 (IP Protection & Search)
course: ICS Startup Ecosystems & Talent Development
week: 11
date: 2026-05-07
status: active
version: 3
project: 114-2-資傳人才新創育成
area: SHU
created: 2026-04-29T12:26:00
updated: 2026-05-06T19:54:00
---

<!-- _class: lead -->
![bg left:45%](https://images.unsplash.com/photo-1589829545856-d10d557cf95f?q=80&w=1600&auto=format&fit=crop)

# 114-2 資傳人才新創育成
ICS Startup Ecosystems & Talent Development
## Week 11: 智財保護與檢索實戰
**授課教師**：林展
**日期**：2026 / 05 / 07

---

## 今日核心：守護你的數位資產

在 W10 決定了公司名稱後，這週我們要確保你的品牌與技術具備「排他性」。

**課程目標：**
1. **商標基礎 (Trademark)**：理解類別與符號（©, ™, ®）的法律意義。
2. **專利基礎 (Patent)**：理解發明、新型與設計專利的差異。
3. **檢索實戰**：學會使用「智慧財產局」系統進行檢索。
4. **IP YAML 建立**：將智財規劃與品牌資產結構化。

---

## 1. 商標：品牌的身分證

對於資傳產出專案（App、平台、內容服務），最常涉及的類別：
* **第 09 類**：錄載有電腦程式之光碟、可下載之電腦軟體。
* **第 35 類**：廣告、企業管理、電子商務零售。
* **第 42 類**：電腦硬體與軟體之設計與開發 (**ICS 專案核心**)。

<div class="highlight">警告：名稱沒過商標檢索，強行品牌化可能導致日後被迫改名或支付賠償金。</div>

---

## 1.1 標記的藝術：© vs ™ vs ®

在產品介面底部或 Logo 旁，這些符號代表的法律位階完全不同：

| 符號 | 名稱 | 法律效力 | 取得方式 |
| :---: | :--- | :--- | :--- |
| **©** | **Copyright (著作權)** | 保護表現形式（設計圖、程式碼、文案）。 | **自動取得**。作品完成即受保護。 |
| **™** | **Trademark (商標聲明)** | 警示大眾「我打算將此作為商標使用」。 | **自行標註**。無須登記，保障較弱。 |
| **®** | **Registered (註冊商標)** | **最強保護**。證明已通過智財局核准。 | **審核通過**。拿到證書才能標註。 |

---

## 什麼時候該用哪一個？

* **© (Copyright)**：
    * **情境**：UI 介面、宣傳影片。標註 `© 2026 Mapmo Inc.` 提醒他人勿侵權。
* **™ (Trademark)**：
    * **情境**：剛想好 Logo 但還沒拿到證書。這是告訴對手「我在用了」。
* **® (Registered)**：
    * **嚴禁**：**未經註冊嚴禁標註**。這涉及虛偽標示，可能吃上官司！ 拿到正式註冊證後，請立刻將 ™ 升級為 ®。

---

## AI 生成 Logo 的法律陷阱

如果 Logo 是直接用生成式 AI 生成的，請特別注意：

* **沒有著作權 (No ©)**：目前台灣與國際多數實務認定，純 AI 生成的圖像缺乏「人類精神創作」，**無法取得著作權**。別人原封不動照抄你的 AI Logo，你很難用《著作權法》告他。
* **可以當商標用 (Can use ™ / ®)**：只要這張圖具備「識別性」，且沒抄襲現有商標，你依然可以將它作為商標使用（標註 ™），甚至去註冊（®）。
* **破解法 (Human Touch)**：用 AI 生成草圖後，務必透過 Illustrator 進行**人為的大幅度修改、向量化與排版**。有人介入創作，才能同時獲得 © 與 ™ 的雙重防護網。

---

## 2. 專利：技術的保護

資傳系的畢業製作或新創專案可以申請專利嗎？
* **發明專利 (20年)**：具備高度創作性，如：特殊的 AI 演算法流程。
* **新型專利 (10年)**：針對物體形狀、構造的改良（如硬體裝置）。
* **設計專利 (15年)**：針對物品之形狀、花紋、色彩或其結合之創作 (**UI 介面屬此類**)。

---

## 3. 檢索實戰：只能有一個鼎泰豐

**實作任務：**
1. 進入 [經濟部智慧財產局商標檢索系統](https://tmsearch.tipo.gov.tw/)。
2. 輸入你們上週擬定的 3 個公司名稱。
3. **查核點**：是否有相似名稱已在同類別（如 42 類）註冊？
4. **思考**：如果名稱被佔用了，你們要微調名字，還是換一個類別競爭？

---

## 實作練習 1：智財保護 YAML 化

請各組更新專案筆記中的 IP 策略，釐清整體法律佈局：
```yaml
IP_Protection_Strategy:
  Trademark_Plan:
    Proposed_Name: "Mapmo"
    Target_Classes: ["09", "42"]
    Search_Status: "Clear / Conflict Found" # 填寫今日檢索結果
    Symbol_Usage: "Currently using ™"
  Patent_Potential:
    Feature: "地理位置自動生成敘事演算法"
    Type_Target: "發明專利 / 設計專利 (UI)"
  Action_Item: "預計於 2026 Q4 委託事務所進行正式申請"
```

---

## 實作練習 2：品牌資產與商標管理 YAML

將 Logo 的「產製過程」記錄下來，這能幫助 AI 後續自動生成品牌手冊 (Brand Guidelines) 或授權書：

```yaml
Brand_Assets_Manager:
  Brand_Name: "Mapmo"
  Visual_Identity:
    Primary_Color: "#FF5A5F"
    Typography: "Noto Sans TC"
  Logo_Creation_Log:
    Method: "AI Assisted (Midjourney + Illustrator)"
    AI_Prompt: "A minimalist map pin forming a letter M, geometric, flat design, vector style"
    Human_Modification: "在 AI 中重新描繪向量路徑、微調圓角比例、加入專屬標準字"
    Copyright_Status: "具備人類加工心血，主張擁有 ©"
  Trademark_Status:
    Current_Symbol: "™"
    Search_Record_Image: "2026-05-07_TIPO_Search_Clear.png"
```

---

![bg right:40%](https://images.unsplash.com/photo-1556761175-5973dc0f32e7?q=80&w=1600&auto=format&fit=crop)

## 課堂任務：智財防禦報告

請各團隊完成以下任務並更新至專案筆記：
* [ ] ~~**商標檢索截圖**：截圖檢索結果並分析潛在侵權風險。~~
* [ ] **IP 策略 YAML**：寫入專案筆記中 IP 策略 YAML。
* [ ] **建立品牌 YAML**：確實記錄 Logo 的產製過程（由人修改了哪裡）。
* [ ] **標註檢查**：在你們的 **Stitch 網頁** 底部正確標註 © 與 ™。
* [ ] **著作權聲明**：針對專案中純 AI 生成的素材，撰寫一份權利聲明。*利用 [範本](https://seraphwu.github.io/ICS-Startup-Ecosystems-Talent-Development/11-supplement-ai-copyright-template) 進行修改*

---

## 下週預告：定價心理學與策略 (Week 12)

保護好了技術，下週我們要決定產品的「身價」：
* **定價心理學**：為什麼 99 元比 100 元更有魔力？
* **成本利潤計算**：算清楚每一筆訂單的毛利。
* **競品比價表**：找出你們在市場中的價格甜蜜點。

⚠️ **請確保今日的 IP 檢索結果已存檔，這會影響你未來的品牌支出預算。**