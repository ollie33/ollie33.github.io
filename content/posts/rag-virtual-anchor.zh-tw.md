---
title: "虛擬主播生成系統"
subtitle: "用 RAG 讓財經影音生成從「講得很順」變成「講得是真的」"
period: "2025.02 – 2025.12"
status: "TCSE 2025 論文發表"
impact: "佳作 7 / 80 · 事實密度 +80%"
date: 2025-12-31
kind: "畢業專題 · 論文發表"
hook: "技術深度：從架構設計一路帶到論文發表的 AI 系統。"
weight: 10

overview: "輸入股票代碼，10 分鐘內產出一支播報影片——用檢索讓講稿說的是當天真實發生的事。"

highlight: "帶領四人團隊；負責檢索框架與後端架構。"

role:
  - title: "Project Leader"
    module: "訂定目標與範圍；統整四人的模組，並解決模組交界處的問題。"
  - title: "RAG 檢索框架"
    module: "新聞過濾、模型選型，與手動建置的財經術語語義資料庫。"
  - title: "後端架構"
    module: "Flask 控制中樞、任務管理、SSE 串流。"

challenge_points:
  - "市場每天在動，一支專業影片卻要做好幾個小時。"
  - "不接檢索的 LLM 講得非常流暢，但零個可查證的事實。"
  - "通用嵌入模型串不起新聞裡的「死亡交叉」和算出它的技術指標。"

solution_points:
  - "自建財經題答集，實測比較 5 個嵌入模型。"
  - "手動建置語義標準化層，讓新聞語言對齊技術指標。"
  - "SSE 串流：按下生成後 5 秒內收到首波回饋。"

decisions:
  - title: "嵌入模型用實測選，不憑感覺"
    body: "中文財經檢索沒有現成基準，我自建題答集比較五個模型。BAAI/bge-m3 勝出——hit rate 73.59%、MRR 65.54%。"
    tradeoff: "建題答集的時間本可拿去多做功能，但沒有這組數字，之後每次檢索品質變差都無從歸因。"
  - title: "加一層語義標準化"
    body: "選對模型仍檢索不準——新聞用語和指標數值在向量空間對不上。我手動建了一套資料庫，把兩邊校正到同一個描述層。"
    tradeoff: "手動建置換不了領域、不會自己長大。對一學期的專題是划算的；要產品化就必須改成可自動擴充。"
  - title: "改用 SSE——這是體驗決策，不是技術決策"
    body: "長任務讓使用者面對空白畫面，那正是流失發生的地方。SSE 讓進度 5 秒內回到眼前。"
    tradeoff: "總生成時間一秒都沒變快，改變的只有感知效能——結果那才是真正重要的那個。"

architecture_title: "系統架構"
flow:
  - title: "爬取"
    detail: "MoneyDJ／鉅亨／Yahoo 股市 + yfinance"
  - title: "標準化"
    detail: "新聞語言 ↔ 技術指標"
  - title: "檢索"
    detail: "bge-m3 + FAISS"
  - title: "生成講稿"
    detail: "指標 + Top-5 段落 → OpenAI"
  - title: "語音"
    detail: "Google Cloud TTS"
  - title: "渲染"
    detail: "Unity + Live2D，經 SSE 回推"

image: "/images/rag-architecture.jpg"
image_caption: "五層架構、11 個流程步驟，全程無人工介入。"

demo_link: "https://github.com/ollie33/Virtual-Anchor-Generation-System"

content_title: "成果與反思"
---

### 成果

- **事實密度 +80%**——同一批標的、有無 RAG 兩版講稿逐篇比對可查證事實點。
- **數小時 → 10 分鐘內**，全自動。
- **佳作 7/80**（逢甲資工專題競賽）· **TCSE 2025 全文發表**。

### 反思

如果重做，我會把系統做成 **agent 架構**。現在的管線對每種題材都走同一條路——但法說會、突發利空、技術面盤整，需要的檢索和敘事結構完全不同。

Agent 架構能讓系統自己決定要查什麼、怎麼講。這是這個專案最明顯的天花板——而我是做完才看清楚它在哪裡。
