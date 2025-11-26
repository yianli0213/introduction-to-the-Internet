 台北城市儀表板與 AI 智慧交通助理 (React 實作)本專案是一個 React Web 應用程式，示範如何串接外部資料 API 與生成式 AI 模型。專案包含「台北城市儀表板 API 探索」與「Gemini AI 捷運擁擠度助理」兩大核心功能。🎬 專案展示影片 / Demo Video請點擊下方連結觀看完整解說影片（含 cURL 操作與 AI 實測）：👉 [請在此貼上你的 YouTube 影片連結]🚀 專案功能特色1. 🤖 AI 捷運擁擠度助理 (Gemini Integration)智慧模擬資料層：實作 fetchRealMRTData 函式，模擬真實 IoT 設備回傳的 JSON 數據（包含紅/黃/綠燈號），根據尖峰/離峰時間自動調整擁擠狀態。Gemini 1.5 Flash 串接：使用 Google Gemini API (v1beta/models/gemini-1.5-flash) 進行自然語言處理。角色扮演提示工程 (Role-Playing)：設定 System Instruction 讓 AI 扮演「台北交通指揮中心人員」，根據數據提供專業且人性化的公車替代建議。動態 UI 回饋：對話框顏色會根據擁擠程度（🔴 紅燈警示 / 🟢 綠燈舒適）自動變換樣式。2. 🏙️ 台北城市儀表板 API 驗證 (cURL)針對台北城市儀表板 (City Dashboard) 的三個不同主題 API 進行了完整的 cURL 呼叫測試與資料結構分析。驗證了 API 回傳的 JSON 數據與網頁前端顯示的一致性。🛠️ 技術棧 (Tech Stack)前端框架：ReactHTTP 請求：Axios (用於 REST API 串接)AI 模型：Google Gemini API (gemini-1.5-flash)開發工具：VS Code, Git, cURL📋 實作細節說明📂 核心程式碼：src/Assistant.jsx (或 .tsx)這是本專案的核心 AI 元件，主要邏輯如下：資料模擬：透過演算法判斷當前時間 (new Date()) 與站點名稱，回傳模擬的捷運擁擠度 JSON。Prompt 組合：將「模擬數據」與「使用者問題」打包，發送給 Gemini。API 呼叫：JavaScript// 使用 REST API 格式發送 Post 請求
axios.post(API_URL, {
    contents: [{ parts: [{ text: prompt }] }],
    system_instruction: {
        parts: [{ text: "你是一位精通臺北市即時交通狀況的專業助理..." }]
    }
})
錯誤處理：包含完整的 try...catch 機制，能捕捉 HTTP 400/500 錯誤並提示使用者檢查 API Key。🔍 API 串接清單 (步驟 2 展示)主題說明API Endpoint (範例)交通捷運/停車場相關數據.../api/v1/component/117/chart環境降雨/空氣品質監測.../api/v1/component/255/chart其他城市相關統計數據.../api/v1/component/34/chart(註：上述 API 呼叫過程已收錄於 Demo 影片中)📦 安裝與執行 (Installation)若您希望在本地端執行本專案，請依照以下步驟：複製專案 (Clone)Bashgit clone https://github.com/yianli0213/introduction-to-the-Internet.git
cd introduction-to-the-Internet
安裝依賴 (Install Dependencies)Bashnpm install
# 或
yarn install
設定 API Key啟動專案後，在網頁介面上方的輸入框填入您的 Google Gemini API Key 即可開始對話。(注意：為確保資安，原始碼中不包含寫死的 API Key)啟動專案 (Start)Bashnpm start
開啟瀏覽器前往 http://localhost:8081 (或終端機顯示的 port)。👤 作者[你的名字/學號]GitHub: yianli0213
