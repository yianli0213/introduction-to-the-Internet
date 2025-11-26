# 🌐 網際網路導論 - 課程作業與專題 (Introduction to the Internet)

歡迎來到我的課程學習歷程檔案！本倉庫 (Repository) 記錄了這學期在 **[國立臺灣師範大學]** 修習 **網際網路導論** 課程的所有實作成果。

本學期共包含四個主要階段的實作，從基礎的靜態網頁設計，進階到 React 前端框架，最後整合 API 與 AI 模型，完成期末專題。

---

## 📂 專案目錄 (Table of Contents)

1.  [作業一：個人網站設計 (Personal Website)](#1-作業一個人網站設計-personal-website)
2.  [作業二：React 城市儀表板與 AI 助理](#2-作業二react-城市儀表板與-ai-助理)
3.  [作業三：網站 API 串接實作](#3-作業三網站-api-串接實作)
4.  [期末專題：[Brezzy Day]](#4-期末專題-final-project)

---

## 1. 📄 作業一：個人網站設計 (Personal Website)

### 📝 專案簡介
這是本學期的第一個實作，目標是使用純 **HTML** 與 **CSS** 打造一個響應式的個人自我介紹網站。透過此作業，我掌握了網頁結構與樣式排版的核心基礎。

### 🛠️ 使用技術
- **HTML5**: 語意化標籤結構。
- **CSS3**: Flexbox/Grid 排版、RWD 響應式設計。
- **JavaScript (基礎)**: 簡單的互動效果。

### ✨ 功能亮點
- 個人簡介與經歷展示。
- 響應式導航欄 (RWD Navbar)。
- [圖片的展示]

---

## 2. ⚛️ 作業二：React 城市儀表板與 AI 助理

### 📝 專案簡介
本作業進入現代化前端開發，使用 **React** 框架實作。專案分為兩個部分：驗證台北城市儀表板的資料流，並實作一個結合 **Google Gemini API** 的智慧交通助理。

### 🛠️ 使用技術
- **Framework**: React (Hooks, Functional Components).
- **HTTP Client**: Axios / cURL.
- **AI Model**: Google Gemini API (`gemini-2.0-flash`).

### ✨ 功能亮點
1.  **台北城市儀表板 API 驗證**：
    - 使用 cURL 呼叫「交通」、「環境」、「防災」等三個不同主題 API。
    - 驗證 JSON 原始數據與網頁圖表顯示的一致性。
2.  **AI 捷運擁擠度助理**：
    - 實作模擬 IoT 數據邏輯，根據時段生成捷運擁擠度 (紅/黃/綠燈)。
    - 透過 Prompt Engineering 讓 AI 扮演交通專家，根據數據提供公車替代方案。
    - 動態 UI：對話框顏色隨擁擠程度自動變化。

👉 **[點擊觀看作業二 Demo 影片1](https://youtu.be/Vu3qq4xyTg4) **
👉 **[點擊觀看作業二 Demo 影片2](https://youtu.be/hM52nsiLLpM) **

---

## 3. 🔗 作業三：網站 API 串接實作

### 📝 專案簡介
基於作業一的個人網站基礎，進一步加入 **JavaScript Fetch API** 來串接真實的第三方資料，讓靜態網頁轉變為具有動態資料更新能力的網站。

### 🛠️ 使用技術
- JavaScript (ES6+).
- Fetch API / Async Await.
- [Github api/Apple music api].

### ✨ 功能亮點
- **即時資料獲取**：[例如：顯示當前所在地天氣資訊]。
- **DOM 操作**：將取得的 JSON 資料動態渲染至網頁上。
- **錯誤處理**：處理 API 請求失敗或載入中的狀態。

---

## 4. 🎓 期末專題 (Final Project)

### 🏆 專案名稱：[Brezzy Day]

### 📝 專案簡介
這是本學期的集大成之作，整合了前三個作業所學的技術（HTML/CSS 排版、React 組件化開發、API 串接、AI 整合），解決一個實際生活中的問題。

### 🛠️ 技術棧
- **Frontend**: React / [Mongo].
- **Backend/API**: [例如：Firebase / Node.js / 台北市政府空氣品質 API].
- **Other**: [例如：地圖套件 / 圖表套件].

### ✨ 專案特色
- **特色功能 1**：[例如：即時取得所在地區空氣品質]。
- **特色功能 2**：[例如：按照當日天氣溫度推薦穿著]。
- **特色功能 3**：[例如：發送客製化通知]。

👉 **[專案詳細說明與原始碼請見此資料夾](./final-project)** *(或是放上期末專案的 GitHub 連結)*

---

## 👤 作者

**[李怡安]**
- 學號：[41171131H]
- GitHub: [yianli0213](https://github.com/yianli0213)
- 聯絡方式：[ann930213@gmail.com]

---

*本專案為 [國立師範大學] 網際網路導論課程 114 學年度作品。*
