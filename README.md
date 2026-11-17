<!-- saved from url=(0058)file:///C:/Users/mahar/Downloads/Politologiya_sinaq_5.html -->
<html lang="az"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
  
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Financial Accounting</title>
  <style>
    :root {
      --bg: #121212;
      --bg2: #1b1b1b;
      --panel: #1E1E1E;
      --panel2: #242424;
      --line: #2D2D2D;
      --text: #F3F4F6;
      --muted: #9CA3AF;
      --accent: #8B5CF6;
      --accent2: #06B6D4;
      --good: #22C55E;
      --bad: #EF4444;
      --warn: #F59E0B;
      --danger-quiz-text: #FCA5A5;
      --danger-quiz-border: #7F1D1D;
      --danger-quiz-bg: rgba(127, 29, 29, 0.10);
      --page-bg: #121212;
      --page-bg2: #0f0f0f;
      --card-bg: #1E1E1E;
      --card-bg-soft: #252525;
      --surface: #242424;
      --surface-hover: #2c2c2c;
      --surface-selected: rgba(139, 92, 246, 0.18);
      --surface-correct: rgba(34, 197, 94, 0.16);
      --surface-wrong: rgba(239, 68, 68, 0.14);
      --input-bg: #181818;
      --input-border: #2D2D2D;
      --btn-bg: #242424;
      --btn-border: #2D2D2D;
      --shadow: 0 20px 60px rgba(0,0,0,.35);
      --radius: 22px;
    }
    body[data-theme="light"] {
      --bg: #F8FAFC;
      --bg2: #FFFFFF;
      --panel: #FFFFFF;
      --panel2: #FFFFFF;
      --line: #E2E8F0;
      --text: #111827;
      --muted: #6B7280;
      --accent: #2563EB;
      --accent2: #0891B2;
      --good: #16A34A;
      --bad: #B91C1C;
      --warn: #D97706;
      --danger-quiz-text: #7F1D1D;
      --danger-quiz-border: #7F1D1D;
      --danger-quiz-bg: rgba(127, 29, 29, 0.10);
      --page-bg: #F8FAFC;
      --page-bg2: #EEF2F7;
      --card-bg: #FFFFFF;
      --card-bg-soft: #F8FAFC;
      --surface: #FFFFFF;
      --surface-hover: #EEF2F7;
      --surface-selected: rgba(37, 99, 235, 0.12);
      --surface-correct: rgba(22, 163, 74, 0.12);
      --surface-wrong: rgba(220, 38, 38, 0.10);
      --input-bg: #FFFFFF;
      --input-border: #E2E8F0;
      --btn-bg: #FFFFFF;
      --btn-border: #E2E8F0;
      --shadow: 0 18px 40px rgba(15,23,42,.08);
    }
    * { box-sizing: border-box; }
    body {
      margin: 0;
      min-height: 100vh;
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      color: var(--text);
      background:
        radial-gradient(circle at top left, color-mix(in srgb, var(--accent) 24%, transparent), transparent 28%),
        radial-gradient(circle at top right, color-mix(in srgb, var(--accent2) 16%, transparent), transparent 24%),
        linear-gradient(180deg, var(--page-bg2) 0%, var(--page-bg) 45%, var(--bg2) 100%);
    }
    .app {
      max-width: 1200px;
      margin: 0 auto;
      padding: 28px 18px 46px;
    }
    .topbar {
      position: sticky;
      top: 12px;
      z-index: 40;
      display: flex;
      justify-content: flex-end;
      margin: 0 auto 12px;
      max-width: 1200px;
      padding: 0 18px;
      pointer-events: none;
    }
    .topbar .ghost {
      pointer-events: auto;
      backdrop-filter: blur(10px);
    }
    body[data-mode="quiz"] .hero,
    body[data-mode="results"] .hero {
      display: none;
    }
    body[data-mode="quiz"] .app,
    body[data-mode="results"] .app {
      padding-top: 12px;
    }

    .hero {
      display: grid;
      gap: 14px;
      grid-template-columns: 1.6fr 1fr;
      align-items: stretch;
      margin-bottom: 18px;
    }
    .card {
      background: linear-gradient(180deg, var(--card-bg), var(--card-bg-soft));
      border: 1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      backdrop-filter: blur(14px);
    }
    .hero-main, .hero-side {
      padding: 22px;
    }
    h1 {
      margin: 0 0 8px;
      font-size: clamp(28px, 4vw, 44px);
      letter-spacing: -.03em;
    }
    .subtitle {
      color: var(--muted);
      line-height: 1.6;
      margin: 0;
      max-width: 70ch;
    }
    .stats {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 12px;
      margin-top: 18px;
    }
    .stat {
      padding: 14px 16px;
      border-radius: 18px;
      background: var(--surface);
      border: 1px solid var(--line);
    }
    .stat .label {
      color: var(--muted);
      font-size: 12px;
      margin-bottom: 6px;
    }
    .stat .value {
      font-size: 20px;
      font-weight: 700;
    }
    .controls {
      display: grid;
      gap: 12px;
    }
    .field-row {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 12px;
    }
    label {
      display: block;
      font-size: 13px;
      color: var(--muted);
      margin-bottom: 7px;
    }
    input[type="number"],
    input[type="text"] {
      width: 100%;
      padding: 14px 15px;
      background: var(--input-bg);
      color: var(--text);
      border: 1px solid var(--input-border);
      border-radius: 14px;
      outline: none;
      font-size: 15px;
    }
    input[type="number"]:focus {
      border-color: var(--accent2);
      box-shadow: 0 0 0 3px color-mix(in srgb, var(--accent2) 18%, transparent);
    }
    .btn-row {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      align-items: center;
    }
    button {
      border: 0;
      border-radius: 14px;
      padding: 13px 16px;
      color: var(--text);
      background: var(--surface);
      cursor: pointer;
      transition: transform .12s ease, background .2s ease, opacity .2s ease;
      font-weight: 600;
    }
    button:hover { transform: translateY(-1px); }
    .primary {
      background: linear-gradient(135deg, var(--accent), var(--accent2));
      box-shadow: 0 10px 30px color-mix(in srgb, var(--accent) 25%, transparent);
    }
    .ghost {
      background: var(--btn-bg);
      border: 1px solid var(--btn-border);
    }
    .wrong-quiz-btn {
      border-color: var(--danger-quiz-border);
      color: var(--danger-quiz-text);
      background: var(--danger-quiz-bg);
    }
    .wrong-quiz-btn:hover {
      transform: translateY(-1px);
      filter: brightness(1.03);
    }
    .tiny {
      padding: 9px 12px;
      font-size: 13px;
      border-radius: 12px;
    }
    .hint {
      color: var(--muted);
      font-size: 13px;
      line-height: 1.5;
    }
    .main {
      margin-top: 18px;
      display: grid;
      gap: 16px;
    }
    .progress-wrap {
      padding: 16px 18px;
    }
    .progress-head {
      display: flex;
      justify-content: space-between;
      gap: 10px;
      align-items: center;
      margin-bottom: 10px;
      flex-wrap: wrap;
    }
    .progress-bar {
      width: 100%;
      height: 10px;
      border-radius: 999px;
      overflow: hidden;
      background: var(--surface);
    }
    .progress-fill {
      height: 100%;
      width: 0%;
      background: linear-gradient(90deg, var(--accent), var(--accent2));
      border-radius: 999px;
      transition: width .25s ease;
    }
    .quiz-card {
      padding: 22px;
    }
    .question-meta {
      display: flex;
      justify-content: space-between;
      gap: 12px;
      flex-wrap: wrap;
      align-items: center;
      margin-bottom: 12px;
      color: var(--muted);
      font-size: 13px;
    }
    .qtitle {
      font-size: 20px;
      line-height: 1.5;
      margin: 0 0 16px;
      letter-spacing: -.01em;
    }
    .options {
      display: grid;
      gap: 10px;
    }
    .option {
      text-align: left;
      padding: 14px 15px;
      border-radius: 16px;
      background: var(--surface);
      border: 1px solid var(--btn-border);
      transition: background .15s ease, border-color .15s ease, transform .12s ease;
    }
    .option:hover {
      background: var(--surface-hover);
      border-color: var(--line);
    }
    .option.selected {
      background: var(--surface-selected);
      border-color: var(--accent);
    }
    .option.correct {
      background: var(--surface-correct);
      border-color: var(--good);
    }
    .option.wrong {
      background: var(--surface-wrong);
      border-color: var(--bad);
    }
    .foot {
      display: flex;
      justify-content: space-between;
      gap: 12px;
      flex-wrap: wrap;
      margin-top: 18px;
      align-items: center;
    }
    .jump-box {
      display: flex;
      gap: 8px;
      align-items: center;
      flex-wrap: wrap;
      margin-top: 10px;
    }
    .jump-box input[type="number"] {
      width: 110px;
      padding: 11px 12px;
    }
    .review-grid {
      display: grid;
      gap: 14px;
    }
    .result-grid {
      display: grid;
      grid-template-columns: repeat(4, minmax(0, 1fr));
      gap: 12px;
    }
    .result-card {
      padding: 16px;
    }
    .result-card .label {
      color: var(--muted);
      font-size: 12px;
      margin-bottom: 7px;
    }
    .result-card .value {
      font-size: 24px;
      font-weight: 800;
    }
    .badge {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 7px 10px;
      border-radius: 999px;
      font-size: 12px;
      border: 1px solid var(--btn-border);
      background: var(--surface);
    }
    .badge.good { border-color: color-mix(in srgb, var(--good) 40%, transparent); color: var(--good); }
    .badge.bad { border-color: color-mix(in srgb, var(--bad) 40%, transparent); color: var(--bad); }
    .question-item {
      padding: 18px;
    }
    .question-item h3 {
      margin: 0 0 10px;
      font-size: 17px;
      line-height: 1.45;
    }
    .mini {
      color: var(--muted);
      font-size: 13px;
      line-height: 1.5;
    }
    .divider {
      height: 1px;
      background: var(--line);
      margin: 14px 0;
    }
    .saved-panel {
      margin-top: 14px;
      padding: 14px;
      border-radius: 18px;
      background: var(--surface);
      border: 1px solid var(--btn-border);
    }
    .saved-panel-head {
      display: flex;
      justify-content: space-between;
      gap: 10px;
      align-items: center;
      flex-wrap: wrap;
      margin-bottom: 0;
    }
    .saved-panel-toggle {
      width: 100%;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 12px;
      padding: 0;
      border: 0;
      background: transparent;
      color: inherit;
      text-align: left;
      cursor: pointer;
    }
    .saved-panel-toggle:hover .saved-panel-title {
      color: var(--text);
    }
    .saved-chevron {
      flex: 0 0 auto;
      transition: transform .2s ease;
      color: var(--muted);
      font-size: 16px;
      margin-left: 8px;
    }
    .saved-panel.open .saved-chevron {
      transform: rotate(180deg);
    }
    .saved-panel-body {
      margin-top: 12px;
      display: grid;
      gap: 12px;
    }
    .saved-panel-title {
      font-weight: 700;
      font-size: 14px;
    }
    .saved-panel-sub {
      color: var(--muted);
      font-size: 12px;
      margin-top: 4px;
    }
    .saved-list {
      display: grid;
      gap: 10px;
      max-height: 320px;
      overflow: auto;
      padding-right: 4px;
    }
    .saved-item {
      display: grid;
      grid-template-columns: 1fr auto;
      gap: 10px;
      align-items: start;
      padding: 12px 12px 12px 14px;
      border-radius: 16px;
      background: var(--surface);
      border: 1px solid var(--line);
    }
    .saved-item strong {
      display: block;
      font-size: 13px;
      line-height: 1.45;
      margin-bottom: 4px;
    }
    .saved-item .mini {
      font-size: 12px;
    }
    .saved-remove {
      padding: 8px 10px;
      border-radius: 10px;
      font-size: 12px;
      white-space: nowrap;
    }
    .saved-empty {
      color: var(--muted);
      font-size: 13px;
      line-height: 1.5;
      padding: 4px 2px 2px;
    }
    .hidden {
      display: none !important;
    }
    .footer-note {
      color: var(--muted);
      font-size: 12px;
      margin-top: 10px;
    }

    .theme-toggle {
      pointer-events: auto;
      display: inline-flex;
      align-items: center;
      gap: 10px;
      padding: 12px 14px;
      border-radius: 999px;
      border: 1px solid var(--line);
      background: linear-gradient(180deg, color-mix(in srgb, var(--panel) 92%, transparent), color-mix(in srgb, var(--panel2) 92%, transparent));
      color: var(--text);
      box-shadow: var(--shadow);
      backdrop-filter: blur(14px);
      min-width: 132px;
      justify-content: center;
    }
    .theme-toggle:hover { transform: translateY(-1px); }
    .theme-toggle-track {
      position: relative;
      width: 36px;
      height: 22px;
      border-radius: 999px;
      background: color-mix(in srgb, var(--accent) 18%, var(--surface));
      border: 1px solid var(--line);
      display: inline-flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
    }
    .theme-toggle-icon {
      position: absolute;
      font-size: 12px;
      line-height: 1;
      transition: opacity .18s ease, transform .18s ease;
      color: var(--accent);
    }
    .theme-toggle-sun { opacity: 0; transform: scale(.6) rotate(-25deg); }
    .theme-toggle-moon { opacity: 1; transform: scale(1) rotate(0deg); }
    body[data-theme="light"] .theme-toggle-sun { opacity: 1; transform: scale(1) rotate(0deg); }
    body[data-theme="light"] .theme-toggle-moon { opacity: 0; transform: scale(.6) rotate(25deg); }
    .theme-toggle-text {
      font-weight: 700;
      font-size: 13px;
      letter-spacing: .01em;
      white-space: nowrap;
      line-height: 1;
    }
    .theme-toggle-label {
      opacity: .95;
    }

    @media (max-width: 900px) {
      .hero, .result-grid { grid-template-columns: 1fr; }
      .field-row { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>
  <div class="topbar">
    <button class="theme-toggle" id="themeToggleBtn" type="button" aria-label="Tema rejimini dəyiş">
      <span class="theme-toggle-track" aria-hidden="true">
        <span class="theme-toggle-icon theme-toggle-sun">☀</span>
        <span class="theme-toggle-icon theme-toggle-moon">☾</span>
      </span>
      <span class="theme-toggle-text theme-toggle-label" id="themeToggleText">Rejim</span>
    </button>
  </div>
  <div class="app">
    <div class="hero">
      <div class="card hero-main">
        <h1>Financial Accounting🎈</h1>
        <div class="stats">
          <div class="stat">
            <div class="label">Baza sual sayı</div>
            <div class="value" id="bankCount">338</div>
          </div>
          <div class="stat">
            <div class="label">Hazırkı aralıq</div>
            <div class="value" id="rangeLabel">1 – 338</div>
          </div>
          <div class="stat">
            <div class="label">Sınaq sualı</div>
            <div class="value" id="quizCount">50</div>
          </div>
        </div>
      </div>

      <div class="card hero-side">
        <div class="controls">
          <div>
            <label for="customRanges">İnterval</label>
            <input id="customRanges" type="text" placeholder="4, 7, 100-120, 130">
            <div class="hint">Aralıqları vergüllə ayır. Tək ədəd və aralıq yaza bilərsən.</div>
          </div>
          <div class="btn-row">
            <button class="primary" id="startBtn">Başlat</button>
            <button class="ghost" id="savedQuizBtn">Saxlanılanlarla sınaq</button>
            <button class="ghost" id="resetBtn">Sıfırla</button>
          </div>
          <div class="hint">
            Seçilən aralıqdan təsadüfi 50 sual götürülür. Aralıq 50-dən az olsa, mövcud olan sualların hamısı işlənir.
          </div>
          <div class="footer-note" id="statusLine">Hazırdır.</div>
          <div class="saved-panel" id="savedPanel">
        <button type="button" class="saved-panel-toggle" id="savedPanelToggle" aria-expanded="false">
          <div class="saved-panel-head">
            <div>
              <div class="saved-panel-title">Yadda saxlanılan suallar (0)</div>
              <div class="saved-panel-sub">Sualı saxlamaq və silmək lokal yaddaşda qalır.</div>
            </div>
          </div>
          <div class="saved-chevron" aria-hidden="true">⌄</div>
        </button>
        <div class="saved-panel-body hidden">
          <div class="btn-row">
            <button class="ghost tiny" id="savedQuizBtn2">Saxlanılanlarla sınaq</button>
            <button class="ghost tiny" id="clearSavedBtn">Hamısını təmizlə</button>
          </div>
          
          <div class="saved-empty">Hələ heç nə saxlanmayıb. Sınaqdakı sualda “Yadda saxla” düyməsinə bas.</div>
        </div>
      </div>
        </div>
      </div>
    </div>

    <div class="main" id="appRoot">
      <div class="card progress-wrap hidden" id="progressCard">
        <div class="progress-head">
          <div id="progressText">0 / 0</div>
          <div id="timerText" class="badge">Sual</div>
        </div>
        <div class="progress-bar"><div class="progress-fill" id="progressFill"></div></div>
      </div>

      <div class="card quiz-card hidden" id="quizCard"></div>
      <div class="card review-grid hidden" id="resultsCard"></div>
    </div>
  </div>

  <script>
    const QUESTION_BANK = [
  {
    "num": 1,
    "question": "Şirkət 31 dekabr 2024-cü il tarixində elektrik xərci fakturasını hələ almayıb, lakin dekabr ayı üçün 400 AZN xərcin olduğunu təxmin edir. Hansı korrektə yazılışı edilməlidir?",
    "options": [
      "Debit: Xərc 400 AZN, Kredit: Bank hesablaşma hesabl 400 AZN.",
      "Debit: Xərc 200 AZN, Kredit: Bank hesablaşma hesabl 200 AZN.",
      "Debit: Xərc 100 AZN, kredit: Hesablanmış öhdəlik 100 AZN.",
      "Debit: Xərc 400 AZN, Kredit: Hesablanmış öhdəlik 400 AZN.",
      "Debit: Xərc 400 AZN, Kredit: pul vəsaiti 400 AZN."
    ],
    "correct": "Debit: Xərc 400 AZN, Kredit: Hesablanmış öhdəlik 400 AZN."
  },
  {
    "num": 2,
    "question": "Aktivin ilkin dəyəri $90000 AZN, toplanmış amortizasiyası 30000 AZN-dir. Aktivin xalis satış qiyməti 50000 AZN, istifadə dəyəri isə 45000 AZN-dir. Aktivin yeni balans dəyəri hansı məbləğdə göstərilməlidir?",
    "options": [
      "50000",
      "80000",
      "30000",
      "45000",
      "60000"
    ],
    "correct": "50000"
  },
  {
    "num": 3,
    "question": "BBG Şirkəti hər biri 125$ olmaqla, 50 ədəd kompüter satın alır. Bir müddət sonra şirkət hər biri 150$ olmaqla yenidən 75 ədəd kompüter satın alır və hər biri 150$ müqabilində 100 ədəd kompüter satır.İMİM (FIFO) üsuluna əsasən, dövrün sonuna olan mal-material ehtiyatlarının dəyəri nə qədər olacaq?",
    "options": [
      "20 ədəd və dəyəri 2000 dollar",
      "10ədəd və dəyəri 3000 dollar",
      "25 ədəd və dəyəri 3750 dollar",
      "25 ədəd və dəyəri 2500 dollar",
      "20 ədəd və dəyəri 3000 dollar"
    ],
    "correct": "25 ədəd və dəyəri 3750 dollar"
  },
  {
    "num": 4,
    "question": "Yeni fəaliyyətə başlayan “Turan”MMM şirkəti yanvar ayında dörd partiya mal tədarük edir. 12 yanvarda – 150 ədəd – 530 manat; 14 yanvarda – 200 ədəd – 1480 manat; 18 yanvarda – 200 ədəd – 1660 manat; 20 yanvarda – 150 ədəd – 1090 manat. Anbarda olan malların ümumi dəyəri 4760 manatdır. 25 yanvar tarixində inventarizasiyanın nəticələrinə əsasən ehtiyatların qalığı 275 ədəd təşkil edir. 25 yanvar AVCO metodu ilə hesablamaya əsasən satılmış malların maya dəyəri nə qədər olacaq?",
    "options": [
      "3500",
      "3250",
      "2890",
      "3000",
      "3820"
    ],
    "correct": "2890"
  },
  {
    "num": 5,
    "question": "Yeni fəaliyyətə başlayan “XƏYAL”MMM şirkəti yanvar ayında dörd partiya mal tədarük edir. 12 yanvarda – 150 ədəd – 770 manat; 14 yanvarda – 200 ədəd – 1180 manat; 18 yanvarda – 200 ədəd – 1260 manat; 20 yanvarda – 150 ədəd – 990 manat. 25 yanvar tarixində inventarizasiyanın nəticələrinə əsasən ehtiyatların qalığı 200 ədəd təşkil edir. 25 yanvar AVCO metodu ilə hesablamaya əsasən satılmış malların maya dəyəri nə qədər olacaq?",
    "options": [
      "2865",
      "2500",
      "3845",
      "3000",
      "3150"
    ],
    "correct": "3000"
  },
  {
    "num": 6,
    "question": "Yanvarın 1-də Müəssisənin anbarında 30 ədəd hər birinin alış qiyməti 2 manat olan mal var. 12 yanvarda müəssisə 30 ədəd malı hər biri 2,5 manata olmaqla 75 mnata almışdır. 17 yanvarda müəssisə 50 ədəd malı hər biri 3 manata olmaqla 150 manata almışdır. 22 yanvarda satılmış 50 ədəd malın FİFO və AVCO metodları arasında maya dəyəri fərqini hesablayın.",
    "options": [
      "62.50",
      "75",
      "19.50",
      "178",
      "150"
    ],
    "correct": "19.50"
  },
  {
    "num": 7,
    "question": "Alınmasına 3000 AZN, quraşdırılmasına 800 AZN, xərc çəkilən aktivin ilkin dəyəri nə qədər olacaq?",
    "options": [
      "800",
      "2220",
      "0",
      "3000",
      "3800"
    ],
    "correct": "3800"
  },
  {
    "num": 8,
    "question": "Alınmasına 1000 AZN, daşınmasına 500 AZN, istifadə olunacağı tarixə qədər anbarda saxlanılmasına 150 AZN xərc çəkilən aktivin ilkin dəyəri nə qədər olacaq?",
    "options": [
      "1350",
      "1150",
      "1500",
      "800",
      "1000"
    ],
    "correct": "1500"
  },
  {
    "num": 9,
    "question": "Aktivin gözlənilən mümkün satış qiyməti 1100 manat, satışın baş tutması üçün çəkilməli olan xərc 400 manatdırsa, mümkün xalis satış dəyəri nə qədərdir?",
    "options": [
      "1100",
      "400",
      "1500",
      "700",
      "800"
    ],
    "correct": "700"
  },
  {
    "num": 10,
    "question": "Malsatana ticari öhdəlik hesabının ilkin qalığı 3000 manatdır. Dövr ərzində həmin malsatandan 4000 manat dəyə-rin-də kreditlə mal alınmış və həmin malsatana 5000 manat ödəniş edilmişdir. Dövrün sonuna hesabın qalığını hesablayın.",
    "options": [
      "5000",
      "7000",
      "8000",
      "2000",
      "4000"
    ],
    "correct": "2000"
  },
  {
    "num": 11,
    "question": "Yanvarın 1-də Müəssisənin anbarında 20 ədəd hər birinin alış qiyməti 2 manat olan mal var. 12 yanvarda müəssisə 30 ədəd malı hər biri 2,2 manata olmaqla 66 manata almışdır. 17 yanvarda müəssisə 50 ədəd malı hər biri 2,4 manata olmaqla 120 mnata almışdır. 22 yanvarda satılmış 50 ədəd malın FİFO və AVCO metodları arasında maya dəyəri fərqini hesablayın.",
    "options": [
      "120",
      "20",
      "66",
      "7",
      "22"
    ],
    "correct": "7"
  },
  {
    "num": 12,
    "question": "Yanvarın 1-də Müəssisənin anbarında 10 ədəd hər birinin alış qiyməti 2 manat olan mal var. 12 yanvarda müəssisə 30 ədəd malı hər biri 2,2 manata olmaqla 66 manata almışdır. 17 yanvarda müəssisə 50 ədəd malı hər biri 2,4 mana-ta olmaqla 120 mnata almışdır. 22 yanvarda satılmış 50 ədəd malın AVCO metodu ilə maya dəyərini hesablayın.",
    "options": [
      "110",
      "302",
      "114",
      "206",
      "120"
    ],
    "correct": "114"
  },
  {
    "num": 13,
    "question": "Yanvarın 1-də Müəssisənin anbarında 10 ədəd hər birinin alış qiyməti 2 manat olan mal var. 12 yanvarda müəssisə 30 ədəd malı hər biri 2,2 manata olmaqla 66 manata almışdır. 17 yanvarda müəssisə 50 ədəd malı hər biri 2,4 mana-ta olmaqla 120 manata almışdır. 22 yanvarda satılmış 50 ədəd malın FİFO metodu ilə maya dəyərini hesablayın.",
    "options": [
      "120",
      "116",
      "115",
      "117",
      "110"
    ],
    "correct": "110"
  },
  {
    "num": 14,
    "question": "ABC\" müəssisəsi ehtiyatların uçotunu AVCO (Orta dəyər) metodu ilə aparır. Aşağıda dövr üzrə alış və satışlar haqqında məlumat verilmişdir: 22 noyabr - qalıq 50 ədəd x 10 AZN = 500 AZN; 23 Noyabr alış 150 ədəd x 11 AZN = 1650 AZN; 24 Noyabr alış 200 ədəd x 12 AZN = 2400 AZN. 25 Noyabr satış 330 ədəd x 15 AZN = 4950 AZN. Dövrün sonuna məcmu (ümumi) mənfəəti hesablayın.",
    "options": [
      "1099,00 AZN",
      "3753,75 AZN",
      "2050,00 AZN",
      "1196,25 AZN",
      "22600 AZN"
    ],
    "correct": "1196,25 AZN"
  },
  {
    "num": 15,
    "question": "Corab alqı-satqısı ilə məşğul olan mağaza ehtiyatların uçotunu FIFO üsulu ilə aparır. Dövr üzrə alış və satışlar haqqında məlumat aşağıda verilmişdir: 1 May alış 100 ədəd x 0,40 AZN = 40 manat; 2 May alış 200 ədəd x 0,45 AZN = 90 manat; 3 May alış 150 ədəd x 0,50 AZN = 75 manat. Satılıb 300 ədəd. Dövrün sonuna qalıq malların maya dəyəri nə qədərdir?",
    "options": [
      "87.50",
      "60.00",
      "67.50",
      "75.00",
      "55.00"
    ],
    "correct": "75.00"
  },
  {
    "num": 16,
    "question": "Verilmiş məlumatlar əsasında FIFO metodu ilə şirkətin satılmış məhsulun maya dəyərini hesabla. 2 Dekabr-Anbarda qalıq Miqdar-7. Qiymət15; Tarix- 5 Dekabr. Alış Miqdar-4 Qiymət 20; Tarix- 8 Dekabr. Alış Miqdar-2 Qiymət 21; Tarix- 25 Dekabr. satıldı. Miqdar-8 Qiymət 30",
    "options": [
      "123",
      "122",
      "124",
      "126",
      "125"
    ],
    "correct": "125"
  },
  {
    "num": 17,
    "question": "Şirkət mal-material ehtiyatlarının maya dəyərini FIFO metodunu tətbiq etməklə qiymətləndirir. 1 Yanvar tarixində şirkətin mal-material ehtiyatlarında hər biri 150 AZN olan 500 ədəd ehtiyatı var idi. 31 Dekabr bitən hesabat ili üçün aşağıdakı əməliyyatlar əsasında satılan malların maya dəyəri nə qədər olar? Alış 250 ədəd ehtiyat 160 AZN; Satış 300 ədəd ehtiyat 155AZN; Alış 300 ədəd ehtiyat 170AZN; Satış 100 ədəd ehtiyat 160 azn.",
    "options": [
      "110000",
      "80000",
      "166000",
      "106000",
      "60000"
    ],
    "correct": "60000"
  },
  {
    "num": 18,
    "question": "İlin əvvəlinə mal ehtiyatlarının dəyəri 10 000 AZN, dövr ərzində alışlar 60 000 AZN, dövrün sonuna mal ehtiyatlarının qalıq dəyəri 20 000 AZN təşkil etmişdir. Dövr ərzində qaytarılan alışın dəyəri isə 5000 AZN olarsa, SMMD nə qədər olar?",
    "options": [
      "50000",
      "2700",
      "45000",
      "40000",
      "35000"
    ],
    "correct": "45000"
  },
  {
    "num": 19,
    "question": "İlin əvvəlinə anbardakı malların ilkin qalığı 340 AZN-dir. İl ərzində 7260 AZN məbləğində alış, 9830 AZN-lik satış olmuşdur. İlin sonunda anbardakı qalıq 700 AZN-dir. Satılan malların maya dəyəri nə qədər olar?",
    "options": [
      "7950",
      "6500",
      "6950",
      "7200",
      "6900"
    ],
    "correct": "6900"
  },
  {
    "num": 20,
    "question": "İlin əvvəlinə anbardakı malların ilkin qalığı 1200 AZN-dir. İl ərzində 10 570 AZN məbləğində alışlar və 11 300 AZN-lik satışlar olmuşdur. İlin sonunda anbardakı qalıq 2800 AZN-dir. Satılan malların maya dəyəri nə qədər olar?",
    "options": [
      "11300",
      "12570",
      "8970",
      "12300",
      "8900"
    ],
    "correct": "8970"
  },
  {
    "num": 21,
    "question": "Müəssisə alıcıya 5000 manata mal satmış, alıcı isə ödənişin yalnız 2000 manatını öəmişdir.Müəssisə nə qədər gəlir tanımalıdır?",
    "options": [
      "7000",
      "3000",
      "5000",
      "2000",
      "0"
    ],
    "correct": "5000"
  },
  {
    "num": 22,
    "question": "Yeni yaradılmış müəssisə üç mal dəstini əldə etmişdir. Birinci mal dəstinin maya dəyəri 120 manat, ikinci mal dəstinin maya dəyəri 130 manat, üçüncü mal dəstinin maya dəyəri isə 110 manat təşkil etmişdir. İki mal dəsti 285 manata satılmışdır. FİFO üsulundan istifadə etməklə satılmış mal dəstlərinin maya dəyərini müəyyən edin:",
    "options": [
      "240 manat",
      "260 manat",
      "230 manat",
      "250 manat",
      "280 manat"
    ],
    "correct": "250 manat"
  },
  {
    "num": 23,
    "question": "Ticarət müəssisəsində ehtiyatlar hesabının ilkin qalığı 4000 manatdır. Dövr ərzində 7000 manat dəyərində mal alınmış və maya dəyəri 8000 manat olan mal satılmışdır. Dövrün sonuna hesabın qalığını hesablayın.",
    "options": [
      "2500",
      "3500",
      "3000",
      "1500",
      "2000"
    ],
    "correct": "3000"
  },
  {
    "num": 24,
    "question": "Ticarət müəssisəsində ehtiyatlar hesabının ilkin qalığı 9000 manatdır. Dövr ərzində 10000 manat dəyərində mal alınmış və maya dəyəri 13000 manat olan mal satılmışdır. Dövrün sonuna hesabın qalığını hesablayın.",
    "options": [
      "11000",
      "11100",
      "10000",
      "6000",
      "9000"
    ],
    "correct": "6000"
  },
  {
    "num": 25,
    "question": "Materialların satışı ilə fəaliyyət göstərən \"Qaya\"MMC şirkəti dörd partiya mal tədarük edir. Birinci partiyanın dəyəri 250 manat, ikinci partiyanın – 300 manat, üçüncü partiya 620 manat və dördüncü partiya 750 man təşkil edir. Dörd partiya mal 3600 manata satılır. FİFO metodunun köməyilə dövr üzrə ümumi gəlir nə qədərdir?",
    "options": [
      "1890",
      "1760",
      "1990",
      "1680",
      "1650"
    ],
    "correct": "1680"
  },
  {
    "num": 26,
    "question": "Ehtiyatların satışı ilə fəaliyyət göstərən \"Səma\"MMC müəssisəsi dörd partiya mal tədarük edir. Birinci partiyanın dəyəri 520 manat, ikinci partiyanın – 630 manat, üçüncü partiya 800 manat və dördüncü partiya 1025 man təşkil edir. Dörd partiya mal 3600 manata satılır. FİFO metodunun köməyilə dövr üzrə ümumi gəlir nə qədərdir?",
    "options": [
      "500",
      "756",
      "530",
      "625",
      "250"
    ],
    "correct": "625"
  },
  {
    "num": 27,
    "question": "Yeni yaradılan müəssisə üç partiya mal tədarük edir.Birinci partiyanın dəyəri 50 manat ,ikinci partiyanın 85manat, üçüncü partiyanın isə 75 manat təşkil edir. İki partiya mal 190 manata satılır. FİFO metodunun köməyi ilə dövr üzrə ümumi gəlir nə qədərdir?",
    "options": [
      "175 manat",
      "60 manat",
      "70 manat",
      "55 manat",
      "85 manat"
    ],
    "correct": "55 manat"
  },
  {
    "num": 28,
    "question": "Müəssisənin ehtiyat alışı aşağıdakı kimi olmuşdur:13.07.2024 .100 ədəd x 2.50 azn =250 18.07.2024 150 ədəd x 2.70 azn = 405 26.07.2024 180 ədəd x 5 azn = 900 28.07.2024tarixində 300 ədəd ehtiyat satılmışdır.Satılan ehtiyatların maya dəyərini AVCO metodu ilə hesablayın.",
    "options": [
      "950",
      "896",
      "876",
      "1084.5",
      "870"
    ],
    "correct": "1084.5"
  },
  {
    "num": 29,
    "question": "Müəssisənin ehtiyat alışı aşağıdakı kimi olmuşdur: 13.07.2024 .100 ədəd x 2.50 azn =250 18.07.2024 150 ədəd x 2.70 azn = 405. 26.07.2024 180 ədəd x 5 azn = 900 28.07.2024tarixində 300 ədəd ehtiyat satılmışdır. Satılan ehtiyatların maya dəyərini FİFO metodu ilə hesablayın.",
    "options": [
      "870",
      "950",
      "876",
      "905",
      "896"
    ],
    "correct": "905"
  },
  {
    "num": 30,
    "question": "Müəssisənin ehtiyat alışı olmuşdur: 13.07.2024 .80 ədəd x 2 azn=160 18.07.2024 95 ədəd x 2.40 azn=228 26.07.2024 100 ədəd x 2.60 azn=260 28.07.24 tarixində 200 ədəd ehtiyat satılmışdır.Satılan ehtiyatların maya dəyərini FİFO metodu ilə hesablayın.",
    "options": [
      "450",
      "427",
      "407",
      "453",
      "402"
    ],
    "correct": "453"
  },
  {
    "num": 31,
    "question": "Müəssisənin ehtiyat alışı aşağıdakı kimi olmuşdur:13.07.2014 .800 ədəd x 2 azn=1600 18.07.2014 950 ədəd x 2.40 azn=2280 26.07.2014 1000 ədəd x 2.60 azn=2600 28.07.14 tarixində 2000 ədəd ehtiyat satılmışdır. Satılan ehtiyatların maya dəyərini FİFO metodu ilə hesablayın.",
    "options": [
      "4207",
      "4072",
      "4530",
      "4027",
      "4270"
    ],
    "correct": "4530"
  },
  {
    "num": 32,
    "question": "Verilmiş məlumatlar əsasında FIFO metodu ilə şirkətin anbar qalığını hesabla. 2 Dekabr-Anbarda qalıq Miqdar-8. Qiymət15; Tarix- 5 Dekabr. Alış Miqdar-4 Qiymət20; Tarix- 8 Dekabr. Alış Miqdar-2 Qiymət 21; Tarix- 25 Dekabr. satıldı. Miqdar-8 Qiymət 30",
    "options": [
      "123",
      "122",
      "126",
      "124",
      "125"
    ],
    "correct": "122"
  },
  {
    "num": 33,
    "question": "IFRS 15-ə əsasən şirkət müştəriyə 120,000 AZN-ə avadanlıq satır və bu qiymətə 2 illik pulsuz texniki xidmət daxildir. Həmin avadanlıq təklikdə 100,000 AZN-ə, 2 illik xidmət isə təklikdə 20,000 AZN-ə satılır. Müqavilə bağlandığı gün müəssisə nə qədər gəlir (Revenue) tanımalıdır?",
    "options": [
      "120000 AZN",
      "20000 AZN",
      "60000 AZN",
      "40000 AZN",
      "100000 AZN"
    ],
    "correct": "100000 AZN"
  },
  {
    "num": 34,
    "question": "Müəssisənin 500000 AZN ilkin dəyəri və 100000 AZN toplammış amortizasiyası olan binası var. Binanın xalis satış qiyməti 370000 AZN, istifadə dəyəri isə 390000 AZN-dir. Qeyd olunan bina üçün tanınmalı qiymətdəndüşmə zərəri neçə AZN-dir?",
    "options": [
      "200000",
      "10000",
      "100000",
      "30000",
      "130000"
    ],
    "correct": "10000"
  },
  {
    "num": 35,
    "question": "Aktivin balans dəyəri 80000 AZN, bərpa olunan məbləği isə 65000 AZN müəyyən edilmişdir. MUBS 36-ya əsasən mənfəət və ya zərər haqqında hesabatda nə qədər qiymətdəndüşmə zərəri tanınmalıdır?",
    "options": [
      "0",
      "145000",
      "15000",
      "25000",
      "80000"
    ],
    "correct": "15000"
  },
  {
    "num": 36,
    "question": "Aktivin balans dəyəri 60000 AZN, bərpa olunan məbləği isə 70000 AZN-dir. Müəssisə maliyyə hesabatlarında hansı düzəlişi etməlidir?",
    "options": [
      "13000 AZN xərc tanınır",
      "10000 AZN qiymətdəndüşmə zərəri tanınır",
      "heç bir qiymətdən düşmə zərəri tanınmır",
      "13000 AZN mənfəət tanınır",
      "Aktivin balans dəyəri 70000 AZN-ə qaldırılır"
    ],
    "correct": "heç bir qiymətdən düşmə zərəri tanınmır"
  },
  {
    "num": 37,
    "question": "Müəssisə avadanlığını 50000 AZN-ə sata bilər, satış xərcləri isə 3000$ AZN təşkil edir. Aktivin xalis satış qiyməti neçə AZN-dir?",
    "options": [
      "0",
      "53000",
      "50000",
      "47000",
      "3000"
    ],
    "correct": "47000"
  },
  {
    "num": 38,
    "question": "Aktivin balans dəyəri 120000 AZN, bərpa olunan məbləği isə 95000 AZN olaraq müəyyən edilmişdir. Tanınmalı olan qiymətdəndüşmə zərəri nə qədərdir? Aktivin balans dəyəri 120000 AZN, bərpa olunan məbləği isə 95000 AZN olaraq müəyyən edilmişdir. Tanınmalı olan qiymətdəndüşmə zərəri nə qədərdir?",
    "options": [
      "120000",
      "0",
      "215000",
      "25000",
      "95000"
    ],
    "correct": "25000"
  },
  {
    "num": 39,
    "question": "Aktivin balans dəyəri 100000 AZN, xalis satış qiyməti 80000 AZN, istifadə dəyəri isə 90000 AZN-dir. MUBS 36-ya əsasən aktivin bərpa olunan məbləği nə qədərdir?",
    "options": [
      "100000",
      "10000",
      "20000",
      "90000",
      "80000"
    ],
    "correct": "90000"
  },
  {
    "num": 40,
    "question": "31 dekabr 2025-ci ildə anbardaki bəzi ehtiyatları mənəvi aşındığını aşkar edir. 8000 AZN dəyərində olan ehtiyatın bazarda 500 AZN satış xərci çəkdikdən sonra 7000 AZN-ə satılacağı ehtimal edilir. 31 dekabr2025-ci il tarixli MZHH-da xərc kimi hanslı dəyərdə əks etdiriləcəkdir?",
    "options": [
      "Debet Xərc 700 Kredit Ehtiyatlar 700",
      "Debet Xərc 1500 Kredit Ehtiyatlar 1500",
      "Debet Xərc 500 Kredit Ehtiyatlar 500",
      "Debet Xərc 7000 Kredit Ehtiyatlar 7000",
      "Debet Xərc 8000 Kredit Ehtiyatlar 8000"
    ],
    "correct": "Debet Xərc 1500 Kredit Ehtiyatlar 1500"
  },
  {
    "num": 41,
    "question": "31 dekabr 2025-ci ildə anbardaki bəzi ehtiyatları mənəvi aşındığını aşkar edir. 8000 AZN dəyərində olan ehtiyatın bazarda 500 AZN satış xərci çəkdikdən sonra 7000 AZN-ə satılacağı ehtimal edilir. 31 dekabr2025-ci il tarixli MVHH-da ehtiyatlar hanslı dəyərdə əks etdiriləcəkdir?",
    "options": [
      "7000",
      "1500",
      "8000",
      "500",
      "6500"
    ],
    "correct": "6500"
  },
  {
    "num": 42,
    "question": "Müəssisə istehsal zavodunun tikintisinə 1 yanvar tarixində başlamışdır. Tikintinin tamamlanması 18 ay çəkəcək. Layihə üçün 2 000 000 manat xüsusi borc cəlb edilmiş və illik faiz dərəcəsi 9% olmuşdur. Tikinti il ərzində 12 ay davam etmişdir.Birinci il üçün kapitallaşdırılacaq borclanma məsrəfi nə qədərdir?",
    "options": [
      "180 000 manat",
      "90 000 manat",
      "200 000 manat",
      "2 000 000 manat",
      "360 000 manat"
    ],
    "correct": "180 000 manat"
  },
  {
    "num": 43,
    "question": "Müəssisə hesabat ilində 250 000 manat dövlət yardımı almışdır. Bunun 150 000 manatı avadanlığın alınmasına, 100 000 manatı isə əmək xərclərinin kompensasiyasına aiddir. Açıqlanmalı dövlət yardımının ümumi məbləği nə qədərdir?",
    "options": [
      "150 000 manat",
      "0 manat",
      "50 000 manat",
      "250 000 manat",
      "100 000 manat"
    ],
    "correct": "250 000 manat"
  },
  {
    "num": 44,
    "question": "Müəssisə 120 000 manat dövlət subsidiyasını təxirə salınmış gəlir kimi uçota almışdır. Subsidiyanın 3 il ərzində hər il 40 000 manat gəlir kimi tanınması nəzərdə tutulmuşdur. İlk iki ildə 80 000 manat gəlir tanınmışdır. Üçüncü ilin əvvəlində subsidiya tam geri qaytarılmalıdır. Üçüncü ildə geri qaytarılmanın mənfəət və zərərə təsiri nə qədərdir?",
    "options": [
      "Təsir yoxdur",
      "40 000 manat gəlir",
      "80 000 manat xərc",
      "40 000 manat xərc",
      "120 000 manat xərc"
    ],
    "correct": "80 000 manat xərc"
  },
  {
    "num": 45,
    "question": "Müəssisəyə dövlət tərəfindən 300 000 manat subsidiya vəd edilmişdir. Subsidiyanın alınması müəyyən ekoloji göstəricinin yerinə yetirilməsindən asılıdır. Hesabat tarixində müəssisə şərtin yerinə yetiriləcəyinə dair kifayət qədər əsaslı əminliyə malikdir.Tanınacaq subsidiya məbləği nə qədərdir?",
    "options": [
      "0 manat",
      "150 000 manat",
      "300 000 manat",
      "600 000 manat",
      "30 000 manat"
    ],
    "correct": "300 000 manat"
  },
  {
    "num": 46,
    "question": "Müəssisəyə dövlət tərəfindən 2 il müddətinə faizsiz 200 000 manat kredit verilmişdir. Bazar faiz dərəcəsi 10% təşkil edir. Kreditin ilkin ədalətli dəyəri 165 289 manat hesablanmışdır. Dövlət yardımının məbləği nə qədərdir?",
    "options": [
      "20 000 manat",
      "200 000 manat",
      "35 000 manat",
      "165 289 manat",
      "34 711 manat"
    ],
    "correct": "34 711 manat"
  },
  {
    "num": 47,
    "question": "Müəssisə dövlət tərəfindən işçilərin peşə hazırlığı xərclərinin kompensasiyası üçün 60 000 manat subsidiya almışdır. Vəsait 3 il ərzində çəkiləcək uyğun təlim xərclərinə aid edilməlidir. Müəssisə birinci ildə 20 000 manat uyğun xərc çəkmişdir.Birinci ildə mənfəət və zərərdə tanınacaq subsidiya gəliri nə qədərdir?",
    "options": [
      "10 000 manat",
      "60 000 manat",
      "40 000 manat",
      "20 000 manat",
      "30 000 manat"
    ],
    "correct": "20 000 manat"
  },
  {
    "num": 48,
    "question": "Müəssisə 900 000 manat dəyərində istehsal xətti almışdır. Dövlət 180 000 manat subsidiya vermişdir. Müəssisə subsidiyanı aktivin balans dəyərindən çıxır. Aktivin faydalı istifadə müddəti 12 il, qalıq dəyəri sıfırdır.İllik amortizasiya xərci nə qədər olacaq?",
    "options": [
      "75 000 manat",
      "72 000 manat",
      "45 000 manat",
      "90 000 manat",
      "60 000 manat"
    ],
    "correct": "60 000 manat"
  },
  {
    "num": 49,
    "question": "Müəssisə 500 000 manat dəyərində aktiv əldə etmiş və 100 000 manat dövlət subsidiyasını aktivin balans dəyərindən çıxmışdır. Aktivin faydalı istifadə müddəti 10 il, qalıq dəyəri sıfırdır. Bir il sonra subsidiya geri qaytarılmalıdır.Subsidiyanın geri qaytarılması zamanı aktivin balans dəyərinə əlavə ediləcək subsidiya məbləği nə qədərdir?",
    "options": [
      "90 000 manat",
      "10 000 manat",
      "50 000 manat",
      "100 000 manat",
      "80 000 manat"
    ],
    "correct": "100 000 manat"
  },
  {
    "num": 50,
    "question": "Müəssisə 400 000 manat dəyərində avadanlıq əldə etmiş və bununla əlaqədar 80 000 manat dövlət subsidiyası almışdır. Subsidiyanın təxirə salınmış gəlir kimi uçota alınması seçilmişdir. Avadanlığın faydalı istifadə müddəti 8 ildir. Birinci ildə mənfəət və zərərdə subsidiyadan tanınacaq gəlir nə qədərdir?",
    "options": [
      "40 000 manat",
      "80 000 manat",
      "20 000 manat",
      "8 000 manat",
      "10 000 manat"
    ],
    "correct": "10 000 manat"
  },
  {
    "num": 51,
    "question": "Müəssisə istehsal avadanlığını 600 000 manat dəyərində əldə etmişdir. Avadanlığın alınması ilə əlaqədar dövlət tərəfindən 120 000 manat subsidiya verilmişdir. Müəssisə subsidiyanı aktivin balans dəyərindən çıxır. Avadanlığın faydalı istifadə müddəti 8 il, qalıq dəyəri sıfırdır.Birinci ilin sonunda avadanlığın balans dəyəri nə qədər olacaq?",
    "options": [
      "420 000 manat",
      "450 000 manat",
      "480 000 manat",
      "525 000 manat",
      "540 000 manat"
    ],
    "correct": "420 000 manat"
  },
  {
    "num": 52,
    "question": "Müəssisə 180 000 manat dəyərində avadanlıq almışdır. Faydalı istifadə müddəti 6 il, qalıq dəyəri sıfırdır.4 ildən sonra yığılmış amortizasiyanı müəyyən edin.",
    "options": [
      "60 000 manat",
      "120 000 manat",
      "100 000 manat",
      "150 000 manat",
      "90 000 manat"
    ],
    "correct": "120 000 manat"
  },
  {
    "num": 53,
    "question": "Müəssisə 250 000 manat ilkin dəyəri olan investisiya mülkiyyətini ədalətli dəyər modeli ilə uçota alır. İl sonunda ədalətli dəyər 280 000 manat olmuşdur.İl sonunda maliyyə vəziyyəti hesabatında göstəriləcək məbləği müəyyən edin.",
    "options": [
      "250 000 manat",
      "280 000 manat",
      "275 000 manat",
      "260 000 manat",
      "30 000 manat"
    ],
    "correct": "280 000 manat"
  },
  {
    "num": 54,
    "question": "Müəssisə 400 000 manata bina almışdır. Əmlakın alınması ilə əlaqədar 15 000 manat hüquqi xidmət və 10 000 manat qeydiyyat xərci çəkilmişdir.İnvestisiya mülkiyyətinin ilkin dəyərini müəyyən edin.",
    "options": [
      "400 000 manat",
      "425 000 manat",
      "410 000 manat",
      "430 000 manat",
      "415 000 manat"
    ],
    "correct": "425 000 manat"
  },
  {
    "num": 55,
    "question": "Müəssisə 600 000 manata investisiya mülkiyyəti əldə etmişdir. Hesabat dövrünün sonunda onun ədalətli dəyəri 570 000 manat olmuşdur.IAS 40-a əsasən tanınacaq nəticəni müəyyən edin.",
    "options": [
      "30 000 manat mənfəət",
      "30 000 manat zərər",
      "600 000 manat xərc",
      "15 000 manat zərər",
      "570 000 manat zərər"
    ],
    "correct": "30 000 manat zərər"
  },
  {
    "num": 56,
    "question": "Müəssisə 500 000 manata investisiya mülkiyyəti əldə etmişdir. İl sonunda həmin əmlakın ədalətli dəyəri 550 000 manat olmuşdur.IAS 40-a əsasən ədalətli dəyər modelindən istifadə edilərsə, mənfəət və zərərdə tanınacaq məbləği müəyyən edin.",
    "options": [
      "50 000 manat zərər",
      "50 000 manat mənfəət",
      "500 000 manat xərc",
      "25 000 manat mənfəət",
      "550 000 manat mənfəət"
    ],
    "correct": "50 000 manat mənfəət"
  },
  {
    "num": 57,
    "question": "Müəssisə 120 000 manat dəyərində qeyri-maddi aktiv əldə etmişdir. Aktivin faydalı istifadə müddəti 8 il, qalıq dəyəri 8 000 manatdır.İllik amortizasiya məbləğini hesablayın.",
    "options": [
      "15 000 manat",
      "14 000 manat",
      "16 000 manat",
      "12 000 manat",
      "13 000 manat"
    ],
    "correct": "14 000 manat"
  },
  {
    "num": 58,
    "question": "Müəssisə proqram təminatının hazırlanması mərhələsində 40 000 manat xərc çəkmişdir. Proqramın hazırlanması başa çatdıqdan sonra onun istifadəyə verilməsi üçün əlavə 10 000 manat xərc edilmişdir.Kapitalaşdırılan ümumi məbləği müəyyən edin.",
    "options": [
      "40 000 manat",
      "50 000 manat",
      "30 000 manat",
      "60 000 manat",
      "10 000 manat"
    ],
    "correct": "50 000 manat"
  },
  {
    "num": 59,
    "question": "Müəssisə 90 000 manat dəyərində patent əldə etmişdir. Patentin faydalı istifadə müddəti 10 ildir və qalıq dəyəri yoxdur.3 ildən sonra patentin balans dəyəri nə qədər olacaq?",
    "options": [
      "60 000 manat",
      "63 000 manat",
      "72 000 manat",
      "66 000 manat",
      "70 000 manat"
    ],
    "correct": "63 000 manat"
  },
  {
    "num": 60,
    "question": "Müəssisə patent əldə etmək üçün 50 000 manat ödəmişdir. Patentin qeydiyyatı üçün 5 000 manat, hüquqşünas xidmətləri üçün 3 000 manat xərc çəkilmişdir.IAS 38-ə əsasən qeyri-maddi aktivin ilkin dəyərini müəyyən edin.",
    "options": [
      "50 000 manat",
      "58 000 manat",
      "53 000 manat",
      "60 000 manat",
      "55 000 manat"
    ],
    "correct": "58 000 manat"
  },
  {
    "num": 61,
    "question": "Müəssisə 250 000 manat ilkin dəyəri olan binanı əldə etmişdir. Binanın faydalı istifadə müddəti 25 il, qalıq dəyəri 25 000 manatdır. İllik amortizasiya məbləğini müəyyən edin.",
    "options": [
      "10 000 manat",
      "9 000 manat",
      "11 000 manat",
      "12 500 manat",
      "8 000 manat"
    ],
    "correct": "9 000 manat"
  },
  {
    "num": 62,
    "question": "Müəssisə 100 000 manat dəyərində avadanlıq almışdır. Faydalı istifadə müddəti 5 il, qalıq dəyəri sıfırdır. Düzxətli amortizasiya metodundan istifadə edilir. 2 ildən sonra avadanlığın balans dəyəri nə qədər olacaq?",
    "options": [
      "40 000 manat",
      "60 000 manat",
      "80 000 manat",
      "70 000 manat",
      "50 000 manat"
    ],
    "correct": "60 000 manat"
  },
  {
    "num": 63,
    "question": "Müəssisə 300 000 manat ilkin dəyəri olan binanı yenidən qiymətləndirmişdir. Yenidən qiymətləndirmə tarixində binanın balans dəyəri 240 000 manat, ədalətli dəyəri isə 270 000 manat olmuşdur.Yenidən qiymətləndirmədən yaranan artımı müəyyən edin.",
    "options": [
      "30 000 manat",
      "20 000 manat",
      "60 000 manat",
      "270 000 manat",
      "240 000 manat"
    ],
    "correct": "30 000 manat"
  },
  {
    "num": 64,
    "question": "Müəssisə 80 000 manata avadanlıq almışdır. Daşınma xərcləri 3 000 manat, quraşdırma xərcləri 7 000 manat təşkil etmişdir. Avadanlığın alınması ilə əlaqədar işçilərə keçirilən təlim üçün 2 000 manat xərc çəkilmişdir. Aktivin ilkin dəyərini hesablayın.",
    "options": [
      "87 000 manat",
      "92 000 manat",
      "80 000 manat",
      "90 000 manat",
      "85 000 manat"
    ],
    "correct": "90 000 manat"
  },
  {
    "num": 65,
    "question": "Müəssisə balans dəyəri 100 000 manat olan avadanlığı yeni avadanlıqla dəyişdirmişdir. Yeni avadanlığın ədalətli dəyəri 150 000 manat, verilmiş köhnə avadanlığın ədalətli dəyəri isə 110 000 manatdır. Müəssisə əlavə olaraq 40 000 manat pul ödəmişdir. Əməliyyatın kommersiya mahiyyəti vardır.Yeni aktivin ilkin dəyərini müəyyən edin.",
    "options": [
      "140 000 manat",
      "150 000 manat",
      "100 000 manat",
      "160 000 manat",
      "110 000 manat"
    ],
    "correct": "150 000 manat"
  },
  {
    "num": 66,
    "question": "Avadanlığın balans dəyəri 320 000 manatdır. Yenidən qiymətləndirmə nəticəsində onun ədalətli dəyəri 380 000 manat müəyyən edilmişdir. Əvvəlki illərdə həmin aktiv üzrə 25 000 manat yenidən qiymətləndirmədən yaranan azalma mənfəət və zərərdə xərc kimi tanınmışdır.Cari dövrdə mənfəət və zərərdə tanınacaq məbləği müəyyən edin.",
    "options": [
      "60 000 manat mənfəət",
      "25 000 manat mənfəət",
      "0 manat",
      "85 000 manat mənfəət",
      "35 000 manat mənfəət Cavab açarı 1-D | 2-A | 3-C | 4-C | 5-D | 6-C | 7-E | 8-C | 9-D | 10-D | 11-D | 12-C | 13-E | 14-D | 15-D | 16-E | 17-E | 18-C | 19-E | 20-C | 21-C | 22-D | 23-C | 24-D | 25-D | 26-D | 27-D | 28-D | 29-D | 30-D | 31-C | 32-B | 33-E | 34-B | 35-C | 36-C | 37-D | 38-D | 39-D | 40-B | 41-E | 42-A | 43-D | 44-C | 45-C | 46-E | 47-D | 48-E | 49-D | 50-E | 51-A | 52-B | 53-B | 54-B | 55-B | 56-B | 57-B | 58-B | 59-B | 60-B | 61-B | 62-B | 63-A | 64-D | 65-B | 66-B MH_2 – Suallar və cavablar (67–142) Düzgün cavablar ✓ ilə işarələnib. Hər sualın altında qısa izah verilib. Cavab açarı 67: B      68: B     69: B      70: B     71: B      72: B     73: B    74: B    75: B    76: D 77: E      78: A     79: D      80: D     81: D      82: D     83: C    84: D    85: E    86: D 87: D      88: D     89: D      90: C     91: C      92: D     93: B    94: D    95: B    96: A 97: A      98: D     99: C     100: D     101: C    102: E     103: E   104: E   105: C   106: C 107: E    108: B     109: B    110: B     111: E    112: B     113: B   114: E   115: E   116: D 117: B    118: E     119: E    120: D     121: D    122: D     123: B   124: B   125: D   126: B 127: D    128: B     129: C    130: D     131: D    132: D     133: D   134: D   135: E   136: D 137: A    138: E     139: B    140: D     141: B    142: B"
    ],
    "correct": "25 000 manat mənfəət"
  },
  {
    "num": 67,
    "question": "Müəssisənin öz istifadəsində olan binasının transfer tarixində balans dəyəri 600 000 manatdır. Bina investisiya mülkiyyətinə keçirilir və həmin tarixdə ədalətli dəyəri 680 000 manatdır. Transferdən yaranan artımın məbləğini müəyyən edin.",
    "options": [
      "680 000 manat",
      "80 000 manat",
      "40 000 manat",
      "20 000 manat",
      "600 000 manat"
    ],
    "correct": "80 000 manat"
  },
  {
    "num": 68,
    "question": "Müəssisə ədalətli dəyər modeli ilə uçota aldığı investisiya mülkiyyətini öz istifadəsinə keçirmişdir. Transfer tarixində investisiya mülkiyyətinin balans dəyəri 900 000 manat, ədalətli dəyəri isə 950 000 manatdır. IAS 16 üzrə transfer zamanı əsas vəsaitin ilkin dəyəri kimi hansı məbləğ qəbul ediləcək?",
    "options": [
      "900 000 manat",
      "950 000 manat",
      "850 000 manat",
      "1 000 000 manat",
      "50 000 manat"
    ],
    "correct": "950 000 manat"
  },
  {
    "num": 69,
    "question": "Müəssisə investisiya məqsədilə binanı 800 000 manata almışdır. İlkin alışla bağlı 20 000 manat birbaşa əməliyyat xərci çəkilmişdir. İl sonunda binanın ədalətli dəyəri 870 000 manat olmuşdur. Ədalətli dəyər modelindən istifadə edilirsə, il sonunda mənfəət və zərərdə tanınacaq ümumi mənfəəti müəyyən edin.",
    "options": [
      "70 000 manat",
      "50 000 manat",
      "20 000 manat",
      "80 000 manat",
      "90 000 manat"
    ],
    "correct": "50 000 manat"
  },
  {
    "num": 70,
    "question": "Müəssisə yeni proqram təminatı hazırlamaq üçün 120 000 manat tədqiqat xərci çəkmişdir. İnkişaf mərhələsində isə 200 000 manat xərc çəkilmişdir. İnkişaf mərhələsində aktivin tanınması meyarlarının yerinə yetirildiyi sübut edilmişdir. Maliyyə vəziyyəti hesabatında qeyri- maddi aktiv kimi tanınacaq məbləği müəyyən edin.",
    "options": [
      "320 000 manat",
      "200 000 manat",
      "80 000 manat",
      "0 manat",
      "120 000 manat"
    ],
    "correct": "200 000 manat"
  },
  {
    "num": 71,
    "question": "Müəssisə 180 000 manata patent əldə etmişdir. Patentin faydalı istifadə müddəti 6 ildir. Qalıq dəyəri sıfırdır. 2 il istifadə edildikdən sonra patentin qalan faydalı istifadə müddəti 3 il olaraq yenidən müəyyən edilmişdir. Yenidən qiymətləndirmə tarixindən sonrakı illik amortizasiya məbləği nə qədərdir?",
    "options": [
      "30 000 manat",
      "40 000 manat",
      "36 000 manat",
      "45 000 manat",
      "20 000 manat"
    ],
    "correct": "40 000 manat"
  },
  {
    "num": 72,
    "question": "Müəssisənin avadanlığının ilkin dəyəri 500 000 manatdır. Bu məbləğin 100 000 manatı 5 ildən bir dəyişdirilməli olan mühərrikə aiddir. Qalan hissənin faydalı istifadə müddəti 10 ildir. 5-ci ilin sonunda mühərrik 130 000 manata yenisi ilə əvəz edilmişdir. Yeni mühərrikin kapitallaşdırılmalı məbləği nə qədərdir?",
    "options": [
      "100 000 manat",
      "130 000 manat",
      "500 000 manat",
      "400 000 manat",
      "30 000 manat"
    ],
    "correct": "130 000 manat"
  },
  {
    "num": 73,
    "question": "Müəssisə 600 000 manata bina əldə etmişdir. Binanın ümumi faydalı istifadə müddəti 30 ildir. Bu məbləğin 120 000 manatı dam örtüyünə, 480 000 manatı binanın əsas konstruksiyasına aiddir. Dam örtüyünün faydalı istifadə müddəti 10 il, əsas konstruksiyanın isə 30 ildir. Qalıq dəyər sıfırdır. İllik amortizasiya məbləğini müəyyən edin.",
    "options": [
      "20 000 manat",
      "28 000 manat",
      "30 000 manat",
      "26 000 manat",
      "24 000 manat"
    ],
    "correct": "28 000 manat"
  },
  {
    "num": 74,
    "question": "Müəssisə 240 000 manatlıq avadanlıq almışdır. Faydalı istifadə müddəti əvvəlcə 8 il müəyyən edilmiş və qalıq dəyər sıfır qəbul edilmişdir. Aktiv 3 il istifadə edildikdən sonra onun balans dəyəri 150 000 manat olmuşdur. Həmin tarixdə qalan faydalı istifadə müddəti yenidən qiymətləndirilərək 5 il müəyyən edilmişdir. Yeni illik amortizasiya məbləğini hesablayın.",
    "options": [
      "25 000 manat",
      "30 000 manat",
      "40 000 manat",
      "20 000 manat",
      "37 500 manat"
    ],
    "correct": "30 000 manat"
  },
  {
    "num": 75,
    "question": "Aktivin balans dəyəri 180 000 manatdır. Əvvəlki dövrdə 30 000 manat qiymətdən düşmə zərəri tanınmışdır. Cari dövrdə aktivin bərpa olunan məbləği 165 000 manat olmuşdur. Əgər qiymətdən düşmə baş verməsəydi, aktivin cari balans dəyəri 175 000 manat olacaqdı. Cari dövrdə tanınacaq qiymətdən düşmə zərərinin bərpasını müəyyən edin.",
    "options": [
      "30 000 manat",
      "15 000 manat",
      "25 000 manat",
      "5 000 manat",
      "10 000 manat"
    ],
    "correct": "15 000 manat"
  },
  {
    "num": 76,
    "question": "Müəssisənin avadanlığının balans dəyəri 250 000 manatdır. Aktivin istifadə dəyəri 210 000 manat, satış xərcləri çıxılmaqla ədalətli dəyəri isə 225 000 manatdır. IAS 36 ilə əlaqəli olaraq aktiv üzrə tanınmalı qiymətdən düşmə zərərini müəyyən edin.",
    "options": [
      "15 000 manat",
      "0 manat",
      "210 000 manat",
      "25 000 manat",
      "40 000 manat"
    ],
    "correct": "25 000 manat"
  },
  {
    "num": 77,
    "question": "Müəssisənin avadanlığının ilkin dəyəri 300 000 manat, yığılmış amortizasiyası 180 000 manatdır. Müəssisə avadanlığı 135 000 manata satmışdır. Satışla bağlı 5 000 manat xərc çəkilmişdir. Satış nəticəsində yaranan mənfəət və ya zərəri müəyyən edin.",
    "options": [
      "5 000 manat mənfəət",
      "15 000 manat zərər",
      "15 000 manat mənfəət",
      "10 000 manat zərər",
      "10 000 manat mənfəət"
    ],
    "correct": "10 000 manat mənfəət"
  },
  {
    "num": 78,
    "question": "Müəssisə 1 yanvar 2022-ci ildə 400 000 manata avadanlıq almışdır. Faydalı istifadə müddəti 10 il, qalıq dəyəri sıfırdır. Düzxətli metod tətbiq edilir. 31 dekabr 2025-ci ildə avadanlığın balans dəyəri yenidən qiymətləndirilərək 250 000 manat müəyyən edilmişdir. Yenidən qiymətləndirmədən sonra qalan faydalı istifadə müddəti 6 il qəbul edilmişdir.2026-cı il üzrə amortizasiya xərcini müəyyən edin.",
    "options": [
      "41 666,67 manat",
      "25 000 manat",
      "40 000 manat",
      "50 000 manat",
      "37 500 manat"
    ],
    "correct": "41 666,67 manat"
  },
  {
    "num": 79,
    "question": "Müəssisə investisiya mülkiyyətini 700 000 manata əldə etmişdir. Birinci ilin sonunda ədalətli dəyər 750 000 manat olmuş, ikinci ilin sonunda isə 720 000 manata düşmüşdür. İki il üzrə ümumi olaraq mənfəət və ya zərərdə tanınmış xalis nəticəni müəyyən edin.",
    "options": [
      "30 000 manat zərər",
      "70 000 manat mənfəət",
      "20 000 manat zərər",
      "20 000 manat mənfəət",
      "50 000 manat mənfəət"
    ],
    "correct": "20 000 manat mənfəət"
  },
  {
    "num": 80,
    "question": "Müəssisə 160 000 manat dəyərində proqram təminatı əldə etmişdir. Faydalı istifadə müddəti 8 il, qalıq dəyəri sıfırdır.5 ildən sonra proqram təminatının balans dəyəri nə qədər olacaq?",
    "options": [
      "50 000 manat",
      "80 000 manat",
      "100 000 manat",
      "60 000 manat",
      "40 000 manat"
    ],
    "correct": "60 000 manat"
  },
  {
    "num": 81,
    "question": "Müəssisə 350 000 manat ilkin dəyəri olan binanı yenidən qiymətləndirmişdir. Yenidən qiymətləndirmə tarixində yığılmış amortizasiya 70 000 manat, binanın ədalətli dəyəri isə 320 000 manatdır. Yenidən qiymətləndirmə nəticəsində yaranan artımı müəyyən edin.",
    "options": [
      "30 000 manat",
      "70 000 manat",
      "320 000 manat",
      "40 000 manat",
      "20 000 manat"
    ],
    "correct": "40 000 manat"
  },
  {
    "num": 82,
    "question": "Müəssisə 200 000 manat dəyərində avadanlıq əldə etmişdir. Faydalı istifadə müddəti 8 il, qalıq dəyəri 40 000 manatdır.3 il istifadə edildikdən sonra avadanlığın balans dəyərini hesablayın.",
    "options": [
      "125 000 manat",
      "130 000 manat",
      "160 000 manat",
      "140 000 manat",
      "150 000 manat"
    ],
    "correct": "140 000 manat"
  },
  {
    "num": 83,
    "question": "Müəssisə yeni istehsal avadanlığı almışdır. Alış qiyməti 150 000 manat, gömrük rüsumu 10 000 manat, daşınma xərci 5 000 manat, işçilərin təlim xərci isə 4 000 manat təşkil etmişdir. IAS 16-ya əsasən avadanlığın ilkin dəyərini hesablayın.",
    "options": [
      "169 000 manat",
      "150 000 manat",
      "165 000 manat",
      "160 000 manat",
      "154 000 manat"
    ],
    "correct": "165 000 manat"
  },
  {
    "num": 84,
    "question": "Müəssisə 500 000 manat dəyərində investisiya mülkiyyətinə sahibdir. Ədalətli dəyər modeli tətbiq edilir. Birinci ilin sonunda ədalətli dəyər 530 000 manat, ikinci ilin sonunda isə 510 000 manat olmuşdur. İkinci ildə mənfəət və ya zərərdə tanınacaq nəticəni müəyyən edin.",
    "options": [
      "10 000 manat mənfəət",
      "20 000 manat mənfəət",
      "10 000 manat zərər",
      "20 000 manat zərər",
      "30 000 manat zərər"
    ],
    "correct": "20 000 manat zərər"
  },
  {
    "num": 85,
    "question": "Müəssisə 300 000 manat dəyərində binanı əldə etmişdir. Faydalı istifadə müddəti 15 il, qalıq dəyəri sıfırdır. 4 ildən sonra binanın balans dəyəri müəyyən edilir. Düzxətli metoddan istifadə etməklə balans dəyərini hesablayın.",
    "options": [
      "200 000 manat",
      "240 000 manat",
      "180 000 manat",
      "260 000 manat",
      "220 000 manat"
    ],
    "correct": "220 000 manat"
  },
  {
    "num": 86,
    "question": "Müəssisə 100 000 manat dəyərində patent almışdır. Faydalı istifadə müddəti 5 il, qalıq dəyəri sıfırdır.2 il istifadə edildikdən sonra patent satılmışdır. Satış tarixinə balans dəyəri nə qədərdir?",
    "options": [
      "20 000 manat",
      "40 000 manat",
      "50 000 manat",
      "60 000 manat",
      "80 000 manat"
    ],
    "correct": "60 000 manat"
  },
  {
    "num": 87,
    "question": "Müəssisə 240 000 manat dəyərində avadanlıq əldə etmişdir. Qalıq dəyəri 40 000 manat, faydalı istifadə müddəti 10 ildir.5 ildən sonra balans dəyəri nə qədər olacaq?",
    "options": [
      "150 000 manat",
      "120 000 manat",
      "100 000 manat",
      "140 000 manat",
      "160 000 manat"
    ],
    "correct": "140 000 manat"
  },
  {
    "num": 88,
    "question": "Müəssisə 150 000 manat ilkin dəyəri olan avadanlıq əldə etmişdir. Faydalı istifadə müddəti 10 il, qalıq dəyəri 10 000 manatdır. 3 ildən sonra avadanlığın balans dəyərini müəyyən edin.",
    "options": [
      "112 000 manat",
      "105 000 manat",
      "110 000 manat",
      "108 000 manat",
      "100 000 manat"
    ],
    "correct": "108 000 manat"
  },
  {
    "num": 89,
    "question": "Müəssisə 200 000 manat dəyərində bina əldə etmişdir. Binanın faydalı istifadə müddəti 20 il, qalıq dəyəri isə 20 000 manatdır. Düzxətli metodla illik amortizasiya məbləğini hesablayın.",
    "options": [
      "8 000 manat",
      "11 000 manat",
      "12 000 manat",
      "9 000 manat",
      "10 000 manat"
    ],
    "correct": "9 000 manat"
  },
  {
    "num": 90,
    "question": "Müəssisə avadanlığı 120 000 manata almışdır. Avadanlığın quraşdırılması üçün 8 000 manat, daşınması üçün 2 000 manat xərc çəkilmişdir. Avadanlığın istifadəyə hazırlanması üçün əlavə 5 000 manat xərc edilmişdir. Avadanlığın ilkin dəyərini müəyyən edin.",
    "options": [
      "120 000 manat",
      "140 000 manat",
      "135 000 manat",
      "128 000 manat",
      "130 000 manat"
    ],
    "correct": "135 000 manat"
  },
  {
    "num": 91,
    "question": "Müəssisə yeni istehsal müəssisəsinin tikintisinə 1 yanvar tarixində başlamışdır. İl ərzində tikintiyə 3 000 000 manat xərclənmişdir. Layihənin maliyyələşdirilməsi: 2 000 000 manat xüsusi borc — 9% və 1 000 000 manat ümumi borclanma — 8%. Tikinti il sonunda hələ başa çatmamışdır. Dövlət müəssisəyə layihə ilə bağlı 500 000 manat subsidiya vermişdir. Müəssisə subsidiyanı aktivin balans dəyərindən çıxır. İlin sonunda kapitallaşdırılmış borclanma məsrəfi də daxil olmaqla aktivin balans dəyəri nə qədər olacaq?",
    "options": [
      "2 680 000 manat",
      "3 260 000 manat",
      "2 760 000 manat",
      "2 500 000 manat",
      "3 000 000 manat"
    ],
    "correct": "2 760 000 manat"
  },
  {
    "num": 92,
    "question": "Müəssisə 2 400 000 manat xüsusi borc götürmüşdür. İllik faiz dərəcəsi 10%-dir. Tikinti 1 yanvarda başlamış, 1 iyul–30 sentyabr tarixlərində tam dayandırılmış və 1 oktyabrda yenidən başlamışdır. İl ərzində kapitallaşdırılmalı borclanma məsrəfi nə qədərdir?",
    "options": [
      "120 000 manat",
      "150 000 manat",
      "60 000 manat",
      "180 000 manat",
      "240 000 manat"
    ],
    "correct": "180 000 manat"
  },
  {
    "num": 93,
    "question": "Müəssisənin borcları: 1 000 000 manat — 7%; 2 000 000 manat — 9%; 2 000 000 manat — 11%. Kvalifikasiya olunan aktivə il ərzində 1 800 000 manat xərc çəkilmişdir. Orta çəkili borclanma dərəcəsi və kapitallaşdırılacaq məbləğ nə qədərdir?",
    "options": [
      "9,2% və 165 600 manat",
      "9,4% və 169 200 manat",
      "8,5% və 153 000 manat",
      "10% və 180 000 manat",
      "9% və 162 000 manat"
    ],
    "correct": "9,4% və 169 200 manat"
  },
  {
    "num": 94,
    "question": "Müəssisə tikinti üçün 1 200 000 manat xüsusi borc götürmüşdür. İllik faiz dərəcəsi 10%-dir. Tikinti 12 ay davam etmiş və il ərzində 1 200 000 manat tikinti xərci çəkilmişdir. İl ərzində 120 000 manat faiz kapitallaşdırılmışdır. Tikinti başa çatdıqdan sonra obyekt 1 500 000 manata satılmışdır. Satışdan yaranan mənfəət nə qədərdir?",
    "options": [
      "120 000 manat",
      "60 000 manat",
      "150 000 manat",
      "180 000 manat",
      "300 000 manat"
    ],
    "correct": "180 000 manat"
  },
  {
    "num": 95,
    "question": "Müəssisə tikinti üçün 5 000 000 manat xüsusi borc götürmüşdür. Faiz dərəcəsi 8%-dir. Borcun 1 000 000 manatı tikinti başlamazdan əvvəl 3 ay müddətinə 6% gəlirlə investisiya edilmişdir. Tikinti 1 apreldən il sonuna qədər davam etmişdir. İl üzrə kapitallaşdırılacaq xalis borclanma məsrəfi nə qədərdir?",
    "options": [
      "350 000 manat",
      "300 000 manat",
      "400 000 manat",
      "60 000 manat",
      "385 000 manat"
    ],
    "correct": "300 000 manat"
  },
  {
    "num": 96,
    "question": "Müəssisə zavod tikintisi üçün 2 000 000 manat xüsusi borc götürmüşdür. Faiz dərəcəsi 10%-dir. Dövlət zavodun tikintisinə görə 400 000 manat subsidiya vermişdir. Müəssisə subsidiyanı aktivin balans dəyərindən çıxır. Tikinti üzrə il ərzində 2 000 000 manat uyğun xərc çəkilmişdir. İlin sonunda aktivin balans dəyəri nə qədərdir?",
    "options": [
      "1 800 000 manat",
      "2 000 000 manat",
      "1 600 000 manat",
      "2 200 000 manat",
      "1 400 000 manat"
    ],
    "correct": "1 800 000 manat"
  },
  {
    "num": 97,
    "question": "Müəssisənin eyni vaxtda iki kvalifikasiya olunan tikinti layihəsi vardır. A layihəsinə 1 000 000 manat, B layihəsinə 2 000 000 manat xərclənmişdir. Ümumi borclanma üzrə orta faiz dərəcəsi 8%-dir. İki layihə üzrə ümumi kapitallaşdırılacaq borclanma məsrəfi nə qədərdir?",
    "options": [
      "240 000 manat",
      "160 000 manat",
      "320 000 manat",
      "200 000 manat",
      "80 000 manat"
    ],
    "correct": "240 000 manat"
  },
  {
    "num": 98,
    "question": "Müəssisə tikinti layihəsinə aşağıdakı xərcləri çəkmişdir: 1 yanvar — 1 000 000 manat; 1 aprel — 600 000 manat;1 oktyabr — 400 000 manat. Ümumi borclanma üzrə faiz dərəcəsi 10%-dir. Vaxtla çəkili xərclərin məbləği və kapitallaşdırılacaq faiz nə qədərdir?",
    "options": [
      "2 000 000 manat və 200 000 manat",
      "1 600 000 manat və 160 000 manat",
      "1 800 000 manat və 180 000 manat",
      "1 550 000 manat və 155 000 manat",
      "1 700 000 manat və 170 000 manat"
    ],
    "correct": "1 550 000 manat və 155 000 manat"
  },
  {
    "num": 99,
    "question": "Müəssisə tikinti üçün 4 000 000 manat xüsusi borc götürmüşdür. Faiz dərəcəsi 9%-dir. Vəsaitin 1 500 000 manatı 4 ay müddətinə investisiya edilmiş və illik 6% gəlir əldə edilmişdir. İl üzrə kapitallaşdırılacaq xalis borclanma məsrəfi nə qədərdir?",
    "options": [
      "360 000 manat",
      "30 000 manat",
      "330 000 manat",
      "294 000 manat",
      "270 000 manat"
    ],
    "correct": "330 000 manat"
  },
  {
    "num": 100,
    "question": "Müəssisə layihə üçün 2 000 000 manat xüsusi borc götürmüşdür. Faiz dərəcəsi 10%-dir. Bundan əlavə, ümumi borclanmanın orta faiz dərəcəsi 8%-dir. İl ərzində layihəyə 2 500 000 manat vəsait sərf edilmişdir. Bütün məbləğlər il ərzində uyğun aktivə sərf olunmuşdur. Kapitallaşdırılacaq borclanma məsrəfi nə qədərdir?",
    "options": [
      "210 000 manat",
      "180 000 manat",
      "160 000 manat",
      "240 000 manat",
      "250 000 manat"
    ],
    "correct": "240 000 manat"
  },
  {
    "num": 101,
    "question": "Müəssisə zavod tikintisinə 1 yanvarda başlamışdır. Zavod 30 sentyabrda istifadəyə hazır vəziyyətə gətirilmişdir. Xüsusi borcun illik faiz məsrəfi 360 000 manatdır. Kapitallaşdırılacaq faiz nə qədərdir?",
    "options": [
      "360 000 manat",
      "300 000 manat",
      "270 000 manat",
      "240 000 manat",
      "180 000 manat"
    ],
    "correct": "270 000 manat"
  },
  {
    "num": 102,
    "question": "Müəssisənin kvalifikasiya olunan aktivinin tikintisi zamanı 3 ay ərzində texniki səbəblərdən işlər tam dayandırılmışdır. Həmin dövrdə aktivin hazırlanması üzrə əhəmiyyətli fəaliyyət aparılmamışdır. İllik faiz məsrəfi 240 000 manatdır. Fasilə dövründə kapitallaşdırılmamalı borclanma məsrəfi nə qədərdir?",
    "options": [
      "240 000 manat",
      "180 000 manat",
      "40 000 manat",
      "80 000 manat",
      "60 000 manat"
    ],
    "correct": "60 000 manat"
  },
  {
    "num": 103,
    "question": "Müəssisə kvalifikasiya olunan aktivin tikintisinə 1 mart tarixində başlamışdır. Tikinti üzrə ilk xərc 1 aprel tarixində çəkilmişdir. 1 000 000 manat borc bütün il ərzində mövcud olmuş və illik faiz dərəcəsi 12% təşkil etmişdir. Cari il üçün kapitallaşdırılacaq faiz nə qədərdir?",
    "options": [
      "100 000 manat",
      "30 000 manat",
      "120 000 manat",
      "60 000 manat",
      "90 000 manat"
    ],
    "correct": "90 000 manat"
  },
  {
    "num": 104,
    "question": "Müəssisənin ümumi borcları aşağıdakılardır: 2 500 000 manat — 7% və 1 500 000 manat — 9%. Kvalifikasiya olunan aktivə il ərzində 1 200 000 manat xərclənmişdir. Ümumi borclanma üzrə orta çəkili faiz dərəcəsi və kapitallaşdırılacaq borclanma məsrəfi nə qədərdir?",
    "options": [
      "8,25% və 99 000 manat",
      "9% və 108 000 manat",
      "7,5% və 90 000 manat",
      "8% və 96 000 manat",
      "7,75% və 93 000 manat"
    ],
    "correct": "7,75% və 93 000 manat"
  },
  {
    "num": 105,
    "question": "Müəssisənin ümumi borcları: 2 000 000 manat — 8% və 3 000 000 manat — 10%. Kvalifikasiya olunan aktivə il ərzində 1 500 000 manat xərclənmişdir. Ümumi borclanma üzrə orta çəkili faiz dərəcəsi və kapitallaşdırılacaq məbləğ nə qədərdir?",
    "options": [
      "8,5% və 127 500 manat",
      "9% və 135 000 manat",
      "9,2% və 138 000 manat",
      "8% və 120 000 manat",
      "10% və 150 000 manat"
    ],
    "correct": "9,2% və 138 000 manat"
  },
  {
    "num": 106,
    "question": "Müəssisə tikinti layihəsi üçün 3 000 000 manat xüsusi borc götürmüşdür. Faiz dərəcəsi 8%-dir. Borcun 1 000 000 manatı 6 ay müddətinə bank depozitinə yerləşdirilmiş və illik 5% gəlir əldə edilmişdir. İl üzrə kapitallaşdırılacaq xalis borclanma məsrəfi nə qədərdir?",
    "options": [
      "200 000 manat",
      "190 000 manat",
      "215 000 manat",
      "50 000 manat",
      "240 000 manat"
    ],
    "correct": "215 000 manat"
  },
  {
    "num": 107,
    "question": "Qiymətdəndüşmədən yaranmış zərərin bərpası ilə bağlı hansı qayda \"Qudvil\" üçün tətbiq edilir?",
    "options": [
      "Qudvil zərəri yalnız audit yoxlamasından sonra bərpa edilə bilər",
      "Qudvil zərəri bərpa olunarkən dərhal sair məcmu gəlirdə tanınır",
      "Qudvilin zərəri yalnız bazar qiymətləri artdıqda bərpa edilə bilər",
      "Qudvilin zərəri müəssisənin mənfəəti artdıqda proporsional bərpa olunur",
      "Qudvilə münasibətdə tanınmış qiymətdəndüşmə zərəri sonrakı dövrlərdə heç bir halda bərpa edilmir"
    ],
    "correct": "Qudvilə münasibətdə tanınmış qiymətdəndüşmə zərəri sonrakı dövrlərdə heç bir halda bərpa edilmir"
  },
  {
    "num": 108,
    "question": "MHBS (IAS) 36-ya əsasən, aşağıdakılardan hansı aktivin qiymətdəndüşmə zərərin bərpa edilməsi üçün \"Kənar əlamət\" hesab olunur?",
    "options": [
      "Aktivin fiziki zədələnməsinin daha da pisləşməsi",
      "Bazar faiz dərəcələrinin azalması və bunun nəticəsində aktivin ödənilmə dəyərinin artması",
      "Aktivin bazar kapitallaşdırılmasının balans dəyərindən aşağı düşməsi",
      "Aktivin istifadə intensivliyinin azalması",
      "Müəssisənin fəaliyyət göstərdiyi bazarda rəqabətin kəskin artması"
    ],
    "correct": "Bazar faiz dərəcələrinin azalması və bunun nəticəsində aktivin ödənilmə dəyərinin artması"
  },
  {
    "num": 109,
    "question": "Törədici vahidə daxil olan ayrıca bir aktivin satış xərcləri çıxılmaqla ədalətli dəyəri balans dəyərindən aşağıdırsa, lakin bütövlükdə vahid qiymətdən düşməyibsə, zərər necə tanınır?",
    "options": [
      "Zərər yalnız həmin ayrıca aktiv üçün dərhal tanınmalıdır",
      "Qiymətdəndüşmədən olan zərər tanınmayacaqdır",
      "Zərər müəssisənin digər törədici vahidlərinin mənfəəti hesabına örtülməlidir",
      "Aktivin balans dəyəri mütləq satış qiymətinə qədər azaldılmalıdır",
      "Həmin aktiv dərhal balansdan silinməli və yenisi ilə əvəzlənməlidir"
    ],
    "correct": "Qiymətdəndüşmədən olan zərər tanınmayacaqdır"
  },
  {
    "num": 110,
    "question": "Törədici vahidə daxil olan hər hansı bir aktivin balans dəyəri zərər bölüşdürülərkən hansı kəmiyyətdən aşağı azaldıla bilməz?",
    "options": [
      "Aktivin ilkin alış dəyərinin 50 faizindən",
      "Satış xərcləri çıxılmaqla ədalətli dəyər, istifadənin qiymətliliyi və ya sıfırdan ən yüksək olanından",
      "Müəssisənin bütün aktivləri üçün müəyyən edilmiş orta bazar qiymətindən",
      "Aktivin illik amortizasiya məbləğinin ikiqatından",
      "Yalnız aktivin sıfıra bərabər olan dəyərindən"
    ],
    "correct": "Satış xərcləri çıxılmaqla ədalətli dəyər, istifadənin qiymətliliyi və ya sıfırdan ən yüksək olanından"
  },
  {
    "num": 111,
    "question": "MHBS (IAS) 36-nın 104-cü bəndinə əsasən, törədici vahid üzrə yaranan qiymətdəndüşmə zərəri hansı ardıcıllıqla bölüşdürülməlidir?",
    "options": [
      "Zərər yalnız mənsub olduğu vahidin ən köhnə aktivlərinin dəyərindən çıxılmalıdır",
      "Zərər yalnız müəssisənin sərbəst pul vəsaitləri hesabına bağlanmalı, aktivlərin dəyəri azaldılmamalıdır",
      "Zərər bütün aktivlər (qudvil daxil olmaqla) arasında bərabər məbləğlərdə bölüşdürülməlidir",
      "İlk növbədə torpaq və tikililərin dəyəri azaldılmalı, ən sonda isə qudvilə toxunulmalıdır",
      "İlk növbədə vahidə aid qudvilin balans dəyəri azaldılır, qalan zərər isə digər aktivlərin balans dəyərinə proporsional bölüşdürülür"
    ],
    "correct": "İlk növbədə vahidə aid qudvilin balans dəyəri azaldılır, qalan zərər isə digər aktivlərin balans dəyərinə proporsional bölüşdürülür"
  },
  {
    "num": 112,
    "question": "Göstəricilərə görə avadanlıq üçün 20X1-ci ildə tanınan qiymətdəndüşmə zərəri nə qədərdir? (Balans dəyəri: 650 000, Ödənilmə dəyəri: 618 232)",
    "options": [
      "105 000 p.v.",
      "31 768 p.v.",
      "545 000 p.v.",
      "650 000 p.v.",
      "711 000 p.v."
    ],
    "correct": "31 768 p.v."
  },
  {
    "num": 113,
    "question": "Törədici vahidin identifikasiyası zamanı \"ardıcıllıq\" prinsipi nəyi tələb edir?",
    "options": [
      "Törədici vahidlər hər il müəssisənin mənfəətindən asılı olaraq yenidən qruplaşdırılmalıdır",
      "Əsaslandırılmış səbəb yoxdursa, eyni aktiv tipləri üçün törədici vahidlər hər dövrdə eyni qaydada müəyyən edilməlidir",
      "Qudvil hər il fərqli törədici vahidlər arasında yenidən bölüşdürülməlidir",
      "Törədici vahidlər yalnız auditorların tələbi ilə identifikasiya edilməlidir",
      "Hər bir ayrıca aktiv mütləq təkbaşına bir törədici vahid kimi tanınmalıdır"
    ],
    "correct": "Əsaslandırılmış səbəb yoxdursa, eyni aktiv tipləri üçün törədici vahidlər hər dövrdə eyni qaydada müəyyən edilməlidir"
  },
  {
    "num": 114,
    "question": "\"İqtisadi resurs\" anlayışına Konseptual əsaslarda verilən düzgün tərif hansıdır?",
    "options": [
      "Müəssisənin sahib olduğu bütün borc öhdəliklərinin cəmidir",
      "Təşkilatın istifadə etdiyi bütün ictimai yollar və infrastruktur obyektləridir",
      "Gələcəkdə mütləq şəkildə əldə ediləcək nəqd pul vəsaitləridir",
      "Yalnız fiziki formada olan və toxunula bilən aktivlərdir",
      "İqtisadi faydalar yaratmaq potensialına malik olan mövcud hüquqdur"
    ],
    "correct": "İqtisadi faydalar yaratmaq potensialına malik olan mövcud hüquqdur"
  },
  {
    "num": 115,
    "question": "İqtisadi resursu \"Aktiv\" kimi tanımaq üçün hansı iki şərtə əməl edilməlidir?",
    "options": [
      "Aktiv yalnız nağd pulla alınmalı və dərhal istismara verilməlidir",
      "Aktivin üzərində heç bir girov öhdəliyi olmamalı və o, yalnız ana şirkətə məxsus olmalıdır",
      "Hüquq mütləq şəkildə fiziki formaya malik olmalı və mülkiyyət hüququ qeydiyyatdan keçməlidir",
      "Aktivin dəyəri 100 000 manatdan çox olmalı və istifadə müddəti 10 ili keçməlidir",
      "Hüquq təşkilat üçün artıq iqtisadi fayda yaratmaq potensialına malik olmalı və bu faydalara təşkilat nəzarət etməlidir"
    ],
    "correct": "Hüquq təşkilat üçün artıq iqtisadi fayda yaratmaq potensialına malik olmalı və bu faydalara təşkilat nəzarət etməlidir"
  },
  {
    "num": 116,
    "question": "Xüsusi kapitalın (Equity) ümumi kəmiyyəti maliyyə hesabatlarında necə müəyyən edilir?",
    "options": [
      "Müstəqil qiymətləndirici tərəfindən hər il birbaşa müəyyən edilməklə",
      "Təşkilatın malik olduğu nəqd pul vəsaitlərinin ümumi məbləğinə bərabər tutulmaqla",
      "Müəssisənin gələcək on ildəki mənfəət proqnozlarını diskontlaşdırmaqla",
      "Bütün tanınmış öhdəliklərin dəyəri tanınmış aktivlərin dəyərindən çıxılmaqla (Aktiv = Öhdəlik + Xüsusi Kapital)",
      "Yalnız səhmlərin birjadakı cari bazar qiymətlərini toplamaqla"
    ],
    "correct": "Bütün tanınmış öhdəliklərin dəyəri tanınmış aktivlərin dəyərindən çıxılmaqla (Aktiv = Öhdəlik + Xüsusi Kapital)"
  },
  {
    "num": 117,
    "question": "Hansı qiymətləndirmə bazaları \"Çıxış dəyəri\" (Exit value) hesab edilir?",
    "options": [
      "Tarixi dəyər və əvəzetmənin cari dəyəri",
      "Ədalətli dəyər, istifadənin qiymətliliyi və icraetmənin dəyəri",
      "Aktivin amortizasiya olunan dəyəri",
      "Debitor borcların nominal dəyəri",
      "Yalnız ilkin əldə edilmə məsrəfləri"
    ],
    "correct": "Ədalətli dəyər, istifadənin qiymətliliyi və icraetmənin dəyəri"
  },
  {
    "num": 118,
    "question": "\"İstifadənin qiymətliliyi\" (Value in use) hansı göstəriciyə əsaslanır?",
    "options": [
      "Aktivin ilkin alınma qiyməti ilə yığılmış amortizasiya arasındakı fərqə",
      "Aktivin yalnız fiziki aşınma dərəcəsinə",
      "Aktivin cari bazarda satıla biləcəyi faktiki qiymətə",
      "Ekvivalent aktivin əldə edilməsi üçün tələb olunan cari məsrəflərə",
      "Aktivin istifadəsindən və çıxmasından gözlənilən pul vəsaitlərinin diskontlaşdırılmış dəyərinə"
    ],
    "correct": "Aktivin istifadəsindən və çıxmasından gözlənilən pul vəsaitlərinin diskontlaşdırılmış dəyərinə"
  },
  {
    "num": 119,
    "question": "\"Ədalətli dəyər\" (Fair value) qiymətləndirmə bazasının mahiyyəti nədir?",
    "options": [
      "Aktivin sığorta şirkəti tərəfindən müəyyən edilmiş bərpa dəyəridir",
      "Yalnız rəhbərliyin subyektiv mülahizəsinə əsaslanan dəyərdir",
      "Müəssisənin aktivdən istifadə edərək gələcəkdə əldə edəcəyi pul vəsaitlərinin cəmidir",
      "Aktivin ilkin əldə edilməsi zamanı ödənilmiş faktiki məbləğdir",
      "Bazar iştirakçıları arasında aktiv satılarkən alına biləcək yaxud öhdəlik verilərkən ödənilə biləcək qiymətdir"
    ],
    "correct": "Bazar iştirakçıları arasında aktiv satılarkən alına biləcək yaxud öhdəlik verilərkən ödənilə biləcək qiymətdir"
  },
  {
    "num": 120,
    "question": "Qiymətləndirmə bazalarından biri olan \"Tarixi dəyər\" (Historical cost) haqqında hansı fikir doğrudur?",
    "options": [
      "Aktivlər hər il yenidən qiymətləndirilərək cari bazar qiyməti ilə əks olunur",
      "Tarixi dəyər hər zaman aktivin satışından əldə edilə biləcək məbləğə bərabərdir",
      "Tarixi dəyərə aktivin əldə edilməsi üçün çəkilən sövdələşmə məsrəfləri daxil edilmir",
      "Aktivlər və öhdəliklər onların yaranmış olduğu əməliyyatın qiyməti əsasında təqdim edilir və adətən dəyişmir",
      "Bu dəyər yalnız gələcək pul axınlarının diskontlaşdırılmış məbləğidir"
    ],
    "correct": "Aktivlər və öhdəliklər onların yaranmış olduğu əməliyyatın qiyməti əsasında təqdim edilir və adətən dəyişmir"
  },
  {
    "num": 121,
    "question": "Aktivin tanınmasının dayandırılması (Derecognition) adətən nə zaman baş verir?",
    "options": [
      "Aktivin bazar dəyəri tarixi dəyərindən aşağı düşdükdə",
      "Aktivin fiziki forması dəyişdikdə",
      "Hesabat dövrü başa çatdıqda və yeni dövr başladıqda",
      "Təşkilat tanınmış aktiv üzərində öz nəzarətini itirdiyi anda",
      "Aktiv tam amortizasiya olunduqda, lakin hələ də istifadə edildikdə"
    ],
    "correct": "Təşkilat tanınmış aktiv üzərində öz nəzarətini itirdiyi anda"
  },
  {
    "num": 122,
    "question": "Əgər müəssisə qudvil aid edilmiş bir törədici vahidin bir hissəsini satırsa, satılan hissəyə aid qudvil necə müəyyən edilir?",
    "options": [
      "Bütün qudvil satılan hissə ilə birlikdə balansdan silinir",
      "Satılan hissə üzrə qudvil dərhal mənfəət və zərər haqqında hesabatda gəlir kimi tanınır",
      "Qudvil yalnız bazar qiyməti ilə yenidən qiymətləndirilərək satılır",
      "Təsərrüfatdan çıxan fəaliyyətin nisbi dəyəri və saxlanılan hissənin dəyəri əsasında (məsələn, proporsional)",
      "Qudvilin hamısı müəssisədə saxlanılır və satılan hissəyə aid edilmir"
    ],
    "correct": "Təsərrüfatdan çıxan fəaliyyətin nisbi dəyəri və saxlanılan hissənin dəyəri əsasında (məsələn, proporsional)"
  },
  {
    "num": 123,
    "question": "Korporativ aktivlərin (məsələn, baş ofis binası) fərqləndirici xüsusiyyəti nədir?",
    "options": [
      "Onların ödənilmə dəyəri hər zaman balans dəyərindən yüksək olur",
      "Onlar digər aktivlərdən asılı olmayaraq müstəqil pul vəsaitləri hərəkəti yaratmırlar",
      "Korporativ aktivlər heç vaxt qiymətdəndüşmə testinə cəlb edilmirlər",
      "Onlar dərhal mənfəət və zərərdə xərc kimi tanınan qısamüddətli aktivlərdir",
      "Onlar yalnız qudvil ilə birlikdə bir aktiv kimi tanınırlar"
    ],
    "correct": "Onlar digər aktivlərdən asılı olmayaraq müstəqil pul vəsaitləri hərəkəti yaratmırlar"
  },
  {
    "num": 124,
    "question": "Törədici vahid üzrə qiymətdəndüşmə zərəri tanınarkən, balans dəyərinin azaldılması hansı ardıcıllıqla həyata keçirilir?",
    "options": [
      "Əvvəlcə torpaq və binaların dəyəri azaldılır, qudvil isə sonuncu pillədə saxlanılır",
      "Əvvəlcə qudvilin balans dəyəri azaldılır, sonra digər aktivlərin dəyəri proporsional olaraq azaldılır",
      "Zərər dərhal ehtiyat kapitalı hesabına silinir və aktivlərə toxunulmur",
      "Zərər yalnız maliyyə aktivlərinin balans dəyərinə aid edilir",
      "Bütün aktivlərin (qudvil daxil olmaqla) dəyəri eyni faiz dərəcəsi ilə azaldılır"
    ],
    "correct": "Əvvəlcə qudvilin balans dəyəri azaldılır, sonra digər aktivlərin dəyəri proporsional olaraq azaldılır"
  },
  {
    "num": 125,
    "question": "Törədici vahidə aid edilmiş qudvilin qiymətdəndüşmə testi nə vaxt aparılmalıdır?",
    "options": [
      "Yalnız müəssisə il ərzində xalis zərər əldə etdikdə",
      "Qudvil hər rübün sonunda bütün aktivlərlə birlikdə yoxlanılmalıdır",
      "Yalnız qudvilin aid olduğu vahid ləğv edildikdə",
      "Hər il eyni vaxtda aparılmalı, həmçinin qiymətdəndüşmə əlamətləri olduqda yoxlanılmalıdır",
      "5 ildən bir mütləq qaydada, digər illərdə isə könüllü olaraq"
    ],
    "correct": "Hər il eyni vaxtda aparılmalı, həmçinin qiymətdəndüşmə əlamətləri olduqda yoxlanılmalıdır"
  },
  {
    "num": 126,
    "question": "Biznesin birləşdirilməsi nəticəsində əldə edilmiş qudvil qiymətdəndüşmə testi üçün hara bölüşdürülməlidir?",
    "options": [
      "Yalnız müəssisənin ən yüksək səviyyəli əməliyyat seqmentinə",
      "Əldə edildiyi tarixdən etibarən qudvilin izlənildiyi ən aşağı səviyyədəki törədici vahidlərə və ya qruplara",
      "Qudvil yalnız aktiv satıldığı zaman mənfəət və zərər hesabına daxil edilir",
      "Qudvil bölüşdürülmür və ayrıca bir törədici vahid kimi saxlanılır",
      "Müəssisənin bütün maddi aktivləri arasında bərabər məbləğlərdə"
    ],
    "correct": "Əldə edildiyi tarixdən etibarən qudvilin izlənildiyi ən aşağı səviyyədəki törədici vahidlərə və ya qruplara"
  },
  {
    "num": 127,
    "question": "Törədici vahidin (PVTV) balans dəyərinə hansı aktivlər daxil edilir?",
    "options": [
      "Yalnız ədalətli dəyəri balans dəyərindən yüksək olan aktivlər",
      "Yalnız müəssisənin baş ofisinə məxsus olan korporativ aktivlər",
      "Müəssisənin sahib olduğu bütün nağd pul vəsaitləri və debitor borcları",
      "Ağlabatan və ardıcıl əsasda həmin vahidə aid edilə bilən və gələcək pul daxilolmalarını təmin edən aktivlər",
      "Vahidlə əlaqəsi olmayan, lakin eyni ərazidə yerləşən bütün digər aktivlər"
    ],
    "correct": "Ağlabatan və ardıcıl əsasda həmin vahidə aid edilə bilən və gələcək pul daxilolmalarını təmin edən aktivlər"
  },
  {
    "num": 128,
    "question": "MHBS (IAS) 36-ya əsasən, ayrıca aktivin ödənilmə dəyərini qiymətləndirmək mümkün olmadıqda nə edilməlidir?",
    "options": [
      "Aktivin balans dəyəri dərhal sıfıra bərabər tutulmalıdır",
      "Aktivin mənsub olduğu törədici vahidin (PVTV) ödənilmə dəyəri müəyyən edilməlidir",
      "Müəssisənin bütün aktivlərinin ümumi bazar dəyəri hesablanmalıdır",
      "Qiymətdəndüşmə testi növbəti hesabat ilinə qədər təxirə salınmalıdır",
      "Aktivin yalnız qırıntı (ləğv) dəyəri uçotda saxlanılmalıdır"
    ],
    "correct": "Aktivin mənsub olduğu törədici vahidin (PVTV) ödənilmə dəyəri müəyyən edilməlidir"
  },
  {
    "num": 129,
    "question": "Aktiv yaxud öhdəliyin \"Tanınması\" (Recognition) nə deməkdir?",
    "options": [
      "Yalnız aktivin mülkiyyət hüququnun rəsmiləşdirilməsidir",
      "Şirkətin gələcək illər üçün satış proqnozlarının sənədləşdirilməsidir",
      "Maddənin element tərifinə cavab verərək maliyyə vəziyyəti və ya maliyyə nəticələri hesabatına daxil edilməsi prosesidir",
      "Hesabat dövrünün sonunda aktivlərin bazar qiymətinin müəyyən edilməsidir",
      "Maddənin yalnız anbara mədaxil edilməsi və fiziki sayılmasıdır"
    ],
    "correct": "Maddənin element tərifinə cavab verərək maliyyə vəziyyəti və ya maliyyə nəticələri hesabatına daxil edilməsi prosesidir"
  },
  {
    "num": 130,
    "question": "\"Gəlirlər\" elementinin Konseptual əsaslardakı tərifi aşağıdakılardan hansıdır?",
    "options": [
      "Müəssisənin səhmdarları tərəfindən kapitala edilən əlavə ödənişlərdir",
      "Yalnız gələcəkdə alınması gözlənilən iqtisadi faydalardır",
      "Aktivlərin azalması və ya öhdəliklərin artması nəticəsində yaranan mənfəətdir",
      "Aktivlərin artması yaxud öhdəliklərin azalmasıdır ki, bu da xüsusi kapitalın (sahiblərin payı ilə bağlı olmayan) artımına səbəb olur",
      "Yalnız müştərilərdən daxil olan nağd pul vəsaitləridir"
    ],
    "correct": "Aktivlərin artması yaxud öhdəliklərin azalmasıdır ki, bu da xüsusi kapitalın (sahiblərin payı ilə bağlı olmayan) artımına səbəb olur"
  },
  {
    "num": 131,
    "question": "Konseptual əsaslara görə \"Aktiv\" elementinin düzgün tərifi hansıdır?",
    "options": [
      "Gələcəkdə müəssisəyə daxil olacaq bütün pul vəsaitlərinin cəmidir",
      "Hamı üçün əlçatan olan infrastruktur obyektləridir (məsələn, yollar)",
      "Təşkilatın özü tərəfindən buraxılmış və geri satın alınmış səhmlərdir",
      "Keçmiş hadisələr nəticəsində təşkilat tərəfindən nəzarət olunan mövcud iqtisadi resursdur",
      "Müəssisə rəhbərliyinə məxsus olan bütün fiziki əmlakdır"
    ],
    "correct": "Keçmiş hadisələr nəticəsində təşkilat tərəfindən nəzarət olunan mövcud iqtisadi resursdur"
  },
  {
    "num": 132,
    "question": "Gələcəkdə baş verə biləcək əməliyyatlar haqqında (proqnoz) informasiya hansı halda maliyyə hesabatlarına daxil edilə bilər?",
    "options": [
      "Yalnız rəhbərliyin şəxsi arzusu olduqda",
      "Bütün hallarda proqnoz informasiyanın daxil edilməsi məcburidir",
      "Proqnoz informasiya heç bir halda maliyyə hesabatlarına daxil edilə bilməz",
      "Hesabat dövrünün sonuna olan aktiv, öhdəlik və xüsusi kapitala aiddirsə və istifadəçilər üçün faydalıdırsa",
      "Yalnız vergi azalmaları proqnozlaşdırıldıqda"
    ],
    "correct": "Hesabat dövrünün sonuna olan aktiv, öhdəlik və xüsusi kapitala aiddirsə və istifadəçilər üçün faydalıdırsa"
  },
  {
    "num": 133,
    "question": "Əgər hesabat verən təşkilata həm ana şirkət, həm də onun nəzarət etdiyi törəmə şirkətlər daxildirsə, belə hesabat necə adlanır?",
    "options": [
      "Konsolidə olunmamış maliyyə hesabatlılığı",
      "Fərdi maliyyə hesabatlılığı",
      "Statik maliyyə hesabatlılığı",
      "Konsolidə olunmuş maliyyə hesabatlılığı",
      "Kombinələşmiş maliyyə hesabatlılığı"
    ],
    "correct": "Konsolidə olunmuş maliyyə hesabatlılığı"
  },
  {
    "num": 134,
    "question": "Maliyyə hesabatları adətən hansı fundamental yolverilmə (prinsip) əsasında tərtib edilir?",
    "options": [
      "Mənfəətin maksimallaşdırılması prinsipi",
      "Dövlət nəzarəti prinsipi",
      "Yalnız keçmiş hadisələrin əks olunması prinsipi",
      "Fəaliyyətin fasiləsizliyi prinsipi (Going concern)",
      "Kassas üsulu prinsipi"
    ],
    "correct": "Fəaliyyətin fasiləsizliyi prinsipi (Going concern)"
  },
  {
    "num": 135,
    "question": "Maliyyə hesabatlılığının əsas məqsədi nədir?",
    "options": [
      "Təşkilatın bazar dəyərini birbaşa müəyyən etmək",
      "Yalnız dövlət vergi orqanları üçün gizli məlumatlar toplamaq",
      "Rəqib şirkətlərin strategiyalarını təhlil etmək",
      "Müəssisənin gündəlik texniki əməliyyatlarını qeydə almaq",
      "Təşkilatın aktivləri, öhdəlikləri, gəlir və xərcləri haqqında faydalı maliyyə informasiyası təqdim etmək"
    ],
    "correct": "Təşkilatın aktivləri, öhdəlikləri, gəlir və xərcləri haqqında faydalı maliyyə informasiyası təqdim etmək"
  },
  {
    "num": 136,
    "question": "İnformasiyanın \"münasib\" (relevant) hesab olunması üçün o hansı xüsusiyyətlərə malik olmalıdır?",
    "options": [
      "Yalnız rəqəmlərlə ifadə olunmalıdır",
      "Şirkətin bazar dəyərini dəqiq göstərməlidir",
      "Yalnız keçmiş hadisələri əks etdirməlidir",
      "Həm təsdiqedetmə, həm də proqnoz vermə üçün əhəmiyyətli olmalıdır",
      "Mütləq şəkildə birbaşa yoxlanıla bilməlidir"
    ],
    "correct": "Həm təsdiqedetmə, həm də proqnoz vermə üçün əhəmiyyətli olmalıdır"
  },
  {
    "num": 137,
    "question": "Konseptual əsaslara görə, \"neytrallıq\" prinsipini möhkəmləndirən və aktivlərin/gəlirlərin əsassız artırılmamasını nəzərdə tutan anlayış hansıdır?",
    "options": [
      "Ehtiyatlılıq (prudence)",
      "Anlaşıqlılıq (understandability)",
      "Əhəmiyyətlilik (materiality)",
      "Münasiblik (relevance)",
      "Müqayisəlilik (comparability)"
    ],
    "correct": "Ehtiyatlılıq (prudence)"
  },
  {
    "num": 138,
    "question": "Qiymətdəndüşmədən olan zərər tanındıqdan sonra aktivə hesablanan amortizasiya ayırmaları ilə bağlı hansı prosedur yerinə yetirilməlidir?",
    "options": [
      "Aktivin qalan xidmət müddəti amortizasiya məqsədləri üçün ikiqat artırılmalıdır",
      "Yalnız aktivin ləğv etmə dəyəri dəyişdikdə amortizasiya korrektə edilməlidir",
      "Amortizasiya hesablanması dərhal dayandırılmalıdır",
      "Aktivin ilkin (zərərdən əvvəlki) dəyəri əsasında amortizasiya hesablanmasına davam edilməlidir",
      "Amortizasiya gələcək dövrlərdə korrektə edilməli və yenidən baxılmış balans dəyəri qalan xidmət müddətinə bölüşdürülməlidir"
    ],
    "correct": "Amortizasiya gələcək dövrlərdə korrektə edilməli və yenidən baxılmış balans dəyəri qalan xidmət müddətinə bölüşdürülməlidir"
  },
  {
    "num": 139,
    "question": "Yenidənqiymətləndirilmiş aktivlər (IAS 16-ya əsasən ehtiyatı olan aktivlər) üzrə qiymətdəndüşmə zərəri ilk növbədə necə uçota alınmalıdır?",
    "options": [
      "Hər bir halda birbaşa mənfəət və zərər hesabatına aid edilməklə",
      "Əvvəlki yenidənqiymətləndirilmə məbləğinin (ehtiyatın) azaldılması kimi",
      "Uzunmüddətli öhdəliklərin artırılması yolu ilə",
      "Aktivin maya dəyərinin süni şəkildə artırılması ilə",
      "Aktivin satışından əldə olunan sair gəlirlər hesabına"
    ],
    "correct": "Əvvəlki yenidənqiymətləndirilmə məbləğinin (ehtiyatın) azaldılması kimi"
  },
  {
    "num": 140,
    "question": "Əgər aktiv yenidənqiymətləndirilmə modeli ilə uçota ALINMIRSA (məsələn, maya dəyəri modeli ilə uçota alınırsa), qiymətdəndüşmə zərəri harada tanınmalıdır?",
    "options": [
      "Kapitalın tərkibindəki yenidənqiymətləndirmə ehtiyatı hesabında",
      "Hesabat dövrünün sonundakı bölüşdürülməmiş mənfəətdə gizli şəkildə",
      "Balansın aktiv hissəsində debitor borcu kimi",
      "Dərhal mənfəət yaxud zərər hesabatında (xərclərdə)",
      "Gələcək dövrlərin gəlirləri maddəsində"
    ],
    "correct": "Dərhal mənfəət yaxud zərər hesabatında (xərclərdə)"
  },
  {
    "num": 141,
    "question": "Aktivin qiymətdəndüşmə zərəri hansı halda yaranır və necə müəyyən edilir?",
    "options": [
      "Aktivin bazar qiyməti müəssisənin nizamnamə kapitalından yüksək olduqda",
      "Aktivin ödənilmə dəyəri onun balans dəyərindən az olduqda və balans dəyəri ödənilmə dəyərinə qədər azaldıldıqda",
      "Aktivin amortizasiya olunan kəmiyyəti onun ləğv etmə dəyərinə bərabər olduqda",
      "Aktivin ədalətli dəyəri onun istifadənin qiymətliliyi ilə eyni səviyyəyə çatdıqda",
      "Aktivin istifadə müddəti gözləniləndən daha sürətlə başa çatdıqda"
    ],
    "correct": "Aktivin ödənilmə dəyəri onun balans dəyərindən az olduqda və balans dəyəri ödənilmə dəyərinə qədər azaldıldıqda"
  },
  {
    "num": 142,
    "question": "Əgər bir aktiv təkbaşına (digər aktivlərdən asılı olmadan) pul daxilolmalarını təmin etmirsə, ödənilmə dəyəri necə müəyyən edilməlidir?",
    "options": [
      "Aktivin yalnız ləğv etmə dəyəri əsasında",
      "Aktivin mənsub olduğu pul vəsaitləri törədən vahid (törədici vahid) üçün",
      "Həmin aktiv üçün ayrıca ədalətli dəyər hesablanması məcburidir",
      "Aktiv qiymətdən düşmüş hesab edilmir və uçotdan silinir",
      "Müəssisənin bütün aktivlərinin ümumi orta dəyəri əsasında"
    ],
    "correct": "Aktivin mənsub olduğu pul vəsaitləri törədən vahid (törədici vahid) üçün"
  },
  {
    "num": 143,
    "question": "Xarici valyuta ilə yaradılan pul vəsaitlərinin gələcək axınları zamanı istifadənin qiymətliliyi necə hesablanır?",
    "options": [
      "Bütün pul axınları əvvəlcə hesabat valyutasına çevrilir, sonra isə yerli faiz dərəcəsi ilə diskontlaşdırılır",
      "Pul axınları yaradıldığı valyutada qiymətləndirilir, diskontlaşdırılır və hesablama tarixinə olan cari mübadilə məzənnəsi ilə çevrilir",
      "Xarici valyuta ilə pul axınları zamanı diskontlaşdırma stavkası həmişə 0% qəbul edilir",
      "Valyuta fərqləri istifadənin qiymətliliyinə təsir etmir, yalnız satışa xərclərə aid edilir",
      "Yalnız hesabat dövrünün sonundakı proqnozlaşdırılan gələcək məzənnədən istifadə edilir"
    ],
    "correct": "Pul axınları yaradıldığı valyutada qiymətləndirilir, diskontlaşdırılır və hesablama tarixinə olan cari mübadilə məzənnəsi ilə çevrilir"
  },
  {
    "num": 144,
    "question": "Diskontlaşdırılma stavkası (stavkaları) barədə hansı fikir MHBS (IAS) 36-ya uyğundur?",
    "options": [
      "Bu, vergitutmadan sonrakı stavkadır və müəssisənin bütün aktivləri üçün eyni (vahid) olmalıdır",
      "Diskontlaşdırma stavkası yalnız xarici valyuta ilə olan pul axınlarına tətbiq edilir",
      "Diskontlaşdırma zamanı yalnız inflyasiya dərəcəsi nəzərə alınmalı, risklər istisna edilməlidir",
      "Bu, vergitutmaya qədər olan stavkadır və pulun vaxt üzrə dəyərini, həmçinin aktivə xas spesifik riskləri əks etdirir",
      "Bu stavka yalnız müəssisənin bankdan aldığı kreditin faktiki faiz dərəcəsinə bərabərdir"
    ],
    "correct": "Bu, vergitutmaya qədər olan stavkadır və pulun vaxt üzrə dəyərini, həmçinin aktivə xas spesifik riskləri əks etdirir"
  },
  {
    "num": 145,
    "question": "İnformasiyanın \"düzgün təqdim olunması\" (faithful representation) hansı üç xüsusiyyəti özündə birləşdirir?",
    "options": [
      "Münasiblik, əhəmiyyətlilik və proqnoz dəyəri",
      "Müqayisəlilik, vaxtında təqdim edilmə və aydınlıq",
      "Birbaşa və dolayı yoxlanıla bilmə",
      "Ehtiyatlılıq, mürəkkəblik və təsnifat",
      "Tamlıq, neytrallıq və səhvlərin olmaması"
    ],
    "correct": "Tamlıq, neytrallıq və səhvlərin olmaması"
  },
  {
    "num": 146,
    "question": "Faydalı maliyyə informasiyasının əsas (fundamental) keyfiyyət xarakteristikaları hansılardır?",
    "options": [
      "Tamlıq və neytrallıq",
      "Müqayisəlilik və vaxtında təqdim edilmə",
      "Yoxlanıla bilmə və anlaşıqlılıq",
      "Münasiblik (relevantlıq) və düzgün (dürüst) təqdim edilmə",
      "Proqnoz əhəmiyyətliliyi və səhvsizlik"
    ],
    "correct": "Münasiblik (relevantlıq) və düzgün (dürüst) təqdim edilmə"
  },
  {
    "num": 147,
    "question": "Konseptual əsasların məqsədləri sırasında \"Interpretasiya\" (şərhlər) ilə bağlı hansı bənd qeyd edilmişdir?",
    "options": [
      "Şərhləri yalnız 2018-ci ildən əvvəlki standartlara tətbiq etmək",
      "Şərhlərin hazırlanmasını yalnız transmilli şirkətlərin ixtiyarına vermək",
      "Standartların interpretasiyasını tamamilə qadağan etmək",
      "Yalnız vergi orqanlarına şərhlər vermək",
      "Standartların başa düşülməsində və interpretasiyasında bütün tərəflərə yardım göstərmək"
    ],
    "correct": "Standartların başa düşülməsində və interpretasiyasında bütün tərəflərə yardım göstərmək"
  },
  {
    "num": 148,
    "question": "Ümumi təyinatlı maliyyə hesabatları haqqında hansı fikir yanlışdır",
    "options": [
      "Tənzimləyici orqanlar bu hesabatlardan faydalana bilsələr də, hesabatlar bilavasitə onlara istiqamətlənməmişdir",
      "Bu hesabatlar istifadəçilərə təşkilatın dəyərini qiymətləndirməyə kömək edən informasiyaya malikdir",
      "Maliyyə hesabatları iqtisadi hadisələrin mütləq dəqiqliklə deyil, daha çox qiymətləndirmələrə əsasən əks etdirilməsidir",
      "Rəhbərlik zəruri maliyyə informasiyasını yalnız bu hesabatlardan deyil, daxili mənbələrdən də almalıdır",
      "Ümumi təyinatlı maliyyə hesabatları hesabat verən təşkilatın real bazar dəyərini göstərmək üçün nəzərdə tutulmuşdur"
    ],
    "correct": "Ümumi təyinatlı maliyyə hesabatları hesabat verən təşkilatın real bazar dəyərini göstərmək üçün nəzərdə tutulmuşdur"
  },
  {
    "num": 149,
    "question": "Ümumi təyinatlı maliyyə hesabatlarının əsas məqsədi kimlər üçün faydalı informasiya təmin etməkdir?",
    "options": [
      "Yalnız yerli bələdiyyə orqanları",
      "Mövcud və potensial investorlar, borcverənlər və digər kreditorlar",
      "Yalnız müəssisənin aşağı səviyyəli işçi heyəti",
      "Yalnız dövlət statistika komitəsi",
      "Rəqib şirkətlərin marketinq şöbələri"
    ],
    "correct": "Mövcud və potensial investorlar, borcverənlər və digər kreditorlar"
  },
  {
    "num": 150,
    "question": "Konseptual əsasların əsas təyinatı və məqsədi hansıdır?",
    "options": [
      "Mövcud olan bütün beynəlxalq standartları (IFRS) birbaşa əvəz etmək",
      "Standartlardan kənar iqtisadi əməliyyatların aparılmasını qadağan etmək",
      "Yalnız auditorların fəaliyyətinə nəzarət etmək",
      "Standartların işlənib hazırlanmasında Şuraya köməklik göstərmək və uçot siyasətinin seçilməsində yardım etmək",
      "Şirkətlərin vergi bəyannamələrini hazırlamaq üçün metodlar təqdim etmək"
    ],
    "correct": "Standartların işlənib hazırlanmasında Şuraya köməklik göstərmək və uçot siyasətinin seçilməsində yardım etmək"
  },
  {
    "num": 151,
    "question": "MHBS Şurası tərəfindən \"Maliyyə hesabatlarının təqdim edilməsinin Konseptual əsasları\" sənədinin son variantı neçənci ildə təsdiq edilmişdir?",
    "options": [
      "1973-cü ilin iyun ayında",
      "2010-cu ilin yanvar ayında",
      "2001-ci ilin aprel ayında",
      "2020-ci ilin dekabr ayında",
      "2018-ci ilin mart ayında"
    ],
    "correct": "2018-ci ilin mart ayında"
  },
  {
    "num": 152,
    "question": "MHBS və US GAAP arasındakı fərqləri aradan qaldırmaq üçün MHBS Şurası hansı qurumla birgə layihələr həyata keçirir?",
    "options": [
      "ASB (Accounting Standard Board)",
      "Beynəlxalq Valyuta Fondu",
      "Avropa Mərkəzi Bankı",
      "FASB (Financial Accounting Standards Board)",
      "ICAEW (İngiltərə və Uels andlı mühasiblər İnstitutu)"
    ],
    "correct": "FASB (Financial Accounting Standards Board)"
  },
  {
    "num": 153,
    "question": "GAAP (Ümumqəbulolunmuş Uçot Prinsipləri) haqqında verilən fikirlərdən hansı doğrudur?",
    "options": [
      "GAAP sistemi 2002-ci ildən sonra ləğv edilmişdir",
      "GAAP-lar bütün dünyada məcburi normativ-hüquqi qüvvəyə malikdir",
      "GAAP və MHBS arasında heç bir nəzəri-metodoloji oxşarlıq yoxdur",
      "GAAP-lar bilavasitə standart deyil, standartların hazırlanmasında istifadə edilən razılaşdırılmış qaydalar və prosedurlardır",
      "GAAP-lar yalnız kənd təsərrüfatı sahəsini tənzimləyir"
    ],
    "correct": "GAAP-lar bilavasitə standart deyil, standartların hazırlanmasında istifadə edilən razılaşdırılmış qaydalar və prosedurlardır"
  },
  {
    "num": 154,
    "question": "Gələcək pul vəsaitləri axınlarının hesabi qiymətləndirilməsinə aşağıdakıların hansı daxil edilməməlidir?",
    "options": [
      "Aktivin istifadəsinin davam etməsindən gözlənilən pul daxilolmaları",
      "Maliyyə fəaliyyəti və mənfəət vergisi ilə əlaqədar pul daxilolmaları və xaricolmaları",
      "Aktivin xidmət müddətinin sonunda təsərrüfatdan çıxmasından gözlənilən xalis axınlar",
      "Aktivin cari vəziyyətinə xidmət göstərilməsi ilə bağlı qaimə xərcləri",
      "Aktivin istifadəyə hazır vəziyyətə gətirilməsi üçün qaçılmaz olan xaricolmalar"
    ],
    "correct": "Maliyyə fəaliyyəti və mənfəət vergisi ilə əlaqədar pul daxilolmaları və xaricolmaları"
  },
  {
    "num": 155,
    "question": "\"İstifadənin qiymətliliyi\" (Value in Use) hesablanarkən aşağıdakı elementlərdən hansı nəzərə alınmalıdır?",
    "options": [
      "Yalnız aktivin ləğv edilməsindən əldə olunacaq xalis nağd vəsaitlər",
      "Müəssisənin gələcəkdə həyata keçirməyi planlaşdırdığı, lakin hələ öhdəlik götürmədiyi restrukturizasiya faydaları",
      "Mənfəət vergisi üzrə gələcək daxilolmalar və ödənişlər",
      "Gələcək pul axınlarının qiymətləndirilməsi, risksiz faiz dərəcəsi və aktivə xas olan risklər",
      "Aktivin əldə edilməsi üçün cəlb edilmiş borclar üzrə ödənilən faiz xərcləri"
    ],
    "correct": "Gələcək pul axınlarının qiymətləndirilməsi, risksiz faiz dərəcəsi və aktivə xas olan risklər"
  },
  {
    "num": 156,
    "question": "Satışa xərclər çıxılmaqla ədalətli dəyərin qiymətləndirilməsi zamanı aşağıdakılardan hansı aktivin ədalətli dəyərindən çıxılan \"bilavasitə əlavə məsrəflərə\" aid edilmir?",
    "options": [
      "Aktivin kənarlaşdırılmasına çəkilən birbaşa məsrəflər",
      "Aktivin satış vəziyyətinə gətirilməsi üçün zəruri olan müstəqim xərclər",
      "Hüquqi məsrəflər və möhür rüsumları",
      "Sövdələşmədən yaranan oxşar vergilər",
      "İşdənçıxma müavinətləri və fəaliyyətin daraldılması ilə əlaqədar məsrəflər"
    ],
    "correct": "İşdənçıxma müavinətləri və fəaliyyətin daraldılması ilə əlaqədar məsrəflər"
  },
  {
    "num": 157,
    "question": "IAS 36-ya əsasən, aktivin yaxud törədici vahidin \"Ödənilmə dəyəri\" necə müəyyən edilir?",
    "options": [
      "Satış xərcləri çıxılmaqla ədalətli dəyər ilə balans dəyərinin cəmi kimi",
      "Satış xərcləri çıxılmaqla ədalətli dəyər ilə istifadənin qiymətliliyindən daha çox olan kəmiyyət kimi",
      "Aktivin gələcək restrukturizasiya xərcləri daxil olmaqla bazar dəyəri kimi",
      "Aktivin sığorta dəyəri ilə vergitutmadan sonrakı diskontlaşdırılmış pul axınlarının cəmi kimi",
      "Yalnız aktivin ilkin satınalma qiyməti ilə yığılmış amortizasiyanın fərqi kimi"
    ],
    "correct": "Satış xərcləri çıxılmaqla ədalətli dəyər ilə istifadənin qiymətliliyindən daha çox olan kəmiyyət kimi"
  },
  {
    "num": 158,
    "question": "Müəssisə tərəfindən aktivin istifadə üsulunda baş verən hansı dəyişiklik qiymətdəndüşmə indikatoru hesab edilir?",
    "options": [
      "Aktivin bazar dəyərinin balans dəyəri ilə eyni səviyyədə qalması",
      "Aktivin başqa bir törədici vahidə (CGU) daxil edilərək effektivliyinin artırılması",
      "Aktivin əvvəl planlaşdırıldığı tarixdən daha tez təsərrüfatdan çıxarılması və ya restrukturizasiya planları",
      "Aktivin təmir olunaraq istifadə müddətinin uzadılması",
      "Aktivin amortizasiya dərəcəsinin standartlara uyğun olaraq azaldılması"
    ],
    "correct": "Aktivin əvvəl planlaşdırıldığı tarixdən daha tez təsərrüfatdan çıxarılması və ya restrukturizasiya planları"
  },
  {
    "num": 159,
    "question": "Daxili hesabatlardan əldə edilən hansı məlumat aktivin dəyərinin aşağı düşməsinə dəlalət edir?",
    "options": [
      "Aktivin saxlanılması üçün tələb olunan pul vəsaitlərinin azalması",
      "Gələcək dövrlərin büdcə məbləğləri üzrə xalis pul daxilolmalarının artması",
      "Aktivin əldə edilməsi üçün çəkilən xərclərin büdcədəki ilkin məbləğdən daha az olması",
      "Aktivin əməliyyat mənfəətinin büdcə ilə müqayisədə artması",
      "Aktivdən irəli gələn faktiki xalis pul vəsaitləri axınlarının planlaşdırılmış məbləğdən əhəmiyyətli dərəcədə az olması"
    ],
    "correct": "Aktivdən irəli gələn faktiki xalis pul vəsaitləri axınlarının planlaşdırılmış məbləğdən əhəmiyyətli dərəcədə az olması"
  },
  {
    "num": 160,
    "question": "Aşağıdakılardan hansı aktivin qiymətdən düşməsinin \"Daxili əlaməti\" kimi xarakterizə olunur?",
    "options": [
      "Aktivin bazar dəyərinin zaman keçdikcə təbii olaraq azalması",
      "Müəssisənin fəaliyyət göstərdiyi iqtisadi və ya hüquqi şəraitdə əlverişsiz dəyişikliklərin baş verməsi",
      "Bazar mənfəət normalarının dövr ərzində aktivin qiymətinə təsir edəcək dərəcədə yüksəlməsi",
      "Aktivin mənəvi köhnəlməsi, fiziki zədələnməsi və ya aktivin boş dayanması",
      "Aktiv üçün nəzərdə tutulan bazarda texnoloji yeniliklərin rəqabəti artırması"
    ],
    "correct": "Aktivin mənəvi köhnəlməsi, fiziki zədələnməsi və ya aktivin boş dayanması"
  },
  {
    "num": 161,
    "question": "ABŞ-da tətbiq edilən milli uçot prinsipləri sistemi necə adlanır?",
    "options": [
      "IAS",
      "UK GAAP",
      "IFRS",
      "US GAAP",
      "SSAP"
    ],
    "correct": "US GAAP"
  },
  {
    "num": 162,
    "question": "MHBS (IAS) 2 standartı nəyi tənzimləyir?",
    "options": [
      "Qeyri-maddi aktivlər",
      "Torpaq, tikili və avadanlıqlar",
      "Pul vəsaitlərinin hərəkəti",
      "Ehtiyatlar",
      "Səhm üzrə mənfəət"
    ],
    "correct": "Ehtiyatlar"
  },
  {
    "num": 163,
    "question": "2002-ci ilə qədər MHBS Komitəsi (IASC) tərəfindən buraxılmış standartlar hansı abbreviyatura ilə adlandırılır?",
    "options": [
      "IFRS (International Financial Reporting Standards)",
      "IFRIC (Interpretations Committee)",
      "SFAC (Statements on Financial Accounting Concepts)",
      "IAS (International Accounting Standards)",
      "GAAP (Generally Accepted Accounting Principles)"
    ],
    "correct": "IAS (International Accounting Standards)"
  },
  {
    "num": 164,
    "question": "MHBS-larda birbaşa baxılmayan yaxud ziddiyyətli məsələlərə dair göstərişlər hazırlayan orqan hansıdır?",
    "options": [
      "Transmilli Şirkətlərin Birliyi",
      "Monitorinq üzrə Komissiya",
      "MHBS Fondunun Qəyyumçuları",
      "MHBS-ların Şərhləri üzrə Komitə (IFRIC)",
      "Beynəlxalq Ticarət Palatası"
    ],
    "correct": "MHBS-ların Şərhləri üzrə Komitə (IFRIC)"
  },
  {
    "num": 165,
    "question": "Maliyyə Hesabatlılığının Beynəlxalq Standartları üzrə Məsləhət Şurasının (SAC) əsas funksiyası nədir?",
    "options": [
      "Milli standartları ləğv etmək üçün hüquqi qərarlar çıxarmaq",
      "Yalnız Şimali Amerika ölkələri üçün xüsusi uçot qaydaları hazırlamaq",
      "Standartların son variantını təkbaşına təsdiq etmək",
      "Fondun büdcəsini hazırlamaq və maliyyələşməni təmin etmək",
      "İşçi proqramın prioritetləri və layihələr üzrə MHBS Şurasına məsləhətlər vermək"
    ],
    "correct": "İşçi proqramın prioritetləri və layihələr üzrə MHBS Şurasına məsləhətlər vermək"
  },
  {
    "num": 166,
    "question": "MHBS Fondunun strukturuna daxil olan və qəyyumçuları təyin edən, onların fəaliyyətinə nəzarət edən orqan hansıdır?",
    "options": [
      "Məsləhət Şurası",
      "Beynəlxalq Mühasiblər Federasiyası",
      "Regional Audit Departamenti",
      "Monitorinq üzrə Komissiya",
      "Şərhlər üzrə Daimi Komitə"
    ],
    "correct": "Monitorinq üzrə Komissiya"
  },
  {
    "num": 167,
    "question": "MHBS üzrə Şuranın nizamnaməsinə görə, milli standartlarla bağlı əsas hədəfi nədir?",
    "options": [
      "Bütün milli standartların ləğv edilərək yerli dillərdə qalmasını təmin etmək",
      "Milli standartların MHBS ilə konvergensiyasına (yaxınlaşmasına) nail olmaq",
      "Yalnız İslam modelinə uyğun standartlar hazırlamaq",
      "Milli uçot sistemləri arasında fərqləri artırmaq",
      "Milli standartların beynəlxalq standartlardan fərqliliyini qorumaq"
    ],
    "correct": "Milli standartların MHBS ilə konvergensiyasına (yaxınlaşmasına) nail olmaq"
  },
  {
    "num": 168,
    "question": "MHBS Komitəsinin (2001-ci ildən Şura) əsas məqsədlərindən biri hansıdır?",
    "options": [
      "Hər bir ölkə üçün fərqli uçot modelləri tətbiq etmək",
      "Müəssisələrin yalnız daxili idarəetmə hesabatlarını yoxlamaq",
      "Beynəlxalq ticarət dövriyyəsini məhdudlaşdırmaq",
      "Şirkətlərin mənfəət vergisi dərəcələrini müəyyən etmək",
      "Şəffaflığı və müqayisəliliyi təmin edən yüksək keyfiyyətli vahid standartlar hazırlamaq"
    ],
    "correct": "Şəffaflığı və müqayisəliliyi təmin edən yüksək keyfiyyətli vahid standartlar hazırlamaq"
  },
  {
    "num": 169,
    "question": "MHBS Komitəsi (IASC) neçənci ildə və harada yaradılmışdır?",
    "options": [
      "1997-ci ildə, Paris şəhərində",
      "1972-ci ildə, Meksikada",
      "2001-ci ildə, Sidney şəhərində",
      "29 iyun 1973-cü ildə, London şəhərində",
      "1995-ci ildə, Niderlandda"
    ],
    "correct": "29 iyun 1973-cü ildə, London şəhərində"
  },
  {
    "num": 170,
    "question": "Beynəlxalq uçot-hesabat sisteminin (MHBS) yaradılmasını zəruri edən əsas amil hansıdır?",
    "options": [
      "Milli standartların beynəlxalq standartlardan üstün olması",
      "Yalnız yerli mülkiyyətçilərin gəlirlərini müəyyən etmək istəyi",
      "Ölkələrin daxili vergi siyasətini sərtləşdirməsi",
      "İqtisadi qloballaşma və transmilli şirkətlərin (TMŞ) fəaliyyətinin genişlənməsi",
      "İnformasiya texnologiyalarından istifadənin dayandırılması"
    ],
    "correct": "İqtisadi qloballaşma və transmilli şirkətlərin (TMŞ) fəaliyyətinin genişlənməsi"
  },
  {
    "num": 171,
    "question": "Bazar faiz dərəcələrinin yüksəlməsi aktivin qiymətdən düşməsinə necə təsir göstərə bilər?",
    "options": [
      "Bazar faiz dərəcəsi artdıqda aktivin ədalətli dəyəri həmişə balans dəyərinə bərabər olur",
      "Bazar faiz dərəcəsinin artması aktivin balans dəyərinin avtomatik artmasına səbəb olur",
      "Faiz dərəcələrinin yüksəlməsi yalnız müəssisənin borclarına təsir edir, aktivin ödənilmə dəyərinə təsir göstərmir",
      "Bu artım aktivin istifadəsinin qiymətliliyi hesablanarkən istifadə olunan diskontlaşdırma dərəcəsini artırır və ödənilmə dəyərini azaldır",
      "Bu, aktivin faydalı istifadə müddətinin qeyri-müəyyəndən müəyyənə dəyişməsi üçün əsas şərtdir"
    ],
    "correct": "Bu artım aktivin istifadəsinin qiymətliliyi hesablanarkən istifadə olunan diskontlaşdırma dərəcəsini artırır və ödənilmə dəyərini azaldır"
  },
  {
    "num": 172,
    "question": "IAS 36-ya əsasən, aşağıdakılardan hansı aktivin qiymətdən düşməsinin \"Kənar əlaməti\" hesab olunur?",
    "options": [
      "Aktivin mənəvi köhnəlməsi və ya fiziki zədələnməsi əlamətlərinin mövcudluğu",
      "Aktivin faktiki istismar məsrəflərinin büdcədə nəzərdə tutulan məbləğ daxilində olması",
      "Daxili hesabatlara görə aktivin iqtisadi effektivliyinin gözləniləndən pis olması",
      "Müəssisənin xalis aktivlərinin balans dəyərinin onun bazar kapitallaşdırılmasından yüksək olması",
      "Aktivin boş dayanması və ya müəssisənin aktivin aid olduğu fəaliyyəti dayandırmaq planı"
    ],
    "correct": "Müəssisənin xalis aktivlərinin balans dəyərinin onun bazar kapitallaşdırılmasından yüksək olması"
  },
  {
    "num": 173,
    "question": "Hansı hallarda qiymətdəndüşmə testi (balans dəyəri ilə ödənilmə dəyərinin müqayisəsi) əlamətlərin olub-olmamasından asılı olmayaraq hər il aparılmalıdır?",
    "options": [
      "İcarəyə verilmiş və amortizasiya olunmayan bütün binalar üçün",
      "Yalnız fiziki aşınmaya məruz qalan bütün maddi aktivlər üçün",
      "Bütün növ ehtiyatlar və qısamüddətli maliyyə investisiyaları üçün",
      "Qeyri-müəyyən xidmət müddəti olan qeyri-maddi aktivlər və qudvil üçün",
      "Yalnız müəssisə zərərlə işlədiyi illərdə bütün uzunmüddətli aktivlər üçün"
    ],
    "correct": "Qeyri-müəyyən xidmət müddəti olan qeyri-maddi aktivlər və qudvil üçün"
  },
  {
    "num": 174,
    "question": "\"Pul vəsaitləri törədən vahid (törədici vahid)\" anlayışının tərifi hansı variantda düzgün verilmişdir?",
    "options": [
      "Müəssisənin mərkəzi ofisində yerləşən bütün inzibati aktivlərin cəmidir",
      "Qudvilin daxil olduğu və yalnız mənfəət gətirən bütün qeyri-maddi aktivlərdir",
      "Müəssisənin bütün debitor borclarının cəmləşdiyi mühasibat bölməsidir",
      "Digər aktivlərdən asılı olmayaraq pul vəsaitləri daxilolmaları törədən aktivlərin ən az identifikasiya olunan qrupudur",
      "Yalnız xaricdən valyuta gətirən ixrac yönümlü avadanlıqlardır"
    ],
    "correct": "Digər aktivlərdən asılı olmayaraq pul vəsaitləri daxilolmaları törədən aktivlərin ən az identifikasiya olunan qrupudur"
  },
  {
    "num": 175,
    "question": "\"Aktivin yaxud törədici vahidin ödənilmə dəyəri\" dedikdə nə başa düşülür?",
    "options": [
      "Aktivin sığorta dəyəri ilə ləğv etmə dəyərinin orta göstəricisi",
      "Aktivdən gələcəkdə gözlənilən bütün gəlirlərin cəmi (diskontlaşdırılmadan)",
      "Yalnız aktivin bazarındakı ən aşağı satış qiyməti",
      "Aktivin alış qiyməti ilə yığılmış amortizasiyanın cəmi",
      "Satış xərcləri çıxılmaqla ədalətli dəyər ilə istifadənin qiymətliliyindən ən yüksək olanı"
    ],
    "correct": "Satış xərcləri çıxılmaqla ədalətli dəyər ilə istifadənin qiymətliliyindən ən yüksək olanı"
  },
  {
    "num": 176,
    "question": "IAS 36 standartı aşağıdakı aktivlərin hansının qiymətdən düşməsini tənzimləmir?",
    "options": [
      "Filiallarda istifadə olunan kompüter texnikası",
      "Faydalı istifadə müddəti məhdud olan qeyri-maddi aktivlər",
      "İstehsalat avadanlıqları və binalar",
      "Ehtiyatlar, maliyyə aktivləri və satış üçün nəzərdə tutulan uzunmüddətli aktivlər",
      "Müəssisənin öz fəaliyyətində istifadə etdiyi torpaq sahələri"
    ],
    "correct": "Ehtiyatlar, maliyyə aktivləri və satış üçün nəzərdə tutulan uzunmüddətli aktivlər"
  },
  {
    "num": 177,
    "question": "IAS 36 əsasən, aktiv nə zaman qiymətdən düşmüş hesab edilir?",
    "options": [
      "Aktivin bazar qiyməti onun ilkin alış dəyərindən yuxarı qalxdıqda",
      "Aktiv yalnız fiziki olaraq sıradan çıxdıqda",
      "Aktiv tam amortizasiya olunduqdan sonra hələ də istifadə edildikdə",
      "Aktivin balans dəyəri onun ödənilmə dəyərini (istifadə və ya satış yolu ilə əldə ediləcək məbləği) aşdıqda",
      "Aktivin faydalı istifadə müddəti 10 ildən çox olduqda"
    ],
    "correct": "Aktivin balans dəyəri onun ödənilmə dəyərini (istifadə və ya satış yolu ilə əldə ediləcək məbləği) aşdıqda"
  },
  {
    "num": 178,
    "question": "Borclanmalar üzrə məsrəflərin kapitallaşdırılması zamanı hesabatlarda hansı göstərici barədə məlumat verilməlidir?",
    "options": [
      "Kredit götürülərkən girov qoyulmuş aktivlərin bazar qiyməti",
      "Borc vəsaitlərinin alındığı gün mövcud olan rəsmi inflyasiya dərəcəsi",
      "Müəssisənin nizamnamə kapitalının borclara olan nisbəti",
      "Borclanmaların kapitallaşdırılması üçün istifadə edilmiş kapitallaşdırılma stavkası (faizi)",
      "Borc müqaviləsinin imzalanması üçün çəkilən hüquqi xərclərin dərəcəsi"
    ],
    "correct": "Borclanmaların kapitallaşdırılması üçün istifadə edilmiş kapitallaşdırılma stavkası (faizi)"
  },
  {
    "num": 179,
    "question": "IAS 23-ə əsasən, təşkilat borclanmalar üzrə məsrəflərə dair maliyyə hesabatlarında hansı məbləği mütləq açıqlamalıdır?",
    "options": [
      "Borc vəsaitlərini təqdim edən bankların və digər kreditorların siyahısını",
      "Müəssisənin cəlb etdiyi borclar üzrə ödənilmiş komissiya haqlarının ümumi məbləğini",
      "Gələcək 10 il ərzində ödənilməsi planlaşdırılan bütün faiz xərclərinin cəmini",
      "Yalnız vergi uçotunda nəzərə alınan faiz xərclərinin məbləğini",
      "Hesabat dövrü ərzində aktivlərin ilkin dəyərinə daxil edilmiş (kapitallaşdırılmış) borclanma məsrəflərinin məbləğini"
    ],
    "correct": "Hesabat dövrü ərzində aktivlərin ilkin dəyərinə daxil edilmiş (kapitallaşdırılmış) borclanma məsrəflərinin məbləğini"
  },
  {
    "num": 180,
    "question": "Çoxsaylı binalardan ibarət kompleksin bir hissəsi istifadəyə hazır olduqda, lakin digər hissələrində tikinti davam etdikdə kapitallaşdırma necə tənzimlənir?",
    "options": [
      "Hazır olan hissənin də faizləri tikinti bitənə qədər kapitallaşdırılır",
      "Bütün kompleks tam hazır olana qədər kapitallaşdırma bütün hissələr üçün davam edir",
      "Hazır olan hissə vahid kvalifikasiya olunan aktiv kimi tanınmır",
      "Bütün kompleks üzrə kapitallaşdırma dərhal dayandırılır və xərcə silinir",
      "Hazır olan hissə üçün kapitallaşdırma dayandırılır, tikintisi davam edən hissələr üçün isə davam etdirilir"
    ],
    "correct": "Hazır olan hissə üçün kapitallaşdırma dayandırılır, tikintisi davam edən hissələr üçün isə davam etdirilir"
  },
  {
    "num": 181,
    "question": "Borclanmalar üzrə məsrəflərin kapitallaşdırılması nə vaxt dayandırılmalıdır?",
    "options": [
      "Aktivin istismara verilməsindən 1 il keçdikdən sonra",
      "Müəssisənin maliyyə ilinin sonu çatdıqda",
      "Tikinti sahəsindəki inzibati işlər hələ davam etdiyi müddətdə",
      "Aktivin təyinatı üzrə istifadəyə və ya satışa hazır olması üçün bütün işlər praktiki olaraq bitdikdə",
      "Borc vəsaitləri banka tam geri qaytarıldıqdan sonra"
    ],
    "correct": "Aktivin təyinatı üzrə istifadəyə və ya satışa hazır olması üçün bütün işlər praktiki olaraq bitdikdə"
  },
  {
    "num": 182,
    "question": "Aşağıdakı hallardan hansında kapitallaşdırma prosesi saxlanılmalı (ara verilməli) və çəkilən faizlər xərc kimi tanınmalıdır?",
    "options": [
      "Binanın rəsmi sənədləşmə işlərinin aparıldığı dövrdə",
      "Çayın səviyyəsinin qalxması kimi təbii proseslərin körpü tikintisini müvəqqəti ləngitdiyi dövrdə",
      "Tikintinin başlanması üçün inzibati və texniki işlərin aparıldığı dövrdə",
      "Aktivin inkişafına (tikintisinə) xeyli müddət ara verildiyi dövrlərdə (məsələn, istehsalın dayandırılması)",
      "Tikinti davam edərkən mühəndislərin layihə üzərində texniki dəyişikliklər etdiyi qısa müddətdə"
    ],
    "correct": "Aktivin inkişafına (tikintisinə) xeyli müddət ara verildiyi dövrlərdə (məsələn, istehsalın dayandırılması)"
  },
  {
    "num": 183,
    "question": "Borclanmalar üzrə məsrəflərin kapitallaşdırılmasına başlamaq üçün hansı şərtlərin hamısı eyni vaxtda yerinə yetirilməlidir?",
    "options": [
      "Aktiv üzrə gələcək amortizasiya xərcləri qabaqcadan hesablanıb təsdiq edilməlidir",
      "Yalnız tikintinin fiziki olaraq başa çatması barədə rəsmi icazə alınmalıdır",
      "Aktiv üzrə məsrəflər çəkilməli, borclanma məsrəfləri yaranmalı və aktivin hazırlanması üçün zəruri fəaliyyət aparılmalıdır",
      "Tikinti üçün bütün materiallar anbara daxil olmalı və işçilərin maaşı ödənilməlidir",
      "Borc vəsaiti bank hesabına daxil olmalı və müəssisə mənfəət əldə etməyə başlamalıdır"
    ],
    "correct": "Aktiv üzrə məsrəflər çəkilməli, borclanma məsrəfləri yaranmalı və aktivin hazırlanması üçün zəruri fəaliyyət aparılmalıdır"
  },
  {
    "num": 184,
    "question": "Borclanma məsrəflərinin aktivin ilkin dəyərinə daxil edilməsi (kapitallaşdırılması) üçün hansı şərtlər ödənilməlidir?",
    "options": [
      "Kapitallaşdırma yalnız audit yoxlaması başa çatdıqdan sonra həyata keçirilməlidir",
      "Borcun məbləği aktivin dəyərindən mütləq çox olmalıdır",
      "Aktiv mütləq xarici valyuta ilə əldə edilməlidir",
      "Gələcək iqtisadi faydaların götürülməsi ehtimal olunmalı və məsrəflər etibarlı ölçülməlidir",
      "Borc yalnız dövlət banklarından alınmalıdır"
    ],
    "correct": "Gələcək iqtisadi faydaların götürülməsi ehtimal olunmalı və məsrəflər etibarlı ölçülməlidir"
  },
  {
    "num": 185,
    "question": "Aşağıdakı maddələrdən hansı kvalifikasiya olunan aktiv hesab edilə bilər?",
    "options": [
      "Mütəmadi əsasda və çox qısa zamanda kütləvi istehsal edilən mallar",
      "Müəssisənin bank hesabındakı pul vəsaitləri",
      "Səhmlər, istiqrazlar və digər maliyyə aktivləri",
      "İstehsal gücləri, elektrik istehsal edən güclər və investisiyalı daşınmaz əmlak",
      "Əldə olunduğu gün mağazada satışa qoyulan hazır məhsullar"
    ],
    "correct": "İstehsal gücləri, elektrik istehsal edən güclər və investisiyalı daşınmaz əmlak"
  },
  {
    "num": 186,
    "question": "Standarta əsasən, \"Kvalifikasiya olunan aktiv\" nədir?",
    "options": [
      "Qısa vaxt dövründə (məsələn, 1 həftə) istehsal edilən bütün ehtiyatlardır",
      "Yalnız ədalətli dəyərlə qiymətləndirilən bioloji aktivlərdir",
      "Əldə olunduğu anda dərhal istifadəyə və ya satışa hazır olan aktivdir",
      "Müəssisənin sahib olduğu bütün maliyyə aktivləri və debitor borclarıdır",
      "Təyinatı üzrə istifadəsi və ya satışı üçün hazırlanmasına əhəmiyyətli vaxt tələb olunan aktivdir"
    ],
    "correct": "Təyinatı üzrə istifadəsi və ya satışı üçün hazırlanmasına əhəmiyyətli vaxt tələb olunan aktivdir"
  },
  {
    "num": 187,
    "question": "MHBS (IAS) 23 standartının əsas prinsipi nədən ibarətdir?",
    "options": [
      "Bütün borclanma məsrəfləri çəkildiyi dövrdə birbaşa xərc kimi tanınmalıdır",
      "Borclanma məsrəfləri yalnız nizamnamə kapitalının artırılmasına yönəldilir",
      "Faizin kapitallaşdırılması yalnız dövlət tərəfindən verilən borclara şamil edilir",
      "Kvalifikasiya olunan aktivin əldə edilməsi və ya tikintisinə aid olan borclanma məsrəfləri həmin aktivin ilkin dəyərinə daxil edilir (kapitallaşdırılır)",
      "Borclanma məsrəfləri yalnız aktiv tam hazır olduqdan sonra mənfəət və zərərdə əks olunur"
    ],
    "correct": "Kvalifikasiya olunan aktivin əldə edilməsi və ya tikintisinə aid olan borclanma məsrəfləri həmin aktivin ilkin dəyərinə daxil edilir (kapitallaşdırılır)"
  },
  {
    "num": 188,
    "question": "Gəlirə aid edilən subsidiyanın qaytarılan məbləği mövcud təxirəsalınmış gəlir qalığından çox olarsa, bu artıq hissə harada əks etdirilməlidir?",
    "options": [
      "Şübhəli borclar üzrə ehtiyatda",
      "Yalnız qeydlərdə (şərti öhdəlik kimi)",
      "Gələcək illərin daxilolmalarında",
      "Qeyri-maddi aktivlərin tərkibində",
      "Bilavasitə mənfəət yaxud zərərdə"
    ],
    "correct": "Bilavasitə mənfəət yaxud zərərdə"
  },
  {
    "num": 189,
    "question": "Aşağıdakılardan hansı MHBS (IAS) 20-yə görə maliyyə hesabatlarında açıqlanmalı olan informasiyalara aid DEYİL?",
    "options": [
      "Subsidiyaların uçotu və təqdim edilməsi üçün qəbul edilmiş metodlar",
      "Təşkilatın birbaşa fayda aldığı dövlət yardımının digər formaları barədə məlumatlar",
      "Tanınmış subsidiyalarla bağlı yerinə yetirilməmiş şərtlər və sair mümkün şəraitlər",
      "Subsidiyanı verən dövlət məmurlarının siyahısı və onların vəzifələri",
      "Maliyyə hesabatlarında tanınmış subsidiyaların xarakteri və həcmi"
    ],
    "correct": "Subsidiyanı verən dövlət məmurlarının siyahısı və onların vəzifələri"
  },
  {
    "num": 190,
    "question": "Aktivə aid edilən subsidiyanın (balans dəyərindən çıxılma metodu tətbiq edildikdə) qaytarılması zamanı uçotda hansı dəyişiklik baş verir?",
    "options": [
      "Yalnız maliyyə fəaliyyəti üzrə pul vəsaitlərinin hərəkəti maddəsində qeyd olunur",
      "Aktiv dərhal balansdan silinərək xərcə verilir",
      "Aktivin balans dəyəri daha da azaldılır və dövlətə əlavə faiz ödənilir",
      "Aktivin balans dəyəri artırılır və subsidiyanın olmaması halında yaranacaq əlavə amortizasiya mənfəət və zərərdə tanınır",
      "Aktivin faydalı istifadə müddəti yenidən sıfırlanır"
    ],
    "correct": "Aktivin balans dəyəri artırılır və subsidiyanın olmaması halında yaranacaq əlavə amortizasiya mənfəət və zərərdə tanınır"
  },
  {
    "num": 191,
    "question": "Gəlirə aid edilən subsidiya qaytarılarkən, qaytarılan məbləğ ilk növbədə hansı maddənin azaldılmasına aid edilir?",
    "options": [
      "Maddi ehtiyatların maya dəyərinə",
      "Müəssisənin cari dövr üzrə xalis mənfəətinə",
      "Nizamnamə kapitalının ümumi məbləğinə",
      "Həmin subsidiyaya aid təxirəsalınmış gəlirin amortizasiya olunmamış qalığına",
      "Uzunmüddətli bank kreditləri üzrə borclara"
    ],
    "correct": "Həmin subsidiyaya aid təxirəsalınmış gəlirin amortizasiya olunmamış qalığına"
  },
  {
    "num": 192,
    "question": "Kadrların yığılması üçün alınan 180 000 p.v. həcmində subsidiya 3 ilə bölüşdürülürsə, ikinci alternativ metoda görə illik mühabirləşmə necə olar?",
    "options": [
      "DT Aktivlər (60 000) — KT Sair gəlirlər (60 000)",
      "DT Bank hesabı (60 000) — KT Təxirə salınmış gəlir (60 000)",
      "DT Kadr yığılması xərcləri (60 000) — KT Mənfəət və zərər (60 000)",
      "DT Təxirə salınmış gəlir (60 000) — KT Kadr yığılması xərcləri (60 000)",
      "DT Təxirə salınmış gəlir (180 000) — KT Bank hesabı (180 000)"
    ],
    "correct": "DT Təxirə salınmış gəlir (60 000) — KT Kadr yığılması xərcləri (60 000)"
  },
  {
    "num": 193,
    "question": "Təşkilat dövr ərzində maliyyə aktivini yenidən təsnifləşdirərsə (reclassification), nəyi açıqlamalıdır?",
    "options": [
      "Yalnız həmin aktivin alındığı ölkəni",
      "Bazarın son 10 ildəki orta qiymət statistikasını",
      "Auditorun şəxsi rəyini və tərcümeyi-halını",
      "Yenidəntəsnifləşdirilmiş məbləğləri və bunun səbəblərini",
      "Müəssisənin bütün bank hesablarının nömrələrini"
    ],
    "correct": "Yenidəntəsnifləşdirilmiş məbləğləri və bunun səbəblərini"
  },
  {
    "num": 194,
    "question": "MHBS (IFRS) 7-yə əsasən, maliyyə vəziyyəti haqqında hesabatda hansı kateqoriya üzrə balans dəyəri açıqlanmalıdır?",
    "options": [
      "Müəssisənin bütün qeyri-maliyyə aktivləri",
      "Gələcəkdə gözlənilən mümkün satışlar",
      "İşçilərin say tərkibi və əmək haqqı fondu",
      "Amortizasiya olunan dəyərlə qiymətləndirilən maliyyə öhdəlikləri",
      "Yalnız nağd satışdan gələn gəlirlər"
    ],
    "correct": "Amortizasiya olunan dəyərlə qiymətləndirilən maliyyə öhdəlikləri"
  },
  {
    "num": 195,
    "question": "Xüsusi pay alətlərinin emissiyasından yaxud satın alınmasından yaranan mənfəət və ya zərər harada tanınmalıdır?",
    "options": [
      "Təxirə salınmış vergi aktivlərində",
      "Mənfəət və zərər hesabatında",
      "Sair əməliyyat gəlirlərində",
      "Xüsusi kapitalda",
      "Gələcək illərin xərclərində"
    ],
    "correct": "Xüsusi kapitalda"
  },
  {
    "num": 196,
    "question": "Təşkilatın öz xüsusi səhmlərini satın alması maliyyə hesabatında necə əks olunur?",
    "options": [
      "Mənfəət və zərər hesabatında gəlir kimi tanınır",
      "Amortizasiya olunan qeyri-maddi aktiv kimi uçota alınır",
      "Uzunmüddətli öhdəliklər bölməsində artırılır",
      "Xüsusi kapitaldan çıxılır",
      "Aktivlərin tərkibində debitor borcu kimi göstərilir"
    ],
    "correct": "Xüsusi kapitaldan çıxılır"
  },
  {
    "num": 197,
    "question": "Mürəkkəb maliyyə alətlərinə (məsələn, səhmlərə konvertasiya oluna bilən istiqrazlar) dair hansı fikir doğrudur?",
    "options": [
      "Bu alətlər üzrə faizlər dividendlər kimi uçota alınır",
      "Onlar yalnız mənfəət və zərər hesabatında xərc kimi tanınır",
      "Onlar heç vaxt xüsusi kapitalda əks etdirilə bilməz",
      "Onlar həm öhdəlik, həm də sahibinə gələcəkdə səhmə dəyişmək hüququ verən komponenti birləşdirir",
      "Onlar yalnız nağd pul vəsaiti kimi təsnifləşdirilir"
    ],
    "correct": "Onlar həm öhdəlik, həm də sahibinə gələcəkdə səhmə dəyişmək hüququ verən komponenti birləşdirir"
  },
  {
    "num": 198,
    "question": "Gəlirə aid edilən subsidiyalar mənfəət və zərər hesabatında hansı formada təqdim edilə bilər?",
    "options": [
      "Ya alış qiymətinə əlavə edilir, ya da satış qiymətindən çıxılır",
      "Ya nizamnamə kapitalında əks olunur, ya da uzunmüddətli öhdəlik kimi tanınır",
      "Ya pul vəsaitlərinin hərəkəti hesabatında, ya da kapitalda dəyişikliklər hesabatında",
      "Ya ayrıca/ümumi maddədə (\"Sair gəlirlər\") göstərilir, ya da müvafiq xərclərdən çıxılır",
      "Ya xalis mənfəətin tərkibində, ya da aktivlərin silinməsində"
    ],
    "correct": "Ya ayrıca/ümumi maddədə (\"Sair gəlirlər\") göstərilir, ya da müvafiq xərclərdən çıxılır"
  },
  {
    "num": 199,
    "question": "Balans dəyərindən çıxılma əsasən, subsidiyanın mənfəət və zərərə təsiri necə baş verir?",
    "options": [
      "Aktivin bazar dəyərinin yenidən qiymətləndirilməsi nəticəsində yaranan fərq kimi",
      "Aktivin faydalı istifadə müddətinin uzadılması hesabına",
      "\"Sair əməliyyat gəlirləri\" maddəsində məbləğin artması ilə",
      "Müəssisənin vergi öhdəliyinin birbaşa artması ilə",
      "Amortizasiya üzrə xərclərin azalması qismində (çünki aktivin maya dəyəri azalır)"
    ],
    "correct": "Amortizasiya üzrə xərclərin azalması qismində (çünki aktivin maya dəyəri azalır)"
  },
  {
    "num": 200,
    "question": "Təxirə salınmış gəlir metoduna əsasən, aktiv üçün alınmış subsidiya mənfəət və ya zərər hesabatında necə tanınır?",
    "options": [
      "Yalnız müəssisə mənfəət əldə etdiyi illərdə dividend kimi",
      "Yalnız aktiv tam aşındıqdan sonra qalıq dəyəri kimi",
      "Aktivin faydalı istifadə müddəti ərzində sistematik əsasda gəlir kimi",
      "Aktiv istismara verildiyi gün birbaşa kapitalın artımı kimi",
      "Subsidiyanın alındığı tarixdə bütün məbləğ birdəfəlik gəlir kimi"
    ],
    "correct": "Aktivin faydalı istifadə müddəti ərzində sistematik əsasda gəlir kimi"
  },
  {
    "num": 201,
    "question": "Aktivlərə aid edilən dövlət subsidiyalarının Maliyyə Vəziyyəti Haqqında Hesabatda (Balansda) təqdim edilməsi üçün hansı alternativ metodlar mövcuddur?",
    "options": [
      "Subsidiyanı ya nizamnamə kapitalına əlavə etmək, ya da birbaşa xərcə silmək",
      "Subsidiyanı ya satışın maya dəyərinə aid etmək, ya da bölüşdürülməmiş mənfəətdə gizlətmək",
      "Subsidiyanı ya təxirəsalınmış gəlir kimi əks etdirmək, ya da aktivin balans dəyərindən çıxmaq",
      "Subsidiyanı ya debitor borc kimi göstərmək, ya da ehtiyatlara daxil etmək",
      "Subsidiyanı ya qeyri-maddi aktiv kimi tanımaq, ya da maliyyə xərcləri ilə əvəzləşdirmək"
    ],
    "correct": "Subsidiyanı ya təxirəsalınmış gəlir kimi əks etdirmək, ya da aktivin balans dəyərindən çıxmaq"
  },
  {
    "num": 202,
    "question": "Şərti-geriqaytarılmayan borclar nə vaxt dövlət subsidiyası kimi qəbul edilir?",
    "options": [
      "Borc müqaviləsi bağlandığı ilk gündən etibarən",
      "Yalnız borcun məbləği 1 milyon manatdan çox olduqda",
      "Borcun faizləri vaxtında ödənildikdə",
      "Şərtlərin yerinə yetiriləcəyinə və borcun bağışlanacağına ağlabatan inam olduqda",
      "Müəssisə iflas həddinə çatdıqda"
    ],
    "correct": "Şərtlərin yerinə yetiriləcəyinə və borcun bağışlanacağına ağlabatan inam olduqda"
  },
  {
    "num": 203,
    "question": "Artıq çəkilmiş xərclərin kompensasiyası üçün verilən subsidiyalar nə vaxt mənfəət və ya zərərdə tanınır?",
    "options": [
      "Növbəti 10 il ərzində tədricən",
      "Yalnız müəssisə mənfəətlə işlədiyi ilin sonunda",
      "Alınmalı olduğu (və ya alındığı) dövrün mənfəət-zərərində",
      "Aktiv tam köhnəldikdən sonra",
      "Subsidiyanın məbləği tam xərcləndiyi tarixdə"
    ],
    "correct": "Alınmalı olduğu (və ya alındığı) dövrün mənfəət-zərərində"
  },
  {
    "num": 204,
    "question": "Təşkilatın əməliyyat fəaliyyəti ilə əlaqədar şərtlər müqabilində dövlət tərəfindən resursların verilməsi necə adlanır?",
    "options": [
      "Nizamnamə kapitalı",
      "İnvestisiya mənfəəti",
      "Şərti öhdəlik",
      "Dövlət subsidiyası",
      "Vergi tətili"
    ],
    "correct": "Dövlət subsidiyası"
  },
  {
    "num": 205,
    "question": "Qeyri-monetar dövlət subsidiyaları (məsələn, torpaq və ya avadanlıq) adətən hansı dəyərlə tanınır?",
    "options": [
      "Müəssisənin təyin etdiyi daxili qiymətlə",
      "Yalnız ləğv etmə dəyəri ilə",
      "Öncəki illərin orta satış qiyməti ilə",
      "Yalnız vergi uçotu qaydalarına uyğun qiymətlə",
      "Ədalətli dəyərlə"
    ],
    "correct": "Ədalətli dəyərlə"
  },
  {
    "num": 206,
    "question": "Aktivlərə aid edilən subsidiyalar dedikdə nə başa düşülür?",
    "options": [
      "Yalnız cari əməliyyat xərclərini ödəmək üçün verilən yardımlar",
      "İşçilərin əməkhaqqının ödənilməsi üçün nəzərdə tutulan vəsaitlər",
      "Yalnız qısamüddətli aktivlərin (stokların) alınması üçün verilən pullar",
      "Əsas şərti uzunmüddətli aktivin alınması, tikilməsi və ya əldə edilməsi olan subsidiyalar",
      "Vergi borclarının silinməsi formasında olan güzəştlər"
    ],
    "correct": "Əsas şərti uzunmüddətli aktivin alınması, tikilməsi və ya əldə edilməsi olan subsidiyalar"
  },
  {
    "num": 207,
    "question": "Maliyyə öhdəliyi maliyyə vəziyyəti haqqında hesabatdan (balansdan) nə zaman çıxarılır?",
    "options": [
      "Kreditorla danışıqlara başlandığı anda",
      "Hesabat dövrü başa çatdıqdan dərhal sonra",
      "Öhdəliyin məbləği rəhbərlik tərəfindən çox hesab edildikdə",
      "Şirkətin səhmlərinin qiyməti artdıqda",
      "Öhdəçilik icra edildikdə, ləğv edildikdə yaxud müddəti bitdikdə"
    ],
    "correct": "Öhdəçilik icra edildikdə, ləğv edildikdə yaxud müddəti bitdikdə"
  },
  {
    "num": 208,
    "question": "Maliyyə aktivinin tanınmasının tam dayandırılması zamanı yaranan fərq harada əks etdirilməlidir?",
    "options": [
      "Yalnız xüsusi kapitalda",
      "Vergi ehtiyatlarında",
      "Şərti aktivlər hesabında",
      "Mənfəət yaxud zərərlərin tərkibində",
      "Gələcək dövrlərin gəlirlərində"
    ],
    "correct": "Mənfəət yaxud zərərlərin tərkibində"
  },
  {
    "num": 209,
    "question": "Təşkilat maliyyə aktivinin tanınmasını hansı halda dayandırır?",
    "options": [
      "Aktivin amortizasiya müddəti yarıya çatdıqda",
      "Debitor borcu ödənilməmişdən əvvəl yenidən təsnifləşdirildikdə",
      "Müqavilə bağlandığı tarixdən bir il keçdikdə",
      "Aktivin bazar qiyməti müvəqqəti olaraq aşağı düşdükdə",
      "Müqavilə üzrə aktivdən pul axınlarının alınması hüququnun müddəti bitdikdə və ya aktiv verildikdə"
    ],
    "correct": "Müqavilə üzrə aktivdən pul axınlarının alınması hüququnun müddəti bitdikdə və ya aktiv verildikdə"
  },
  {
    "num": 210,
    "question": "MHBS (IFRS) 9-a əsasən, hansı növ maliyyə aktivləri üçün gözlənilən kredit zərərləri üzrə rezerv (ehtiyat) tanınmalıdır?",
    "options": [
      "Yalnız müəssisənin öz səhmləri üçün",
      "Yalnız nağd pul vəsaitləri üçün",
      "Yalnız mənfəət yaxud zərər vasitəsilə ədalətli dəyərlə qiymətləndirilən aktivlər üçün",
      "Amortizasiya olunan dəyərlə və sair məcmu gəlir vasitəsilə ədalətli dəyərlə qiymətləndirilən maliyyə aktivləri üçün",
      "Heç bir maliyyə aktivi üçün rezerv tanınmır"
    ],
    "correct": "Amortizasiya olunan dəyərlə və sair məcmu gəlir vasitəsilə ədalətli dəyərlə qiymətləndirilən maliyyə aktivləri üçün"
  },
  {
    "num": 211,
    "question": "Maliyyə aktivlərinin sonrakı qiymətləndirilməsi üçün tətbiq edilən effektiv faiz stavkası metodunun əsas məqsədi nədir?",
    "options": [
      "Aktivin ilkin dəyərini olduğu kimi saxlamaq",
      "Vergi tutulan mənfəəti süni şəkildə azaltmaq",
      "Aktivin bazar qiymətinin dəyişməsini hər gün izləmək",
      "Yalnız debitor borclarının silinməsi üçün rezerv yaratmaq",
      "Amortizasiya olunan dəyərin hesablanması və faiz gəlir/xərclərinin müvafiq dövrlər üzrə bölüşdürülməsi"
    ],
    "correct": "Amortizasiya olunan dəyərin hesablanması və faiz gəlir/xərclərinin müvafiq dövrlər üzrə bölüşdürülməsi"
  },
  {
    "num": 212,
    "question": "Maliyyə aktivinin balans dəyərini gələcək pul daxilolmalarına dəqiqliklə bərabər edən diskontlaşdırma dərəcəsi necə adlanır?",
    "options": [
      "Effektiv faiz stavkası",
      "Bazar faiz dərəcəsi",
      "Nominal faiz dərəcəsi",
      "Sabit faiz dərəcəsi",
      "İnflyasiya dərəcəsi"
    ],
    "correct": "Effektiv faiz stavkası"
  },
  {
    "num": 213,
    "question": "Əhəmiyyətli maliyyələşdirmə komponentinə malik olmayan ticarət debitor borcları ilkin olaraq hansı qiymətlə tanınır?",
    "options": [
      "Nominal dəyərlə",
      "Bazar qiyməti ilə",
      "Gələcək pul axınlarının diskontlaşdırılmış dəyəri ilə",
      "Maya dəyəri ilə",
      "Sövdələşmə qiyməti ilə"
    ],
    "correct": "Sövdələşmə qiyməti ilə"
  },
  {
    "num": 214,
    "question": "Mənfəət yaxud zərər vasitəsilə ədalətli dəyərlə qiymətləndirilməyən maliyyə aktivlərinin ilkin tanınması zamanı sövdələşmə məsrəfləri necə uçota alınır?",
    "options": [
      "Aktivin ömrü boyu amortizasiya edilir",
      "Uçotda ümumiyyətlə əks etdirilmir",
      "Ədalətli dəyərdən çıxılır",
      "Birbaşa mənfəət və zərər hesabatına xərc kimi yazılır",
      "Ədalətli dəyərin üzərinə əlavə edilir"
    ],
    "correct": "Ədalətli dəyərin üzərinə əlavə edilir"
  },
  {
    "num": 215,
    "question": "Aşağıdakılardan hansı maliyyə aktivlərinin təsnifləşdirildiyi qruplardan biri deyil?",
    "options": [
      "İlkin tanınma zamanı mənfəət/zərər vasitəsilə təsnifləşdirilən aktivlər",
      "Amortizasiya olunan dəyərlə qiymətləndirilən maliyyə aktivləri",
      "Sair məcmu gəlir vasitəsilə ədalətli dəyərlə qiymətləndirilən maliyyə aktivləri",
      "Maddi ehtiyatlar vasitəsilə qiymətləndirilən maliyyə aktivləri",
      "Mənfəət yaxud zərər vasitəsilə ədalətli dəyərlə qiymətləndirilən maliyyə aktivləri"
    ],
    "correct": "Maddi ehtiyatlar vasitəsilə qiymətləndirilən maliyyə aktivləri"
  },
  {
    "num": 216,
    "question": "Dövlət subsidiyasının tanınması üçün əsas şərt hansıdır?",
    "options": [
      "Təşkilatın maliyyə hesabatlarının auditdən keçməsi",
      "Subsidiyanın yalnız nağd pul şəklində kassaya daxil olması",
      "Dövlət orqanı tərəfindən rəsmi məktubun göndərilməsi",
      "Aktivin istismar müddətinin başa çatması",
      "Şərtlərin yerinə yetiriləcəyinə və subsidiyanın alınacağına ağlabatan inamın olması"
    ],
    "correct": "Şərtlərin yerinə yetiriləcəyinə və subsidiyanın alınacağına ağlabatan inamın olması"
  },
  {
    "num": 217,
    "question": "Standarta əsasən, aşağıdakılardan hansı \"Dövlət yardımı\" hesab olunmur?",
    "options": [
      "Şərti-geriqaytarılmayan borcların bağışlanması",
      "Müəyyən meyarlara cavab verən müəssisələrə resurs transferi",
      "Müəyyən təşkilata iqtisadi fayda verən hərəkətlər",
      "Bazar faizindən aşağı dərəcə ilə verilən kreditlər",
      "İnkişaf edən rayonlarda yaradılmış ümumi infrastrukturlar"
    ],
    "correct": "İnkişaf edən rayonlarda yaradılmış ümumi infrastrukturlar"
  },
  {
    "num": 218,
    "question": "MHBS (IAS) 20 standartının tətbiq sferasına aşağıdakılardan hansı daxil deyil?",
    "options": [
      "Aktivlərə aid edilən subsidiyalar",
      "Keçmiş xərclərin kompensasiyası üçün alınan subsidiyalar",
      "Pul vəsaiti formasında alınan birbaşa yardımlar",
      "Dövlətin təşkilatın kapitalında iştirakı",
      "Gəlirə aid edilən subsidiyalar"
    ],
    "correct": "Dövlətin təşkilatın kapitalında iştirakı"
  },
  {
    "num": 219,
    "question": "QMA-nın ləğv dəyəri hansı halda sıfırdan fərqli (müsbət məbləğ) götürülə bilər?",
    "options": [
      "Yalnız aktiv daxildə yaradıldıqda",
      "Müəssisə rəhbərliyi istədiyi istənilən halda",
      "Aktivin maya dəyəri 500.000 manatdan çox olduqda",
      "Aktivin istifadə müddətinin sonunda onu almağa hazır olan üçüncü tərəf və ya aktiv bazar mövcud olduqda",
      "Aktivin fiziki forması olduğu halda"
    ],
    "correct": "Aktivin istifadə müddətinin sonunda onu almağa hazır olan üçüncü tərəf və ya aktiv bazar mövcud olduqda"
  },
  {
    "num": 220,
    "question": "QMA-nın amortizasiyası nə zaman başlayır?",
    "options": [
      "Aktivin satınalma müqaviləsi imzalandığı tarixdən",
      "Aktiv üçün ilk sifariş daxil olduğu tarixdən",
      "Layihənin tədqiqat mərhələsi bitdiyi andan",
      "Aktiv rəhbərliyin niyyətinə uyğun istifadə üçün hazır vəziyyətdə olduğu andan",
      "Aktiv tam istismara verilib ilk gəliri gətirdikdən bir il sonra"
    ],
    "correct": "Aktiv rəhbərliyin niyyətinə uyğun istifadə üçün hazır vəziyyətdə olduğu andan"
  },
  {
    "num": 221,
    "question": "QMA-nın yenidənqiymətləndirilməsi nəticəsində yaranan ARTIM (əvvəllər zərər olmayıbsa) harada əks olunur?",
    "options": [
      "Xalis mənfəətin bölüşdürülməsində",
      "Satışdan gələn gəlir kimi mənfəət və zərər hesabatında",
      "Kapitalda \"Yenidənqiymətləndirilmə ehtiyatı\" (artımı) adı altında",
      "Cəmi aktivlərin azaldılmasında",
      "Birbaşa hesabat dövrünün əməliyyat gəlirlərində"
    ],
    "correct": "Kapitalda \"Yenidənqiymətləndirilmə ehtiyatı\" (artımı) adı altında"
  },
  {
    "num": 222,
    "question": "Şirkətin daxilində yaradılmış \"İşgüzar imic\" (Qudvil) haqqında hansı mülahizə doğrudur?",
    "options": [
      "O, patent və lisenziyalarla eyni qrupda uçota alınır",
      "Yalnız daxili resurslar hesabına yaradıldıqda amortizasiya olunur",
      "Daxildə yaradılan işgüzar imic aktiv kimi tanınmamalıdır",
      "O, identifikasiya oluna bilən ayrıca aktivdir",
      "O, mütləq ədalətli dəyərlə hər il yenidən qiymətləndirilməlidir"
    ],
    "correct": "Daxildə yaradılan işgüzar imic aktiv kimi tanınmamalıdır"
  },
  {
    "num": 223,
    "question": "Aktiv bazarın mövcud olması QMA-lar üçün hansı uçot modelinin tətbiqi üçün zəruridir?",
    "options": [
      "İlkin qiymətləndirmə modeli",
      "Yenidənqiymətləndirilmə modeli",
      "Tarixi xərc modeli",
      "Likvidasiya dəyəri modeli",
      "Maya dəyəri modeli"
    ],
    "correct": "Yenidənqiymətləndirilmə modeli"
  },
  {
    "num": 224,
    "question": "Faydalı istifadə müddəti \"Qeyri-müəyyən\" (Məlum olmayan) olan QMA-lar üçün hansı uçot qaydası tətbiq edilir?",
    "options": [
      "Faydalı ömrü qeyri-müəyyən olan QMA amortizasiya olunmur. Hər il və qiymətdəndüşmə əlaməti olduqda qiymətdəndüşmə testi aparılır, həmçinin ömrün qeyri-müəyyən qalıb-qalmadığı hər dövr yenidən nəzərdən keçirilir (IAS 38). MHBS - Cavablı suallar (225-338) Düzgün cavab yaşıl rəngdə və ✓ işarəsi ilə göstərilib; hər sualın altında qısa izah verilib. Qısa cavab açarı: 225-E; 226-E; 227-D; 228-D; 229-A; 230-D; 231-D; 232-E; 233-C; 234-D; 235-E; 236-E; 237-C; 238-E; 239-A; 240-D; 241-D; 242-D; 243-D; 244-D; 245-D; 246-D; 247-D; 248-D; 249-D; 250-C; 251-A; 252-C; 253-C; 254-B; 255-A; 256-A; 257-D; 258-A; 259-C; 260-D; 261-E; 262-D; 263-D; 264-E; 265-E; 266-D; 267-B; 268-D; 269-E; 270-E; 271-C; 272-A; 273-E; 274-C; 275-D; 276-E; 277-B; 278-E; 279-D; 280-D; 281-D; 282-C; 283-A; 284-C; 285-E; 286-D; 287-D; 288-D; 289-E; 290-D; 291-D; 292-D; 293-E; 294-E; 295-C; 296-A; 297-E; 298-D; 299-D; 300-C; 301-A; 302-D; 303-B; 304-D; 305-D; 306-D; 307-C; 308-B; 309-C; 310-D; 311-E; 312-A; 313-E; 314-D; 315-D; 316-D; 317-C; 318-B; 319-D; 320-B; 321-E; 322-D; 323-E; 324-C; 325-E; 326-D; 327-D; 328-E; 329-E; 330-D; 331-C; 332-D; 333-C; 334-D; 335-E; 336-B; 337-E; 338-C"
    ],
    "correct": "Faydalı ömrü qeyri-müəyyən olan QMA amortizasiya olunmur. Hər il və qiymətdəndüşmə əlaməti olduqda qiymətdəndüşmə testi aparılır, həmçinin ömrün qeyri-müəyyən qalıb-qalmadığı hər dövr yenidən nəzərdən keçirilir (IAS 38). MHBS - Cavablı suallar (225-338) Düzgün cavab yaşıl rəngdə və ✓ işarəsi ilə göstərilib; hər sualın altında qısa izah verilib. Qısa cavab açarı: 225-E; 226-E; 227-D; 228-D; 229-A; 230-D; 231-D; 232-E; 233-C; 234-D; 235-E; 236-E; 237-C; 238-E; 239-A; 240-D; 241-D; 242-D; 243-D; 244-D; 245-D; 246-D; 247-D; 248-D; 249-D; 250-C; 251-A; 252-C; 253-C; 254-B; 255-A; 256-A; 257-D; 258-A; 259-C; 260-D; 261-E; 262-D; 263-D; 264-E; 265-E; 266-D; 267-B; 268-D; 269-E; 270-E; 271-C; 272-A; 273-E; 274-C; 275-D; 276-E; 277-B; 278-E; 279-D; 280-D; 281-D; 282-C; 283-A; 284-C; 285-E; 286-D; 287-D; 288-D; 289-E; 290-D; 291-D; 292-D; 293-E; 294-E; 295-C; 296-A; 297-E; 298-D; 299-D; 300-C; 301-A; 302-D; 303-B; 304-D; 305-D; 306-D; 307-C; 308-B; 309-C; 310-D; 311-E; 312-A; 313-E; 314-D; 315-D; 316-D; 317-C; 318-B; 319-D; 320-B; 321-E; 322-D; 323-E; 324-C; 325-E; 326-D; 327-D; 328-E; 329-E; 330-D; 331-C; 332-D; 333-C; 334-D; 335-E; 336-B; 337-E; 338-C"
  },
  {
    "num": 225,
    "question": "Aşağıdakı məsrəflərdən hansı QMA-nın maya dəyərinə daxil edilmir?",
    "options": [
      "İdxal rüsumları və əvəzləşdirilməyən satınalma vergiləri",
      "Aktivin işçi vəziyyətə gətirilməsi ilə bağlı peşəkar xidmət haqları",
      "Aktivin yaradılması zamanı istifadə olunmuş materiallar və işçi mükafatları",
      "Aktivin lazımi səviyyədə işləməsinin yoxlanılmasına çəkilən sınaq işləri",
      "Yeni məhsulun reklamı, heyətin hazırlanması və inzibati ümumi qaimə xərcləri"
    ],
    "correct": "Yeni məhsulun reklamı, heyətin hazırlanması və inzibati ümumi qaimə xərcləri"
  },
  {
    "num": 226,
    "question": "İki təşkilat arasında mal alışı üzrə müqavilə imzalanarsa, lakin tərəflərdən heç biri öhdəliyini hələ yerinə yetirməmişsə (məsələn, mal hələ göndərilməyibsə), tanınma barədə hansı fikir doğrudur?",
    "options": [
      "Yalnız satıcı tərəf debitor borcunu tanımalıdır",
      "Hesabatda yalnız şərti öhdəlik kimi göstərilməlidir",
      "Müqavilə imzalandığı an həm aktiv, həm öhdəlik tanınmalıdır",
      "Yalnız alıcı tərəf aktivi tanımalıdır",
      "Nə aktiv, nə də öhdəlik tanınmayacaqdır"
    ],
    "correct": "Nə aktiv, nə də öhdəlik tanınmayacaqdır"
  },
  {
    "num": 227,
    "question": "Təşkilat maliyyə aktivini yaxud maliyyə öhdəliyini maliyyə vəziyyəti haqqında hesabatında nə zaman tanımalıdır?",
    "options": [
      "Aktivin bazar qiyməti artdıqda",
      "Müqavilə bağlamaq üçün danışıqlara başladıqda",
      "İlkin ödənişin yalnız 100%-i ödənildikdə",
      "Müvafiq alətə uyğun şərtləri müəyyən edən müqavilənin tərəflərindən biri olduqda",
      "Maliyyə ili başa çatdıqda"
    ],
    "correct": "Müvafiq alətə uyğun şərtləri müəyyən edən müqavilənin tərəflərindən biri olduqda"
  },
  {
    "num": 228,
    "question": "Maliyyə öhdəlikləri, istisnalar çıxılmaqla, adətən hansı dəyərlə qiymətləndirilən kimi təsnifləşdirilir?",
    "options": [
      "Maya dəyəri ilə",
      "Ləğv olunma dəyəri ilə",
      "Tarixi dəyərlə",
      "Amortizasiya olunan dəyərlə",
      "Yalnız ədalətli dəyərlə"
    ],
    "correct": "Amortizasiya olunan dəyərlə"
  },
  {
    "num": 229,
    "question": "MHBS (IFRS) 9-a əsasən, maliyyə aktivlərinin təsnifatı hansı iki əsas amildən asılıdır?",
    "options": [
      "Biznes-modeldən və pul axınlarının müqavilə xüsusiyyətlərindən",
      "Aktivin bazar dəyərindən və alış tarixindən",
      "Səhmdarların qərarından və debitorun ölkəsindən",
      "Auditor rəyindən və aktivin istifadə müddətindən",
      "Müəssisənin illik mənfəətindən və vergi dərəcəsindən"
    ],
    "correct": "Biznes-modeldən və pul axınlarının müqavilə xüsusiyyətlərindən"
  },
  {
    "num": 230,
    "question": "\"Opsion\" törəmə maliyyə aləti tərəflərə hansı hüququ verir?",
    "options": [
      "Müəssisənin idarə edilməsində səsvermə hüququnu",
      "Yalnız dividend almaq hüququnu",
      "Mütləq şəkildə malı gələcəkdə təhvil vermək öhdəliyini",
      "Müəyyən olunmuş qiymətlə nəyi isə əldə etmək yaxud satmaq hüququnu",
      "Kredit faizlərini dayandırmaq hüququnu"
    ],
    "correct": "Müəyyən olunmuş qiymətlə nəyi isə əldə etmək yaxud satmaq hüququnu"
  },
  {
    "num": 231,
    "question": "Bir aktivdən gələcək pul axınının, digər aktivdən gələcək pul axınına mübadilə edilməsi barədə saziş necə adlanır?",
    "options": [
      "Forvard",
      "Opsion",
      "İstiqraz",
      "Svop",
      "Fyuçers"
    ],
    "correct": "Svop"
  },
  {
    "num": 232,
    "question": "Aşağıdakılardan hansı törəmə maliyyə alətlərinin (derivativlərin) əsas xüsusiyyətlərindən biridir?",
    "options": [
      "Hesablaşmaların dərhal (saziş bağlanan anda) həyata keçirilməsi",
      "Başlanğıcda çox böyük həcmdə xalis investisiya tələb etməsi",
      "Yalnız nağd pulla əməliyyatları əhatə etməsi",
      "Heç bir risk daşımaması",
      "Dəyərinin faiz dərəcəsi, valyuta məzənnəsi və ya indeks kimi dəyişənlərdən asılı olaraq dəyişməsi"
    ],
    "correct": "Dəyərinin faiz dərəcəsi, valyuta məzənnəsi və ya indeks kimi dəyişənlərdən asılı olaraq dəyişməsi"
  },
  {
    "num": 233,
    "question": "IFRS 13-ə görə \"Ədalətli dəyər\" nədir?",
    "options": [
      "Aktivin alınması üçün çəkilən tarixi xərclərin cəmi",
      "Aktivin ləğv edilməsi zamanı yaranan xərclər",
      "Bazar iştirakçıları arasındakı adi sövdələşmədə aktivin satışından əldə oluna biləcək məbləğ",
      "Yalnız törəmə alətlərin ilkin investisiya məbləği",
      "Aktivin balans dəyəri ilə bazar dəyəri arasındakı fərq"
    ],
    "correct": "Bazar iştirakçıları arasındakı adi sövdələşmədə aktivin satışından əldə oluna biləcək məbləğ"
  },
  {
    "num": 234,
    "question": "Pay aləti nəyi ifadə edir?",
    "options": [
      "Müəssisənin bank qarşısındakı kredit öhdəliyini",
      "Mal satanlara olan borcların cəmini",
      "Müəssisənin illik xalis mənfəətini",
      "Təşkilatın bütün öhdəliklərini çıxdıqdan sonra onun aktivlərindəki qalıq payını təsdiq edən müqaviləni",
      "Yalnız törəmə maliyyə alətlərinin dəyərini"
    ],
    "correct": "Təşkilatın bütün öhdəliklərini çıxdıqdan sonra onun aktivlərindəki qalıq payını təsdiq edən müqaviləni"
  },
  {
    "num": 235,
    "question": "MHBS (IFRS) 7 standartı hansı məsələni tənzimləyir?",
    "options": [
      "Ehtiyatların maya dəyərinin hesablanmasını",
      "İşçilərin əmək haqqı uçotunu",
      "Əsas vəsaitlərin amortizasiya normalarını",
      "İnvestisiya mülkiyyətinin qiymətləndirilməsini",
      "Maliyyə alətləri ilə bağlı informasiyanın maliyyə hesabatlarında açıqlanmasını"
    ],
    "correct": "Maliyyə alətləri ilə bağlı informasiyanın maliyyə hesabatlarında açıqlanmasını"
  },
  {
    "num": 236,
    "question": "Daxili layihə çərçivəsində aparılan \"Tədqiqat\" (Research) mərhələsinin xərcləri uçotda necə əks olunmalıdır?",
    "options": [
      "Yalnız layihə uğurlu olduqda aktiv kimi tanınır",
      "Aktivin maya dəyərinə daxil edilərək kapitallaşdırılır",
      "Amortizasiya olunaraq 10 il ərzində silinir",
      "Kapitalın tərkibində ehtiyat kimi yığılır",
      "Qeyri-maddi aktiv kimi tanınmır və baş verdiyi dövrün xərclərinə aid edilir"
    ],
    "correct": "Qeyri-maddi aktiv kimi tanınmır və baş verdiyi dövrün xərclərinə aid edilir"
  },
  {
    "num": 237,
    "question": "MHBS (IAS) 38-ə əsasən, qeyri-maddi aktivin (QMA) tərifi hansı variantda düzgün verilmişdir?",
    "options": [
      "Müəssisənin nağd pul vəsaitləri və bank qalıqlarıdır",
      "Yalnız şirkətin daxilində yaradılmış işgüzar imicdir (qüdvil)",
      "Fiziki əsasa malik olmayan, identifikasiya oluna bilən qeyri-monetar aktivdir",
      "Fiziki formaya malik olan və istehsalda istifadə edilən aktivdir",
      "Müəssisənin sahib olduğu bütün maliyyə investisiyalarıdır"
    ],
    "correct": "Fiziki əsasa malik olmayan, identifikasiya oluna bilən qeyri-monetar aktivdir"
  },
  {
    "num": 238,
    "question": "Faydalı qazıntıların hasilatının texniki mümkünlüyü və kommersiya məqsədəuyğunluğu nümayiş etdirildikdən sonra kəşfiyyat aktivləri ilə bağlı hansı prosedur həyata keçirilməlidir?",
    "options": [
      "Aktivlər dərhal mənfəət və zərər hesabatında xərc kimi silinməlidir",
      "Aktivlərin dəyəri dərhal 50% azaldılmalıdır",
      "Aktivlər birbaşa kapital ehtiyatlarına köçürülməlidir",
      "Aktivlərin uçotu IFRS 6 standartı ilə davam etdirilməlidir",
      "Aktivlərin qiymətdəndüşməsi yoxlanılmalı, zərər varsa tanınmalı və aktivlər yenidən təsnifləşdirilməlidir"
    ],
    "correct": "Aktivlərin qiymətdəndüşməsi yoxlanılmalı, zərər varsa tanınmalı və aktivlər yenidən təsnifləşdirilməlidir"
  },
  {
    "num": 239,
    "question": "Aşağıdakı məsrəflərdən hansı kəşfiyyat və qiymətləndirmə aktivlərinin ilkin dəyərinə daxil edilə bilər?",
    "options": [
      "Topoqrafik, geoloji, geokimyavi tədqiqatların aparılması və axtarış quyularının qazılması məsrəfləri",
      "Çıxarılan faydalı qazıntıların emalı və təmizlənməsi xərcləri",
      "Şirkət rəhbərliyinin ümumi idarəetmə və ofis xərcləri",
      "Hasilat başladıqdan sonra məhsulun bazara çıxarılması üçün çəkilən reklam xərcləri",
      "Kəşfiyyat işlərinin aparılmasına ixtiyari hüquqların alınmasına qədər çəkilmiş xərclər"
    ],
    "correct": "Topoqrafik, geoloji, geokimyavi tədqiqatların aparılması və axtarış quyularının qazılması məsrəfləri"
  },
  {
    "num": 240,
    "question": "MHBS (IFRS) 6 standartı faydalı qazıntıların kəşfiyyatı ilə bağlı hansı dövrdə çəkilən məsrəflərə şamil olunur?",
    "options": [
      "Mineral resursların emalı və satışına çəkilən məsrəflərə",
      "Yalnız kəşfiyyat hüquqları alınana qədər aparılan ilkin axtarış işlərinə",
      "Faydalı qazıntıların çıxarılmasının texniki cəhətdən mümkünlüyü tam sübut olunduqdan sonra çəkilən bütün xərclərə",
      "Müəyyən ərazidə kəşfiyyat hüququ əldə edildikdən sonra, lakin hasilatın texniki mümkünlüyü və kommersiya faydalılığı sübut edilənə qədər olan dövrdə",
      "Müəssisənin kəşfiyyat fəaliyyəti ilə bağlı olmayan bütün inzibati xərclərinə"
    ],
    "correct": "Müəyyən ərazidə kəşfiyyat hüququ əldə edildikdən sonra, lakin hasilatın texniki mümkünlüyü və kommersiya faydalılığı sübut edilənə qədər olan dövrdə"
  },
  {
    "num": 241,
    "question": "Satış məsrəfləri çıxılmaqla ədalətli dəyərlə qiymətləndirilən bioloji aktivlərə aid edilən \"şərtsiz\" dövlət subsidiyaları nə zaman tanınmalıdır?",
    "options": [
      "Kapitalın tərkibində ehtiyat kimi",
      "Aktivin faydalı ömür müddəti ərzində bərabər hissələrlə",
      "Yalnız müəssisə fəaliyyətini dayandırdığı zaman",
      "Həmin dövlət subsidiyalarının alınması gerçəkləşdikdə (alınma hüququ yarandıqda) mənfəət və ya zərərdə",
      "Subsidiyadan istifadə edərək yeni heyvanlar alındığı zaman"
    ],
    "correct": "Həmin dövlət subsidiyalarının alınması gerçəkləşdikdə (alınma hüququ yarandıqda) mənfəət və ya zərərdə"
  },
  {
    "num": 242,
    "question": "Bioloji aktivdən yığılmış kənd təsərrüfatı məhsulu (məsələn, yun, süd, kəsilmiş qamış) yığım anından sonra hansı standartla uçota alınır?",
    "options": [
      "MHBS (IAS) 16 \"Torpaq, tikili və avadanlıqlar\"",
      "Standart tətbiq edilmir, birbaşa xərcə silinir",
      "MHBS (IAS) 38 \"Qeyri-maddi aktivlər\"",
      "MHBS (IAS) 2 \"Ehtiyatlar\"",
      "MHBS (IFRS) 9 \"Maliyyə alətləri\""
    ],
    "correct": "MHBS (IAS) 2 \"Ehtiyatlar\""
  },
  {
    "num": 243,
    "question": "Aşağıdakılardan hansı maliyyə aktivlərinə aid deyil?",
    "options": [
      "Müəssisənin əldə etdiyi istiqrazlar",
      "Nağd pul vəsaitləri",
      "Digər təşkilatın pay alətləri (səhmləri)",
      "Müəssisənin ödəməli olduğu kreditor borcları",
      "Debitor borcları və verilmiş borclar"
    ],
    "correct": "Müəssisənin ödəməli olduğu kreditor borcları"
  },
  {
    "num": 244,
    "question": "Maliyyə alətinin tərifi aşağıdakılardan hansıdır?",
    "options": [
      "Yalnız bank kreditlərini əks etdirən müqavilədir",
      "Yalnız nağd pul vəsaitlərinin hərəkətini tənzimləyən sənəddir",
      "Müəssisənin bütün aktivlərinin cəmidir",
      "Bir təşkilatda maliyyə aktivi, digər təşkilatda isə maliyyə öhdəliyi yaxud pay aləti yaradan müqavilədir",
      "Vergi hesabatlılığı üçün istifadə olunan formadır"
    ],
    "correct": "Bir təşkilatda maliyyə aktivi, digər təşkilatda isə maliyyə öhdəliyi yaxud pay aləti yaradan müqavilədir"
  },
  {
    "num": 245,
    "question": "MHBS (IAS) 32 standartının əsas məqsədi nədən ibarətdir?",
    "options": [
      "Debitor borclarının silinməsi qaydalarını müəyyən etmək",
      "Maliyyə alətlərinin ədalətli dəyərini qiymətləndirmək",
      "Yalnız törəmə maliyyə alətlərinin uçotunu aparmaq",
      "Maliyyə alətlərinin öhdəlik yaxud xüsusi kapital tərkibində təqdim edilməsi prinsiplərini müəyyən etmək",
      "Pul vəsaitlərinin hərəkəti haqqında hesabatı hazırlamaq"
    ],
    "correct": "Maliyyə alətlərinin öhdəlik yaxud xüsusi kapital tərkibində təqdim edilməsi prinsiplərini müəyyən etmək"
  },
  {
    "num": 246,
    "question": "Hansı halda satış üçün nəzərdə tutulan aktivlərin və öhdəliklərin əsas sinifləri üzrə informasiyanın təqdim edilməsi və açıqlanması tələb olunmur?",
    "options": [
      "Əgər aktivlər xarici valyuta ilə əldə edilibsə",
      "Aktivin dəyəri müəssisənin cəmi aktivlərinin 10%-dən az olduqda",
      "Əgər satış bir ildən daha uzun müddət çəkərsə",
      "Yenidən satış üçün nəzərdə tutulan törəmə müəssisələr üçün",
      "Yalnız xidmət sferasında fəaliyyət göstərən müəssisələr üçün"
    ],
    "correct": "Yenidən satış üçün nəzərdə tutulan törəmə müəssisələr üçün"
  },
  {
    "num": 247,
    "question": "Maliyyə vəziyyəti haqqında hesabatda satış üçün nəzərdə tutulan aktivlər üzrə müqayisəli informasiya ilə bağlı tələb hansıdır?",
    "options": [
      "Müqayisəli dövr üçün yalnız aktivlər göstərilməli, öhdəliklər silinməlidir",
      "Keçmiş illərin bütün rəqəmləri cari ilin təsnifatına uyğun olaraq yenidən hesablanmalıdır",
      "Müqayisəli informasiya yalnız aktivlərin ədalətli dəyəri artdıqda yenidən hazırlanır",
      "Müqayisəli informasiyanın yenidən hesablanması tələb olunmur",
      "Müqayisəli məlumatlar mütləq müstəqil auditor tərəfindən yenidən təsdiqlənməlidir"
    ],
    "correct": "Müqayisəli informasiyanın yenidən hesablanması tələb olunmur"
  },
  {
    "num": 248,
    "question": "Aşağıdakılardan hansı dayandırılmış fəaliyyətin nəticəsi kimi məcmu gəlir haqqında hesabatda əks etdirilən məbləğlərə aid deyil?",
    "options": [
      "Vergi ödənişindən sonra dayandırılmış fəaliyyətə aid olan xalis məbləğlər",
      "Vergitutmadan sonra dayandırılmış fəaliyyətdən yaranan mənfəət və ya zərər",
      "Dayandırılmış fəaliyyət tərkibinə daxil olan aktivlərin təsərrüfatdan çıxmasından yaranan mənfəət və ya zərər",
      "Müəssisənin bütün fəaliyyəti üzrə hesablanmış ümumi amortizasiya xərcləri",
      "Vergitutmadan sonra satış xərcləri çıxılmaqla ədalətli dəyərlə yenidənqiymətləndirilmədən olan nəticə"
    ],
    "correct": "Müəssisənin bütün fəaliyyəti üzrə hesablanmış ümumi amortizasiya xərcləri"
  },
  {
    "num": 249,
    "question": "Mənfəət və ya zərər və sair məcmu gəlir haqqında hesabatda fəaliyyətlər hansı qaydada qruplaşdırılmalıdır?",
    "options": [
      "Hesabatda yalnız vergitutmadan əvvəlki mənfəət göstərilməli, dayandırılmış fəaliyyət isə nəzərə alınmamalıdır",
      "Bütün gəlir və xərclər fəaliyyət növündən asılı olmayaraq vahid bölmədə birləşdirilməlidir",
      "Yalnız davam etdirilən fəaliyyət əks olunmalı, dayandırılmış fəaliyyət isə yalnız Qeydlərdə verilməlidir",
      "Davam etdirilən fəaliyyət və dayandırılmış fəaliyyət üzrə informasiya ayrıca əks etdirilməlidir",
      "Dayandırılmış fəaliyyət üzrə məlumatlar yalnız növbəti ilin hesabatında açıqlanmalıdır"
    ],
    "correct": "Davam etdirilən fəaliyyət və dayandırılmış fəaliyyət üzrə informasiya ayrıca əks etdirilməlidir"
  },
  {
    "num": 250,
    "question": "Əgər təşkilat satış planından imtina edərsə və aktivi yenidən \"uzunmüddətli aktiv\" kimi təsnifləşdirərsə, qiymətləndirmə necə aparılır?",
    "options": [
      "Aktivin yenidən qiymətləndirilməsi üzrə müstəqil ekspertin təyin etdiyi məbləğlə",
      "Yalnız mülkiyyətçilərin razılaşdığı nominal dəyərlə",
      "Amortizasiya çıxılmaqla balans dəyəri ilə ödənilmə dəyərindən kiçik olanla",
      "Aktivin ilkin alış qiyməti (tarixi dəyəri) ilə",
      "Həmin tarixdəki ən yüksək bazar qiyməti ilə"
    ],
    "correct": "Amortizasiya çıxılmaqla balans dəyəri ilə ödənilmə dəyərindən kiçik olanla"
  },
  {
    "num": 251,
    "question": "Aşağıdakı bioloji aktivlərdən hansı MHBS (IAS) 16 \"Torpaq, tikili və avadanlıqlar\" standartının tətbiq sferasına aiddir?",
    "options": [
      "Üzümlüklər, meyvə ağacları və çay kolları kimi məhsulverən bitkilər",
      "Yığım anındakı çay yarpağı və ya üzüm",
      "Satış üçün nəzərdə tutulmuş donuzlar",
      "Ətlik məqsədilə saxlanılan mal-qara",
      "Meşə təsərrüfatında kəsilmək üçün yetişdirilən ağaclar"
    ],
    "correct": "Üzümlüklər, meyvə ağacları və çay kolları kimi məhsulverən bitkilər"
  },
  {
    "num": 252,
    "question": "\"Bioloji transformasiya\" anlayışı MHBS (IAS) 41-də necə tərif edilir?",
    "options": [
      "Aktivin amortizasiya olunaraq dəyərini itirməsi prosesidir",
      "Bioloji aktivin bazarda satış qiymətinin dəyişməsidir",
      "Bioloji aktivdə keyfiyyət və ya kəmiyyət dəyişikliklərinə səbəb olan artım, degenerasiya, məhsul istehsalı və təkrar istehsal prosesləridir",
      "Kənd təsərrüfatı məhsulunun zavodda emal edilərək ərzağa çevrilməsidir",
      "Heyvanların yalnız bir məkandan digər məkana daşınması prosesidir"
    ],
    "correct": "Bioloji aktivdə keyfiyyət və ya kəmiyyət dəyişikliklərinə səbəb olan artım, degenerasiya, məhsul istehsalı və təkrar istehsal prosesləridir"
  },
  {
    "num": 253,
    "question": "MHBS (IAS) 41 standartına əsasən, bioloji aktivlər ilkin tanınma zamanı və hər hesabat dövrünün sonunda hansı dəyərlə qiymətləndirilməlidir?",
    "options": [
      "Ləğv dəyəri əlavə olunmaqla balans dəyəri ilə",
      "Yalnız tarixi maya dəyəri ilə",
      "Ehtimal olunan satış məsrəfləri çıxılmaqla ədalətli dəyərlə",
      "Aktivin 5 illik gözlənilən məhsuldarlıq dəyəri ilə",
      "Müəssisənin müəyyən etdiyi daxili istifadə qiyməti ilə"
    ],
    "correct": "Ehtimal olunan satış məsrəfləri çıxılmaqla ədalətli dəyərlə"
  },
  {
    "num": 254,
    "question": "İnvestisiyalı daşınmaz əmlakın tanınmasının dayandırılması (balansdan silinməsi) hansı halda baş verir?",
    "options": [
      "Aktivin faydalı istifadə müddətinin yarısı başa çatdıqda",
      "Obyekt təsərrüfatdan çıxdıqda və ya ondan gələcəkdə hər hansı iqtisadi faydanın alınması ehtimalı olmadıqda",
      "Aktivin bazar qiyməti onun maya dəyərindən 10% aşağı düşdükdə",
      "Aktivin təmirə ehtiyacı olduğu üçün istifadəsi müvəqqəti dayandıqda",
      "Müəssisə icarədar dəyişmək qərarına gəldikdə"
    ],
    "correct": "Obyekt təsərrüfatdan çıxdıqda və ya ondan gələcəkdə hər hansı iqtisadi faydanın alınması ehtimalı olmadıqda"
  },
  {
    "num": 255,
    "question": "Sahibolan tərəfindən tutulan daşınmaz əmlak (IAS 16) İDƏ kateqoriyasına (IAS 40 - ədalətli dəyər modeli ilə) keçirilərkən yaranan müsbət fərq necə uçota alınır?",
    "options": [
      "MHBS (IAS) 16-ya uyğun olaraq aparılmış yenidənqiymətləndirilmə ehtiyatı (kapital) kimi",
      "Dərhal digər əməliyyat gəliri kimi mənfəət və zərər hesabatında",
      "Gələcək dövrlərin gəliri kimi",
      "Ehtiyatların (malların) dəyərinin artması kimi",
      "Aktivin amortizasiya xərclərinin azaldılması kimi"
    ],
    "correct": "MHBS (IAS) 16-ya uyğun olaraq aparılmış yenidənqiymətləndirilmə ehtiyatı (kapital) kimi"
  },
  {
    "num": 256,
    "question": "İDƏ-nin uçotu üçün \"Ədalətli dəyər modeli\" seçildikdə, dəyər dəyişikliyindən yaranan gəlir və ya zərər harada tanınmalıdır?",
    "options": [
      "Baş verdiyi dövrün mənfəət və ya zərərində",
      "Kapitalın tərkibindəki yenidənqiymətləndirilmə ehtiyatında",
      "Sair məcmu gəlirdə (OCI)",
      "Balans hesabatında aktivin maya dəyərinə əlavə edilməklə",
      "Yalnız aktiv satıldığı zaman bölüşdürülməmiş mənfəətdə"
    ],
    "correct": "Baş verdiyi dövrün mənfəət və ya zərərində"
  },
  {
    "num": 257,
    "question": "İnvestisiyalı daşınmaz əmlakın (İDƏ) ilkin qiymətləndirilməsi hansı dəyərlə aparılmalıdır?",
    "options": [
      "Yalnız bazar iştirakçıları tərəfindən müəyyən edilən ədalətli dəyərlə",
      "Aktivin sığorta dəyəri ilə",
      "Aktivin 10 illik gözlənilən icarə gəlirlərinin cəmi ilə",
      "Maya dəyəri (əldə olunma qiyməti və digər birbaşa məsrəflər daxil edilməklə)",
      "Müəssisə rəhbərliyinin müəyyən etdiyi subyektiv dəyərlə"
    ],
    "correct": "Maya dəyəri (əldə olunma qiyməti və digər birbaşa məsrəflər daxil edilməklə)"
  },
  {
    "num": 258,
    "question": "MHBS (IAS) 40 standartına əsasən, aşağıdakılardan hansı \"İnvestisiyalı daşınmaz əmlak\" (İDƏ) hesab olunur?",
    "options": [
      "İcarə gəliri və ya kapitalın dəyərinin artması məqsədilə saxlanılan torpaq və ya bina",
      "Üçüncü tərəflərə xidmət göstərilməsi üçün istifadə edilən texniki avadanlıqlar",
      "Malların istehsalı və ya inzibati məqsədlər üçün istifadə olunan bina",
      "Adi fəaliyyət dövründə qısamüddətli satış üçün nəzərdə tutulmuş daşınmaz əmlak",
      "İşçilərin yaşayışı üçün nəzərdə tutulmuş müəssisə yataqxanası"
    ],
    "correct": "İcarə gəliri və ya kapitalın dəyərinin artması məqsədilə saxlanılan torpaq və ya bina"
  },
  {
    "num": 259,
    "question": "Aşağıdakı hallardan hansında aktiv \"dayandırılmış fəaliyyət\" hesab oluna bilər?",
    "options": [
      "Yeni bir fəaliyyət növünə başlamaq üçün avadanlıqların alınması",
      "İnzibati binanın bir mərtəbəsinin icarəyə verilməsi",
      "Müəssisənin əhəmiyyətli fəaliyyət növü və ya coğrafi rayonunun satış üçün nəzərdə tutulması",
      "Direktorlar şurasının tərkibində dəyişiklik edilməsi",
      "Müəssisədə yalnız bir istehsal xəttinin müvəqqəti (təmir üçün) dayandırılması"
    ],
    "correct": "Müəssisənin əhəmiyyətli fəaliyyət növü və ya coğrafi rayonunun satış üçün nəzərdə tutulması"
  },
  {
    "num": 260,
    "question": "\"Pul vəsaitləri yaradan vahid\" nədir?",
    "options": [
      "Müəssisənin yalnız kassa və bank hesablarından ibarət olan bölməsi",
      "Müəssisənin mənfəət vergisini hesablayan maliyyə departamenti",
      "Aktivin istifadə müddəti bitdikdən sonra satıla biləcəyi qalıq dəyəri",
      "Digər aktivlərdən asılı olmayaraq pul daxilolmaları yaradan ən az identifikasiya olunan aktivlər qrupu",
      "Yalnız satış şöbəsinin tabeliyində olan bütün maşın və avadanlıqlar"
    ],
    "correct": "Digər aktivlərdən asılı olmayaraq pul daxilolmaları yaradan ən az identifikasiya olunan aktivlər qrupu"
  },
  {
    "num": 261,
    "question": "Satış üçün nəzərdə tutulan aktivin ədalətli dəyəri sonradan artarsa, bu artım necə tanınır?",
    "options": [
      "Artım yalnız ehtiyat kapitalında əks etdirilir",
      "Bu artım aktivin amortizasiya normasının azaldılmasına yönəldilir",
      "Tam məbləğdə mənfəət kimi tanınır və məhdudiyyət qoyulmur",
      "Bu artım tanınmır və aktiv satış anına qədər köhnə qiymətlə qalır",
      "Yalnız əvvəlki dövrlərdə tanınmış qiymətdəndüşmədən olan zərər məbləği həddində"
    ],
    "correct": "Yalnız əvvəlki dövrlərdə tanınmış qiymətdəndüşmədən olan zərər məbləği həddində"
  },
  {
    "num": 262,
    "question": "\"Satışa xərclər\" anlayışına aşağıdakılardan hansı DAXİL EDİLMİR?",
    "options": [
      "Aktivin satışı ilə bilavasitə bağlı olan hüquqi xərclər",
      "Aktivin təsərrüfatdan çıxması ilə əlaqədar olan komissiya xərcləri",
      "Sövdələşməni həyata keçirmək üçün ödənilən vasitəçilik haqqı",
      "Maliyyələşdirməyə çəkilən məsrəflər və mənfəət vergisi üzrə xərclər",
      "Malların çıxarılması və ya daşınması üçün çəkilən əlavə məsrəflər"
    ],
    "correct": "Maliyyələşdirməyə çəkilən məsrəflər və mənfəət vergisi üzrə xərclər"
  },
  {
    "num": 263,
    "question": "\"Ödənilmə dəyəri\" nəyi ifadə edir?",
    "options": [
      "Aktivin yenidən alınması üçün tələb olunan cari bazar məbləğini",
      "Yalnız aktivin istifadə müddəti ərzində gətirəcəyi pul vəsaitlərini",
      "Aktivin bazar qiyməti ilə balans dəyərinin cəmini",
      "Satış xərcləri çıxılmaqla ədalətli dəyər və istifadənin qiymətliliyindən ən yüksək olanı",
      "Aktivin sığorta dəyəri ilə maya dəyəri arasındakı fərqi"
    ],
    "correct": "Satış xərcləri çıxılmaqla ədalətli dəyər və istifadənin qiymətliliyindən ən yüksək olanı"
  },
  {
    "num": 264,
    "question": "MHBS (IFRS) 5-ə əsasən, satış üçün nəzərdə tutulan uzunmüddətli aktivlər hesabatda necə qiymətləndirilməlidir?",
    "options": [
      "Balans dəyəri və ödənilmə dəyərindən böyük olanla",
      "Yalnız alış qiyməti və ya istehsal maya dəyəri ilə",
      "Hər iki ildən bir bazar tərəfindən müəyyən edilən ədalətli dəyərlə",
      "Yalnız diskontlaşdırılmış satış dəyəri ilə",
      "Balans dəyəri və satış xərcləri çıxılmaqla ədalətli dəyərdən kiçik olanla"
    ],
    "correct": "Balans dəyəri və satış xərcləri çıxılmaqla ədalətli dəyərdən kiçik olanla"
  },
  {
    "num": 265,
    "question": "Təşkilat hansı halda ehtiyatların qiymətləndirilməsi üçün müxtəlif metodlardan istifadə edə bilər?",
    "options": [
      "Müəssisə mənfəət vergisi ödənişini azaltmaq istədikdə",
      "Ehtiyatların alış qiyməti son bir il ərzində sabit qaldıqda",
      "Ehtiyatların həcmi anbar tutumundan çox olduqda",
      "Ehtiyatlar yalnız müxtəlif ölkələrdən idxal edildikdə",
      "Ehtiyatlar öz xarakterinə və istifadəsinə görə müxtəlif olduqda"
    ],
    "correct": "Ehtiyatlar öz xarakterinə və istifadəsinə görə müxtəlif olduqda"
  },
  {
    "num": 266,
    "question": "Orta maya dəyəri (AVCO) metodunda orta kəmiyyət hansı intervallarla hesablanıla bilər?",
    "options": [
      "Yalnız ehtiyatlar tamamilə tükəndiyi zaman",
      "Yalnız müəssisə rəhbərliyi tərəfindən xüsusi qərar verildiyi tarixlərdə",
      "Yalnız hər ilin sonunda bir dəfə",
      "Ya dövrü əsasda (sadə orta çəki), ya da hər əlavə dəst ehtiyat alındıqdan sonra (sürüşkən orta çəki)",
      "Malların anbara daxil olduğu tarixdən asılı olmayaraq hər günün sonunda"
    ],
    "correct": "Ya dövrü əsasda (sadə orta çəki), ya da hər əlavə dəst ehtiyat alındıqdan sonra (sürüşkən orta çəki)"
  },
  {
    "num": 267,
    "question": "TTA obyektinin balansda tanınması (tanınmanın dayandırılması) hansı halda baş verir?",
    "options": [
      "Aktivin faydalı istifadə müddətinin yarısı başa çatdıqda",
      "Obyekt təsərrüfatdan çıxdıqda və ya onun istifadəsindən gələcəkdə hər hansı iqtisadi fayda gözlənilmədikdə",
      "Müəssisə rəhbərliyi dəyişdikdə",
      "Aktiv müvəqqəti olaraq təmirə dayandıqda",
      "Aktivin ədalətli dəyəri onun maya dəyərindən aşağı düşdükdə"
    ],
    "correct": "Obyekt təsərrüfatdan çıxdıqda və ya onun istifadəsindən gələcəkdə hər hansı iqtisadi fayda gözlənilmədikdə"
  },
  {
    "num": 268,
    "question": "Aktivin amortizasiyası ilə bağlı aşağıdakı mülahizələrdən hansı doğrudur?",
    "options": [
      "Torpaq sahələri hər zaman binalarla birlikdə eyni norma ilə amortizasiya olunur",
      "Aktivin ləğv dəyəri balans dəyərindən çox olduqda amortizasiya artırılmalıdır",
      "Amortizasiya metodu yalnız 5 ildən bir dəyişdirilə bilər",
      "Amortizasiya aktiv istifadə üçün əlçatan olduğu andan (yerləşdiyi yer və vəziyyəti uyğun olduqda) başlanılır",
      "Aktivin təmiri və ona xidmət göstərilməsi amortizasiya hesablanması zəruriliyini aradan qaldırır"
    ],
    "correct": "Amortizasiya aktiv istifadə üçün əlçatan olduğu andan (yerləşdiyi yer və vəziyyəti uyğun olduqda) başlanılır"
  },
  {
    "num": 269,
    "question": "Yenidənqiymətləndirilmə modeli tətbiq edilərkən, aktivin dəyərinin İLK DƏFƏ artması (artım fərqi) maliyyə hesabatlarında necə əks olunur?",
    "options": [
      "Bölüşdürülməmiş mənfəətin artması kimi",
      "Öhdəliklərin azalması kimi",
      "Aktivin amortizasiya xərclərinin azaldılması kimi",
      "Birbaşa hesabat dövrünün xalis mənfəəti kimi",
      "Kapitalda (Sair məcmu gəlir bölməsində) yenidənqiymətləndirilmə ehtiyatı kimi"
    ],
    "correct": "Kapitalda (Sair məcmu gəlir bölməsində) yenidənqiymətləndirilmə ehtiyatı kimi"
  },
  {
    "num": 270,
    "question": "\"İstifadənin qiymətliliyi\" (Value in use) anlayışı aşağıdakılardan hansını ifadə edir?",
    "options": [
      "Aktivin sığorta şirkəti tərəfindən müəyyən edilmiş bərpa qiymətini",
      "Aktivin yalnız sonuncu ilində yaradacağı mənfəəti",
      "Aktivin hazırkı bazar qiymətindən satış xərcləri çıxıldıqdan sonra qalan məbləği",
      "Aktivin ilkin satın alınma qiymətini",
      "Aktivdən gələcəkdə əldə olunması gözlənilən xalis pul vəsaitlərinin diskontlaşdırılmış dəyərini"
    ],
    "correct": "Aktivdən gələcəkdə əldə olunması gözlənilən xalis pul vəsaitlərinin diskontlaşdırılmış dəyərini"
  },
  {
    "num": 271,
    "question": "MHBS (IAS) 16-ya əsasən, TTA obyektlərinin ilkin tanınmasından sonra uçotun aparılması üçün hansı modellər təklif edilir?",
    "options": [
      "Yalnız bazar dəyəri ilə uçot modeli",
      "Likvidlik modeli və Gəlirlilik modeli",
      "Maya dəyəri ilə uçot modeli və ya Yenidənqiymətləndirilmə dəyəri ilə uçot modeli",
      "Faiz dərəcəsi modeli və İnflyasiya modeli",
      "Tarixi dəyər və Nominal dəyər modelləri"
    ],
    "correct": "Maya dəyəri ilə uçot modeli və ya Yenidənqiymətləndirilmə dəyəri ilə uçot modeli"
  },
  {
    "num": 272,
    "question": "Təşkilatın iri ehtiyat hissələri və servis avadanlığı hansı halda TTA kimi tanına bilər?",
    "options": [
      "Əgər təşkilat onları bir hesabat dövründən artıq müddətdə istifadə etməyi nəzərdə tutursa",
      "Əgər onların qiyməti 1000 -dan çoxdursa",
      "Yalnız müəssisə rəhbərliyi icazə verdikdə",
      "Hər bir halda iri ehtiyat hissələri həmişə ehtiyat kimi uçota alınmalıdır",
      "Yalnız aktiv ləğv edildiyi zaman"
    ],
    "correct": "Əgər təşkilat onları bir hesabat dövründən artıq müddətdə istifadə etməyi nəzərdə tutursa"
  },
  {
    "num": 273,
    "question": "IAS 20-yə əsasən, dövlət subsidiyası hesabına alınan aktivin balans dəyəri necə əks etdirilə bilər?",
    "options": [
      "Subsidiya yalnız xüsusi kapitalda ehtiyat kimi saxlanılmalıdır",
      "Subsidiya mütləq şəkildə dərhal xalis mənfəətə aid edilməlidir",
      "Dövlət subsidiyaları maliyyə hesabatlarında ümumiyyətlə əks olunmur",
      "Subsidiyalar TTA-nın ilkin dəyərini artırmaq üçün istifadə olunmalıdır",
      "Ya alınmış subsidiya məbləğində aktivin balans dəyəri azaldılır, ya da subsidiya gələcək dövrlərin gəliri kimi tanınır"
    ],
    "correct": "Ya alınmış subsidiya məbləğində aktivin balans dəyəri azaldılır, ya da subsidiya gələcək dövrlərin gəliri kimi tanınır"
  },
  {
    "num": 274,
    "question": "TTA obyektlərinin mübadiləsi zamanı, əgər həm verilən, həm də alınan aktivin ədalətli dəyəri etibarlı ölçülə bilirsə, alınan aktiv hansı qiymətlə uçota alınır?",
    "options": [
      "Alınan aktivin balans dəyəri ilə",
      "Aktivin maya dəyəri ilə",
      "Təqdim edilən (verilən) aktivin ədalətli dəyəri (\"çıxış\" qiyməti) ilə",
      "Yalnız qarşı tərəfin müəyyən etdiyi satış qiyməti ilə",
      "Hər iki aktivin balans dəyərlərinin orta qiyməti ilə"
    ],
    "correct": "Təqdim edilən (verilən) aktivin ədalətli dəyəri (\"çıxış\" qiyməti) ilə"
  },
  {
    "num": 275,
    "question": "FIFO (First-In, First-Out) metodunun əsas məntiqi nədir?",
    "options": [
      "Sonuncu əldə olunmuş ehtiyatların birinci istifadə olunduğu fərz edilir",
      "Ehtiyatlar müntəzəm olaraq ən köhnə alış qiymətinə bərabər tutulur",
      "Ehtiyatlar yalnız bazar qiyməti ilə qiymətləndirilir",
      "Birinci əldə olunmuş ehtiyatların birinci satıldığı və dövrün sonuna qalanların sonradan alınanlar olduğu fərz edilir",
      "Bütün ehtiyatların maya dəyəri dövr ərzindəki orta çəki qiyməti ilə hesablanır"
    ],
    "correct": "Birinci əldə olunmuş ehtiyatların birinci satıldığı və dövrün sonuna qalanların sonradan alınanlar olduğu fərz edilir"
  },
  {
    "num": 276,
    "question": "Xidmət sferasında fəaliyyət göstərən müəssisələr üçün ehtiyatların maya dəyəri nələrdən ibarətdir?",
    "options": [
      "Yalnız ofis binalarının icarə xərclərindən",
      "Müəssisə rəhbərliyinin xaricə ezamiyyət xərclərindən",
      "Yalnız müəssisənin marketinq və reklam xərclərindən",
      "Müştərilərin xidmətdən yararlanmaq üçün ödədiyi ümumi satış məbləğindən",
      "Sərf olunan materiallar, işçi qüvvəsi məsrəfləri və müvafiq qaimə xərclərindən"
    ],
    "correct": "Sərf olunan materiallar, işçi qüvvəsi məsrəfləri və müvafiq qaimə xərclərindən"
  },
  {
    "num": 277,
    "question": "Saxlanılma xərcləri hansı halda ehtiyatın maya dəyərinə daxil edilə bilməz?",
    "options": [
      "Əgər saxlama müddəti bir ildən qısadırsa",
      "Əgər bu xərclər ehtiyatın növbəti mərhələyə keçməsi üçün istehsal prosesində zəruri deyildirsə",
      "Əgər mallar pərakəndə satış nöqtələrində vitrinlərdə sərgilənirsə",
      "Əgər saxlanılan mallar yalnız xarici bazara ixrac üçün nəzərdə tutulubsa",
      "Əgər mallar soyuducu anbarlarda saxlanılırsa"
    ],
    "correct": "Əgər bu xərclər ehtiyatın növbəti mərhələyə keçməsi üçün istehsal prosesində zəruri deyildirsə"
  },
  {
    "num": 278,
    "question": "Aşağıdakı məsrəflərdən hansı ehtiyatların istehsal maya dəyərinə daxil EDİLMİR?",
    "options": [
      "Ehtiyatın istifadə üçün cari vəziyyətə gətirilməsi ilə bağlı digər birbaşa məsrəflər",
      "Müəyyən hallarda (IAS 23-ə uyğun) borclar üzrə məsrəflər",
      "Birbaşa əmək məsrəfləri (işçilərin əmək haqqı)",
      "Xammalın hazır məhsula çevrilməsi zamanı baş verən dəyişən istehsal qaimə xərcləri",
      "Xammalın, əməyin və digər istehsal məsrəflərinin normativdən artıq olan itkiləri"
    ],
    "correct": "Xammalın, əməyin və digər istehsal məsrəflərinin normativdən artıq olan itkiləri"
  },
  {
    "num": 279,
    "question": "Ehtiyatların əldə olunma məsrəfləri müəyyən edilərkən aşağıdakılardan hansı həmin məsrəflərdən çıxılmalıdır?",
    "options": [
      "Gömrük rüsumları və əvəzləşdirilməyən vergilər",
      "Ehtiyatın əldə olunması ilə bilavasitə əlaqədar olan komissiya xərcləri",
      "Xammalın hazır məhsula çevrilməsi üçün çəkilən emal xərcləri",
      "Ticarət güzəştləri, tədiyyələrin qaytarılması və sair oxşar maddələr",
      "Malların anbara gətirilməsi üçün çəkilən daşınma xərcləri"
    ],
    "correct": "Ticarət güzəştləri, tədiyyələrin qaytarılması və sair oxşar maddələr"
  },
  {
    "num": 280,
    "question": "Materiala əsasən, aşağıdakılardan hansı satışa çəkilən məsrəflərə (satış xərclərinə) aid edilir?",
    "options": [
      "Anbarda saxlanılan xammalın ilkin alış qiyməti",
      "İstehsalat binasının sığorta xərcləri",
      "Xammalın anbara gətirilməsi üçün ödənilən yükdaşıma haqqı",
      "Marketinq və satış məsrəfləri",
      "Mühasibatlıq şöbəsinin əməkdaşlarına verilən əmək haqqı"
    ],
    "correct": "Marketinq və satış məsrəfləri"
  },
  {
    "num": 281,
    "question": "Normativ metod tətbiq edilərkən müəyyən olunmuş normalar (material, əmək və istehsal qaimə xərcləri) hansı müddətdən bir yoxlanılmalıdır?",
    "options": [
      "Yalnız müəssisə zərər etdiyi hesabat ilinin sonunda yoxlanılmalıdır",
      "Hər 10 ildən bir dövlət orqanları tərəfindən müəyyən edilməlidir",
      "Yalnız müəssisə rəhbərliyi dəyişdiyi halda, bir dəfə yoxlanılmalıdır",
      "Cari vəziyyətdən asılı olaraq mütəmadi olaraq yoxlanılmalı və zəruri halda yenidən baxılmalıdır",
      "Bir dəfə müəyyən olunduqdan sonra ehtiyat bitənə qədər dəyişdirilməməlidir"
    ],
    "correct": "Cari vəziyyətdən asılı olaraq mütəmadi olaraq yoxlanılmalı və zəruri halda yenidən baxılmalıdır"
  },
  {
    "num": 282,
    "question": "Pərakəndə satış qiymətləri metodunda ehtiyatın maya dəyəri hansı qaydada müəyyən edilir?",
    "options": [
      "Ehtiyatın ilkin alış qiymətindən amortizasiya çıxılması yolu ilə",
      "Müstəqil qiymətləndiricinin təyin etdiyi ədalətli dəyəri əsas götürməklə",
      "Ehtiyatın satış dəyərinin müvafiq ümumi marja (mənfəət) faizi qədər azaldılması yolu ilə",
      "İstehsal zamanı çəkilən bütün xərclərin cəmini vahid sayına bölmək yolu ilə",
      "Bazar qiymətinin üzərinə nəqliyyat və gömrük xərclərini əlavə etmək yolu ilə"
    ],
    "correct": "Ehtiyatın satış dəyərinin müvafiq ümumi marja (mənfəət) faizi qədər azaldılması yolu ilə"
  },
  {
    "num": 283,
    "question": "MHBS (IFRS) 16-ya əsasən, icarədar üçün \"istifadə hüququ olan aktivin\" ilkin dəyərinə hansı element daxil edilir?",
    "options": [
      "İcarə öhdəliyinin diskontlaşdırılmış dəyəri, ilkin birbaşa məsrəflər və bərpa rezervləri",
      "Yalnız icarə müddəti ərzində ödəniləcək dividendlər",
      "İcarəyə verən şirkətin bütün inzibati xərcləri",
      "Aktivin icarə müddəti bitdikdən sonra satılacağı bazar qiyməti",
      "İcarədarın gələcək 10 illik mənfəət proqnozu"
    ],
    "correct": "İcarə öhdəliyinin diskontlaşdırılmış dəyəri, ilkin birbaşa məsrəflər və bərpa rezervləri"
  },
  {
    "num": 284,
    "question": "Aktivin ilkin dəyəri 200 000 , ləğv dəyəri 5 000 və faydalı ömrü 10 il olarsa, 3 il istifadədən sonra düzxətt metodu ilə qalıq balans dəyəri nə qədər olar?",
    "options": [
      "180 500",
      "136 500",
      "141 500",
      "150 000",
      "195 000"
    ],
    "correct": "141 500"
  },
  {
    "num": 285,
    "question": "Əgər TTA obyekti ödənişin möhlətlə verilməsi şərti ilə əldə edilirsə, obyekt balansda hansı dəyərlə tanınır?",
    "options": [
      "Bazar iştirakçılarının təklif etdiyi ən yüksək qiymətlə",
      "Müqavilədə göstərilən nominal qiymətlə",
      "Bütün illər üzrə ödəniləcək məbləğlərin sadə cəmi ilə",
      "Aktivin yalnız ləğv dəyəri ilə",
      "Gələcəkdə ödəniləcək pul vəsaitlərinin cari (diskontlaşdırılmış) dəyəri ilə"
    ],
    "correct": "Gələcəkdə ödəniləcək pul vəsaitlərinin cari (diskontlaşdırılmış) dəyəri ilə"
  },
  {
    "num": 286,
    "question": "IAS 16-ya əsasən, TTA obyektlərinin ilkin dəyərinə (kapitallaşdırılan xərclərə) aşağıdakılardan hansı daxil edilmir?",
    "options": [
      "Sahənin (meydançanın) hazırlanması üzrə məsrəflər",
      "Obyektin quraşdırılması və yığılması üzrə peşəkar xidmət haqları",
      "Aktivin təyinat yerinə gətirilməsi üzrə nəqliyyat xərcləri",
      "Yeni istehsal kompleksinin açılışına və yeni məhsulun reklamına çəkilən məsrəflər",
      "İdxal rüsumları və əvəzləşdirilməyən vergilər"
    ],
    "correct": "Yeni istehsal kompleksinin açılışına və yeni məhsulun reklamına çəkilən məsrəflər"
  },
  {
    "num": 287,
    "question": "\"İstifadənin qiymətliliyi\" (Value in use) dedikdə nə başa düşülür?",
    "options": [
      "Aktivin bazarda hazırkı satışından əldə olunan nağd vəsait",
      "Aktivin amortizasiya olunmayan qalıq dəyəri",
      "Aktivin sığorta dəyəri ilə bazar dəyəri arasındakı fərq",
      "Aktivin davamlı istifadəsindən və istismar müddətinin sonunda satışından gözlənilən pul axınlarının diskontlaşdırılmış dəyəri",
      "Aktivin ilkin alınma anında ödənilən nağd pulun məbləği"
    ],
    "correct": "Aktivin davamlı istifadəsindən və istismar müddətinin sonunda satışından gözlənilən pul axınlarının diskontlaşdırılmış dəyəri"
  },
  {
    "num": 288,
    "question": "Aktivin balans dəyəri 150 000 , istifadə dəyəri 100 000 və mümkün xalis satış qiyməti 80 000 olarsa, qiymətdəndüşmədən olan zərər nə qədərdir?",
    "options": [
      "Zərər yoxdur",
      "70 000",
      "20 000",
      "50 000",
      "150 000"
    ],
    "correct": "50 000"
  },
  {
    "num": 289,
    "question": "MHBS (IAS) 36-ya əsasən, aktivin \"Ödənilmə dəyəri\" (Recoverable amount) necə müəyyən edilir?",
    "options": [
      "Aktivin tarixi dəyəri ilə yığılmış amortizasiyasının fərqi kimi",
      "Bazar iştirakçıları tərəfindən müəyyən edilən ən aşağı qiymət kimi",
      "Aktivin balans dəyəri ilə ləğv dəyərinin cəmi kimi",
      "Aktivin yalnız istifadənin qiymətliliyi (istifadə dəyəri) kimi",
      "Aktivin satış xərcləri çıxılmaqla ədalətli dəyəri ilə istifadənin qiymətliliyindən ən yüksək olanı"
    ],
    "correct": "Aktivin satış xərcləri çıxılmaqla ədalətli dəyəri ilə istifadənin qiymətliliyindən ən yüksək olanı"
  },
  {
    "num": 290,
    "question": "Uzunmüddətli aktivlərin təsnifatına görə aşağıdakılardan hansı \"Maddi aktivlər\" qrupuna aiddir?",
    "options": [
      "Patentlər və texnoloji nou-haular",
      "Kompüter proqramları və lisenziyalar",
      "Müəllif hüquqları və ticarət nişanları",
      "İnvestisiyalı daşınmaz əmlak və bioloji aktivlər",
      "Qudvil (müəssisənin nüfuzu)"
    ],
    "correct": "İnvestisiyalı daşınmaz əmlak və bioloji aktivlər"
  },
  {
    "num": 291,
    "question": "Aktivin ilkin dəyəri 50.000 AZN, likvidasiya dəyəri 5.000 AZN və faydalı istifadə müddəti 9 il olarsa, düzxətt metodu ilə illik amortizasiya məbləği nə qədərdir?",
    "options": [
      "5.555 AZN",
      "50.000 AZN",
      "6.000 AZN",
      "5.000 AZN",
      "4.500 AZN"
    ],
    "correct": "5.000 AZN"
  },
  {
    "num": 292,
    "question": "\"İlkin dəyər\" (Cost) anlayışının ən düzgün tərifi hansıdır?",
    "options": [
      "Aktivin faydalı ömür müddətinin sonunda malik olacağı təxmini dəyərdir",
      "Aktivin sığorta şirkəti tərəfindən müəyyən edilmiş bərpa dəyəridir",
      "Aktivin istifadə edildiyi illər ərzində hesablanmış cəmi amortizasiyadır",
      "Aktivin əldə edilməsi və ya tikilməsi üçün ödənilmiş pul vəsaitlərinin məbləği və ya verilmiş digər qarşı təqdimolunmanın ədalətli dəyəridir",
      "Aktivin yalnız quraşdırılması üçün çəkilən xərclərin cəmidir"
    ],
    "correct": "Aktivin əldə edilməsi və ya tikilməsi üçün ödənilmiş pul vəsaitlərinin məbləği və ya verilmiş digər qarşı təqdimolunmanın ədalətli dəyəridir"
  },
  {
    "num": 293,
    "question": "Pərakəndə satış qiymətləri metodu hansı növ ehtiyatların uçotu zamanı daha çox tətbiq olunur?",
    "options": [
      "Qiyməti bazarda heç vaxt dəyişməyən sabit xammallar üçün",
      "Yalnız gələcəkdə istehsal olunması planlaşdırılan xidmət ehtiyatları üçün",
      "Yalnız bir ədəd olan və çox baha qiymətə satılan xüsusi avadanlıqlar üçün",
      "İstehsalı hələ başa çatmamış bitməmiş istehsalat qalıqları üçün",
      "Çoxlu sayda olan və sürətlə satılan, oxşar marja faizinə malik ehtiyatlar üçün"
    ],
    "correct": "Çoxlu sayda olan və sürətlə satılan, oxşar marja faizinə malik ehtiyatlar üçün"
  },
  {
    "num": 294,
    "question": "Normativ metoddan (standart kost) istifadə etmək üçün əsas tələb aşağıdakılardan hansıdır?",
    "options": [
      "Məhsulun bazar qiymətinin maya dəyərindən mütləq aşağı olması",
      "Müəssisənin yalnız pərakəndə satış sahəsində fəaliyyət göstərməsi",
      "Müəssisənin bütün ehtiyatlarının mütləq şəkildə eyni qiymətə alınması",
      "Bu metodun yalnız xarici ölkədən idxal edilən mallara tətbiq olunması",
      "Hesablamanın nəticəsində alınan kəmiyyətin faktiki maya dəyərinə yaxın olması"
    ],
    "correct": "Hesablamanın nəticəsində alınan kəmiyyətin faktiki maya dəyərinə yaxın olması"
  },
  {
    "num": 295,
    "question": "Ehtiyatların dəyərinin silinməsi (qiymətdən düşməsi) və ya ehtiyat itkiləri üzrə məsrəflər maliyyə hesabatlarında necə əks olunur?",
    "options": [
      "Bu itkilər ehtiyatın maya dəyərinə əlavə edilərək kapitallaşdırılır",
      "Bu məbləğlər yalnız müəssisə ləğv edildikdə nəzərə alınır",
      "Bu itkilər baş verdiyi dövrün xərcləri kimi tanınır",
      "İtkilər növbəti 5 il ərzində bərabər hissələrlə amortizasiya olunur",
      "Bu məbləğlər kapitalın artımı kimi göstərilir"
    ],
    "correct": "Bu itkilər baş verdiyi dövrün xərcləri kimi tanınır"
  },
  {
    "num": 296,
    "question": "Ehtiyatların satılması zamanı onların balans dəyəri nə vaxt xərc kimi tanınır?",
    "options": [
      "Həmin ehtiyatların satışından gəlirin tanındığı (realizə olunduğu) anda",
      "Müştəri tərəfindən sifariş verildiyi tarixdə",
      "Mallar anbardan çıxıb nəqliyyat vasitəsinə yükləndiyi an",
      "Malların istehsalına başlandığı tarixdə",
      "Yalnız hesabat ilinin son günündə (31 dekabr)"
    ],
    "correct": "Həmin ehtiyatların satışından gəlirin tanındığı (realizə olunduğu) anda"
  },
  {
    "num": 297,
    "question": "Ehtiyatların maya dəyərindən aşağı səviyyəyə silinməsinə səbəb olan şərait aradan qalxdıqda və satışın xalis mümkün qiyməti (SXMQ) yenidən artdıqda hansı prosedur tətbiq edilir?",
    "options": [
      "Ehtiyatın dəyəri 50% artırılaraq ehtiyat kapitalına daxil edilir",
      "Silinmiş məbləğ gələcək dövrlərin gəliri kimi tanınır",
      "Ehtiyatın dəyəri birbaşa ədalətli bazar qiymətinə qaldırılır",
      "Heç bir bərpa işi aparılmır, ehtiyat silinmiş dəyərlə qalır",
      "Əvvəllər silinmiş məbləğ maya dəyəri həddində bərpa edilir"
    ],
    "correct": "Əvvəllər silinmiş məbləğ maya dəyəri həddində bərpa edilir"
  },
  {
    "num": 298,
    "question": "Müəssisənin istehsalatda istifadə etdiyi xammalın bazar qiyməti aşağı düşmüşdür. Lakin bu xammaldan hazırlanan hazır məhsulun maya dəyərindən yüksək qiymətə satılacağı gözlənilir. Bu halda xammalın uçot dəyəri ilə bağlı hansı addım atılmalıdır?",
    "options": [
      "Xammal dərhal bazar qiymətinə qədər silinməlidir",
      "Xammal ədalətli dəyərlə yenidən qiymətləndirilməlidir",
      "Xammal aktivlərdən silinərək birbaşa xərcə daxil edilməlidir",
      "Xammal maya dəyərindən aşağı səviyyəyə silinə bilməz, maya dəyəri ilə saxlanılır",
      "Xammalın dəyəri mütləq 10% azaldılmalıdır"
    ],
    "correct": "Xammal maya dəyərindən aşağı səviyyəyə silinə bilməz, maya dəyəri ilə saxlanılır"
  },
  {
    "num": 299,
    "question": "MHBS (IAS) 2-yə əsasən, ehtiyatların ilkin (maya) dəyəri 2500 manat, satışın xalis mümkün qiyməti (SXMQ) isə 2000 manatdırsa, bu aktiv maliyyə hesabatlarında hansı məbləğlə əks olunmalıdır?",
    "options": [
      "2500 manat (İlkin alış qiyməti dəyişməz qaldığı üçün)",
      "500 manat (Yalnız aradakı fərq məbləği ilə)",
      "4500 manat (Hər iki məbləğin cəmi ilə)",
      "2000 manat (Maya dəyəri və SXMQ-dən ən aşağı olanı ilə)",
      "2250 manat (Hər iki qiymətin orta göstəricisi ilə)"
    ],
    "correct": "2000 manat (Maya dəyəri və SXMQ-dən ən aşağı olanı ilə)"
  },
  {
    "num": 300,
    "question": "Aşağıdakılardan hansı aktiv qrupu MHBS (IAS) 16 standartının tətbiq dairəsinə daxil deyil?",
    "options": [
      "Təsərrüfat fəaliyyətində istifadə olunan torpaq sahələri",
      "Şirkət tərəfindən istifadə edilən nəqliyyat vasitələri",
      "Satış üçün saxlanılmış uzunmüddətli aktivlər (MHBS 5) və bərpa olunmayan təbii resurs ehtiyatları",
      "İstehsalatda istifadə olunan dəzgah və avadanlıqlar",
      "Müəssisənin inzibati məqsədlər üçün istifadə etdiyi binalar"
    ],
    "correct": "Satış üçün saxlanılmış uzunmüddətli aktivlər (MHBS 5) və bərpa olunmayan təbii resurs ehtiyatları"
  },
  {
    "num": 301,
    "question": "MHBS (IAS) 16 standartına əsasən, Torpaq, tikili və avadanlıqların (TTA) \"Balans dəyəri\" necə hesablanır?",
    "options": [
      "Aktivin tanındığı məbləğdən (ilkin dəyərdən) yığılmış amortizasiya və qiymətdəndüşmədən olan zərərlər çıxılmaqla",
      "Aktivin əldə edilməsi üçün çəkilən yalnız nəqliyyat xərcləri kimi",
      "Aktivin faydalı istifadə müddəti ərzində yaradacağı ümumi gəlir kimi",
      "Aktivin ilkin dəyəri ilə likvidasiya dəyərinin cəmi kimi",
      "Aktivin yalnız bazardakı cari satış qiyməti ilə"
    ],
    "correct": "Aktivin tanındığı məbləğdən (ilkin dəyərdən) yığılmış amortizasiya və qiymətdəndüşmədən olan zərərlər çıxılmaqla"
  },
  {
    "num": 302,
    "question": "\"Sair açıqlamalar\" bölməsində müəssisənin hüquqi statusu ilə bağlı hansı məlumatlar verilməlidir?",
    "options": [
      "Müəssisənin bütün rəqiblərinin hüquqi ünvanları",
      "Müəssisənin rəhbərliyinin ailə üzvləri haqqında qeyri-maliyyə məlumatları",
      "Yalnız təşkilatın vergi ödəyicisinin eyniləşdirmə nömrəsi (VÖEN)",
      "Təşkilatın daimi yerləşdiyi yer, hüquqi forması, ünvanı və ana şirkətin adı",
      "Təşkilatın gələcəkdə açmağı planlaşdırdığı bütün xarici filialların siyahısı"
    ],
    "correct": "Təşkilatın daimi yerləşdiyi yer, hüquqi forması, ünvanı və ana şirkətin adı"
  },
  {
    "num": 303,
    "question": "Müəssisənin kapitalı haqqında qeydlərdə hansı növ informasiyaların açıqlanması tələb olunur?",
    "options": [
      "Kapitalın yalnız dollar ekvivalenti ilə ifadə olunmuş bazar qiyməti",
      "Kapitalın nədən ibarət olması, idarə edilmə məqsədləri və kənar məhdudiyyətlərin olub-olmaması haqqında keyfiyyət və kəmiyyət göstəriciləri",
      "Yalnız dövlət tərəfindən müəssisəyə verilən subsidiyaların həcmi",
      "Səhmdarların şəxsi bank borcları haqqında məlumatlar",
      "Yalnız müəssisənin bank hesablarındakı qalıq məbləğlər"
    ],
    "correct": "Kapitalın nədən ibarət olması, idarə edilmə məqsədləri və kənar məhdudiyyətlərin olub-olmaması haqqında keyfiyyət və kəmiyyət göstəriciləri"
  },
  {
    "num": 304,
    "question": "Uçot siyasəti haqqında açıqlamalarda müəssisə mütləq hansı məlumatı qeyd etməlidir?",
    "options": [
      "Müəssisədə çalışan bütün işçilərin siyahısını və vəzifələrini",
      "Müəssisənin gələcək 10 ildə əldə edəcəyi dəqiq mənfəət məbləğini",
      "Rəqib şirkətlərin tətbiq etdiyi uçot metodlarının müqayisəsini",
      "Maliyyə hesabatlarının hazırlanması zamanı istifadə olunan qiymətləndirmə bazasını (məsələn, tarixi dəyər və ya ədalətli dəyər)",
      "Yalnız hesabat dövründə baş vermiş bütün nağd pul alış-verişlərini"
    ],
    "correct": "Maliyyə hesabatlarının hazırlanması zamanı istifadə olunan qiymətləndirmə bazasını (məsələn, tarixi dəyər və ya ədalətli dəyər)"
  },
  {
    "num": 305,
    "question": "Qeydlərdə informasiyanın təqdim edilmə ardıcıllığı adətən necə qurulur?",
    "options": [
      "Maddələrin əhəmiyyətinə görə ən böyük məbləğdən ən kiçik məbləğə doğru",
      "Heç bir ardıcıllıq gözlənilmədən, qarışıq şəkildə təqdim edilir",
      "Yalnız pul vəsaitlərinin hərəkəti hesabatındakı ardıcıllığı əsas götürməklə",
      "Maliyyə hesabatı formalarında maddələrin verildiyi ardıcıllığa uyğun və onlara çarpaz istinadlar verməklə",
      "Əlifba sırası ilə bütün aktiv və öhdəlikləri qruplaşdırmaqla"
    ],
    "correct": "Maliyyə hesabatı formalarında maddələrin verildiyi ardıcıllığa uyğun və onlara çarpaz istinadlar verməklə"
  },
  {
    "num": 306,
    "question": "\"Qeydlər\"in (Notes) maliyyə hesabatlarındakı rolu haqqında hansı fikir doğrudur?",
    "options": [
      "Yalnız vergi orqanları üçün nəzərdə tutulmuş gizli məlumatlar toplusudur",
      "Yalnız müəssisə rəhbərliyinin gələcək planlarını əks etdirən qeyri-rəsmi sənəddir",
      "Maliyyə hesabatı formalarından sonra hazırlanan könüllü bir əlavədir",
      "Maliyyə hesabatlarının ayrılmaz hissəsidir və uçot siyasəti, həmçinin hesabatlarda əks olunmayan zəruri informasiyanı təqdim edir",
      "Hesabatlardakı rəqəmlərin səhv olduğunu sübut edən sənədlərdir"
    ],
    "correct": "Maliyyə hesabatlarının ayrılmaz hissəsidir və uçot siyasəti, həmçinin hesabatlarda əks olunmayan zəruri informasiyanı təqdim edir"
  },
  {
    "num": 307,
    "question": "Satışın xalis mümkün qiyməti (SXMQ) ilə Ədalətli dəyər arasındakı əsas fərq nədədir?",
    "options": [
      "Bu iki anlayış arasında heç bir iqtisadi və ya uçot fərqi yoxdur",
      "SXMQ yalnız xammallara, ədalətli dəyər isə yalnız hazır məhsullara tətbiq edilir",
      "SXMQ təşkilat üçün spesifik dəyərdir, ədalətli dəyər isə bazarda müəyyən olunan spesifik olmayan dəyərdir",
      "Ədalətli dəyər müəssisənin daxili hesablamasıdır, SXMQ isə yalnız xarici auditorlar tərəfindən müəyyən edilir",
      "SXMQ həmişə ədalətli dəyərdən daha yüksək olur"
    ],
    "correct": "SXMQ təşkilat üçün spesifik dəyərdir, ədalətli dəyər isə bazarda müəyyən olunan spesifik olmayan dəyərdir"
  },
  {
    "num": 308,
    "question": "MHBS-ə uyğun olaraq ehtiyatlar hansı kəmiyyətlə qiymətləndirilməlidir?",
    "options": [
      "Yalnız alış qiyməti və nəqliyyat xərclərinin cəmi ilə",
      "İlkin (maya) dəyəri və satışın xalis mümkün qiymətindən (SXMQ) ən aşağı olanı ilə",
      "İlkin dəyər və ədalətli dəyərdən ən yüksək olanı ilə",
      "Yalnız ədalətli dəyər (bazar qiyməti) ilə",
      "Satışın xalis mümkün qiyməti və maya dəyərinin cəmi ilə"
    ],
    "correct": "İlkin (maya) dəyəri və satışın xalis mümkün qiymətindən (SXMQ) ən aşağı olanı ilə"
  },
  {
    "num": 309,
    "question": "Reklam məqsədilə pulsuz paylanılan nümunələrin (məsələn, kosmetik vasitələr) uçotu necə aparılmalıdır?",
    "options": [
      "Onlar qeyri-maddi aktiv kimi kapitallaşdırılır",
      "Onlar yalnız müştəriyə verildiyi anda xərc kimi tanınır, o vaxta qədər aktiv sayılır",
      "Onlar ehtiyatlara aid edilmir, istehsal məsrəfləri baş verdiyi anda xərclərə silinir",
      "Onlar \"Sair ehtiyatlar\" maddəsində balans dəyəri ilə əks olunur",
      "Onlar satış qiyməti ilə hazır məhsul kimi uçota alınır"
    ],
    "correct": "Onlar ehtiyatlara aid edilmir, istehsal məsrəfləri baş verdiyi anda xərclərə silinir"
  },
  {
    "num": 310,
    "question": "Ehtiyat hissələri və texniki xidmət avadanlıqları hansı halda ehtiyat kimi deyil, Torpaq, Tikili və Avadanlıq (TTA) kimi təsnifləşdirilir?",
    "options": [
      "Onlar xarici ölkədən idxal edildiyi halda",
      "Onların dəyəri müəyyən edilmiş limitdən yüksək olduqda",
      "Onlar yalnız istehsal prosesində birbaşa iştirak etdikdə",
      "Onların istifadə müddəti bir ildən artıq olduqda və TTA-nın tanınma kriteriyalarına cavab verdikdə",
      "Onlar yalnız təmir məqsədilə anbarda saxlanıldıqda"
    ],
    "correct": "Onların istifadə müddəti bir ildən artıq olduqda və TTA-nın tanınma kriteriyalarına cavab verdikdə"
  },
  {
    "num": 311,
    "question": "Materiala əsasən, aşağıdakılardan hansı ehtiyatların tərkibinə aid edilmir?",
    "options": [
      "İcarəyə verildikdən sonra satış üçün nəzərdə tutulan avtomobillər",
      "Yığımdan sonra kənd təsərrüfatı məhsulları",
      "Satış məqsədi ilə yaradılan kompüter proqram təminatı",
      "Satış məqsədi üçün alınmış torpaq və binalar",
      "Qısamüddətə mənfəət götürmək məqsədilə əldə olunan maliyyə aktivləri (ticarət investisiyaları)"
    ],
    "correct": "Qısamüddətə mənfəət götürmək məqsədilə əldə olunan maliyyə aktivləri (ticarət investisiyaları)"
  },
  {
    "num": 312,
    "question": "Ehtiyatlar digər aktivlərin (məsələn, əsas vəsaitin) yaradılması üçün istifadə olunarsa, onların dəyəri ilə bağlı hansı prosedur həyata keçirilir?",
    "options": [
      "Yaradılan aktivin ilkin dəyərinə daxil edilir (kapitallaşdırılır)",
      "Ədalətli dəyərlə yenidən qiymətləndirilir",
      "Birbaşa dövrün xərclərinə silinir",
      "Gələcək dövrlərin xərcləri kimi uçota alınır",
      "Ehtiyat kimi balansda saxlanılmağa davam edir"
    ],
    "correct": "Yaradılan aktivin ilkin dəyərinə daxil edilir (kapitallaşdırılır)"
  },
  {
    "num": 313,
    "question": "Ehtiyatların balans dəyəri nə zaman mənfəət və ya zərər haqqında hesabatda xərc kimi tanınır?",
    "options": [
      "Ehtiyatlar istehsal prosesinə buraxıldığı anda",
      "Hesabat dövrünün sonunda inventarizasiya aparıldıqda",
      "Ehtiyatların dəyəri təchizatçıya ödənildiyi anda",
      "Ehtiyatlar anbara mədaxil edildiyi anda",
      "Həmin ehtiyatlar faktiki olaraq satıldığı anda"
    ],
    "correct": "Həmin ehtiyatlar faktiki olaraq satıldığı anda"
  },
  {
    "num": 314,
    "question": "FOB (franko-bort) şərtləri ilə mal alındıqda, mülkiyyət hüququ alıcıya nə vaxt keçir?",
    "options": [
      "Mallar daşıyıcı şirkətə təhvil verildiyi an",
      "Ödəniş bank hesabı vasitəsilə həyata keçirildiyi zaman",
      "Gəmi alıcının ölkəsinin limanına çatdığı zaman",
      "Mallar satıcının limanında gəminin bortuna yükləndiyi zaman",
      "Mallar alıcının anbarına boşaldıldığı zaman"
    ],
    "correct": "Mallar satıcının limanında gəminin bortuna yükləndiyi zaman"
  },
  {
    "num": 315,
    "question": "\"Maliyyə vəziyyəti haqqında hesabatda\" (Balans) minimum hansı maddələrin olması mütləqdir?",
    "options": [
      "Müəssisənin gələcək 5 il üçün satış proqnozları və marketinq büdcəsi",
      "Şirkətin bazar payı və rəqiblərin aktivləri haqqında məlumatlar",
      "Yerli icra hakimiyyəti tərəfindən verilən dotasiyaların siyahısı",
      "Torpaq, tikili və avadanlıqlar, qeyri-maddi aktivlər, ehtiyatlar, ticarət debitor və kreditor borcları",
      "Yalnız şirkət direktorunun və səhmdarların şəxsi əmlakları"
    ],
    "correct": "Torpaq, tikili və avadanlıqlar, qeyri-maddi aktivlər, ehtiyatlar, ticarət debitor və kreditor borcları"
  },
  {
    "num": 316,
    "question": "Xüsusi kapitaldakı dəyişikliklər haqqında hesabatda (Statement of Changes in Equity) aşağıdakı məlumatlardan hansının əks etdirilməsi tələb olunur?",
    "options": [
      "Uzunmüddətli bank kreditlərinin faiz dərəcələri",
      "Yalnız müəssisənin ləğvi zamanı satılacaq aktivlərin bazar dəyəri",
      "Müəssisənin bütün debitor borclarının siyahısı və onların ödənmə tarixi",
      "Dövr ərzində mülkiyyətçilər arasında bölüşdürülən dividendlərin məbləği və ümumi məcmu gəlirin bölgüsü",
      "İşçilərin sosial sığorta haqlarının hesablanma metodikası"
    ],
    "correct": "Dövr ərzində mülkiyyətçilər arasında bölüşdürülən dividendlərin məbləği və ümumi məcmu gəlirin bölgüsü"
  },
  {
    "num": 317,
    "question": "Xərclərin təhlili zamanı \"Xərclərin təyinatı (funksiyası) üzrə\" metodda hansı maddə mütləq ayrıca göstərilir?",
    "options": [
      "Hazır məhsul ehtiyatlarındakı dəyişikliklər",
      "İstifadə edilmiş xammalın xarakteri",
      "Satışın maya dəyəri",
      "İşçilərin mükafatlandırılması xərcləri",
      "Amortizasiya üzrə xərclər"
    ],
    "correct": "Satışın maya dəyəri"
  },
  {
    "num": 318,
    "question": "\"Məcmu gəlir haqqında hesabat\" (Statement of Comprehensive Income) özündə hansı iki əsas bölməni birləşdirir?",
    "options": [
      "Dividendlər haqqında hesabat və Vergi bəyannamələri",
      "Mənfəət yaxud zərər haqqında hesabat və Sair məcmu gəlir haqqında bölmə",
      "Cari aktivlər və Uzunmüddətli öhdəliklər bölmələri",
      "Aktivlər haqqında bölmə və Öhdəliklər haqqında bölmə",
      "Pul vəsaitləri bölməsi və Ehtiyatlar bölməsi"
    ],
    "correct": "Mənfəət yaxud zərər haqqında hesabat və Sair məcmu gəlir haqqında bölmə"
  },
  {
    "num": 319,
    "question": "Aktiv və ya öhdəlik hansı halda \"qısamüddətli\" (cari) kimi təsnifləşdirilməlidir?",
    "options": [
      "Aktivin dəyəri müəssisənin nizamnamə kapitalından çoxdursa",
      "Yalnız rəhbərliyin şəxsi qərarı ilə uzunmüddətli kateqoriyadan çıxarılıbsa",
      "Aktiv yalnız fiziki formada (məsələn, bina) mövcuddursa",
      "Reallaşdırılması və ya ödənilməsi hesabat dövrü qurtardıqdan sonrakı 12 ay ərzində gözlənilirsə",
      "Öhdəliyin ödənilməsi üçün 2 ildən artıq möhlət hüququ varsa"
    ],
    "correct": "Reallaşdırılması və ya ödənilməsi hesabat dövrü qurtardıqdan sonrakı 12 ay ərzində gözlənilirsə"
  },
  {
    "num": 320,
    "question": "\"Fasiləsiz fəaliyyət\" (Going concern) prinsipi ilə bağlı hansı fikir doğrudur?",
    "options": [
      "Əgər təşkilat fəaliyyətini dayandırmaq niyyətindədirsə, hesabat tərtib etməyə ehtiyac yoxdur.",
      "Təşkilat öz fəaliyyətini yaxın gələcəkdə davam etdirəcəyi ehtimalı ilə hesabat tərtib etməlidir.",
      "Bu prinsip yalnız dövlət müəssisələrinə şamil edilir.",
      "Təşkilat ləğv olunma mərhələsində olsa belə, hesabatlar həmişə eyni prinsiplə tərtib edilir.",
      "Bu prinsip yalnız pul vəsaitlərinin hərəkəti hesabatına aiddir."
    ],
    "correct": "Təşkilat öz fəaliyyətini yaxın gələcəkdə davam etdirəcəyi ehtimalı ilə hesabat tərtib etməlidir."
  },
  {
    "num": 321,
    "question": "Hesabat verən təşkilat maliyyə hesabatlarının tam komplektini minimum hansı tezliklə təqdim etməlidir?",
    "options": [
      "Beş ildə bir dəfə tam komplekt şəklində",
      "İldə iki dəfə (yarımillik).",
      "Yalnız rəhbərlik ehtiyac duyduqda.",
      "Hər üç ildən bir.",
      "Hər il (minimum ildə bir dəfə)."
    ],
    "correct": "Hər il (minimum ildə bir dəfə)."
  },
  {
    "num": 322,
    "question": "\"Əhəmiyyətlilik və aqreqasiyalaşdırma\" tələbinə görə aşağıdakı fikirlərdən hansı doğrudur?",
    "options": [
      "Bütün maddələr, məbləğindən asılı olmayaraq, həmişə ayrıca göstərilməlidir.",
      "\"Qeydlər\" bölməsində informasiyanın aqreqasiyalaşdırılması qadağandır.",
      "Əhəmiyyətli maddələri gizlətmək üçün onları əhəmiyyətsiz maddələrlə birləşdirmək olar.",
      "Əhəmiyyətli maddələr ayrıca əks etdirilməli, əhəmiyyətsiz maddələr isə digərləri ilə birləşdirilə bilər.",
      "Yalnız xərclər aqreqasiyalaşdırıla bilər, gəlirlər isə mütləq detallandırılmalıdır."
    ],
    "correct": "Əhəmiyyətli maddələr ayrıca əks etdirilməli, əhəmiyyətsiz maddələr isə digərləri ilə birləşdirilə bilər."
  },
  {
    "num": 323,
    "question": "Ehtiyatlar uçotda nə zaman aktiv kimi tanınır?",
    "options": [
      "Malların istehsalına başlanıldığı zaman",
      "Yalnız mallar faktiki olaraq müştəriyə satıldığı zaman",
      "Malın dəyəri satıcıya tam ödənildiyi zaman",
      "Mallar anbara daxil olduğu tarixdən asılı olmayaraq, müqavilə bağlandığı zaman",
      "Mülkiyyət hüququ ilə bağlı əhəmiyyətli risklər və faydalar təşkilata keçdiyi zaman"
    ],
    "correct": "Mülkiyyət hüququ ilə bağlı əhəmiyyətli risklər və faydalar təşkilata keçdiyi zaman"
  },
  {
    "num": 324,
    "question": "Satışın xalis mümkün qiyməti necə müəyyən edilir?",
    "options": [
      "Aktivin bazarda mövcud olan cari satış qiyməti ilə",
      "Aktivin ilkin dəyərindən amortizasiya ayırmalarını çıxmaqla",
      "Hesabi satış qiymətindən istehsalın başa çatdırılması və satış üçün zəruri olan hesabi məsrəflər çıxılmaqla",
      "Bazar iştirakçıları arasında öhdəliyin ödənilməsi üçün nəzərdə tutulan məbləğlə",
      "Aktivin alış qiyməti üzərinə nəqliyyat xərclərini əlavə etməklə"
    ],
    "correct": "Hesabi satış qiymətindən istehsalın başa çatdırılması və satış üçün zəruri olan hesabi məsrəflər çıxılmaqla"
  },
  {
    "num": 325,
    "question": "MHBS (IAS) 2 standartına əsasən, aşağıdakılardan hansı ehtiyatların tərifinə aid deyil?",
    "options": [
      "Xidmət göstərilməsi prosesində istifadə olunacaq materiallar",
      "Məhsul istehsalında istifadə olunacaq xammallar",
      "Adi fəaliyyət gedişində satış üçün nəzərdə tutulmuş aktivlər",
      "Sonradan satış üçün istehsal prosesində olan aktivlər",
      "Müəssisənin inzibati binalarının gələcəkdə satış məqsədilə saxlanılması"
    ],
    "correct": "Müəssisənin inzibati binalarının gələcəkdə satış məqsədilə saxlanılması"
  },
  {
    "num": 326,
    "question": "\"Qiymətdəndüşmə zərərin bərpası\" nə vaxt baş verir?",
    "options": [
      "Aktivin bazar qiyməti balans dəyərinə bərabər olduqda",
      "Qudvilin dəyəri bazar kapitallaşdırılmasından aşağı düşdükdə",
      "Aktivin amortizasiya müddəti bitdikdən sonra istifadəsi davam etdikdə",
      "Zərərin sonuncu tanınmasından sonra aktivin ödənilmə dəyərinin müəyyən edilməsi üçün istifadə olunmuş hesabi qiymətləndirmələrdə dəyişikliklər baş verdikdə",
      "Yalnız aktiv başqa bir şirkətə icarəyə verildikdə"
    ],
    "correct": "Zərərin sonuncu tanınmasından sonra aktivin ödənilmə dəyərinin müəyyən edilməsi üçün istifadə olunmuş hesabi qiymətləndirmələrdə dəyişikliklər baş verdikdə"
  },
  {
    "num": 327,
    "question": "Müəssisə maliyyə hesabatlarında qiymətdəndüşmə ilə bağlı hansı informasiyanı açıqlamağa borcludur?",
    "options": [
      "Müəssisə rəhbərliyinin aktivlərin satışı ilə bağlı şəxsi rəylərini",
      "Yalnız aktivin bazar qiymətinin dəyişməsi üzrə proqnozları",
      "Bütün aktivlərin ləğv edilməsi üçün tələb olunan hüquqi xərclərin siyahısını",
      "Dövr ərzində mənfəət və ya zərərdə tanınmış zərərlərin və onların bərpa edilmiş məbləğlərini",
      "Yalnız qudvilin gələcəkdə yarada biləcəyi ehtimal olunan mənfəəti"
    ],
    "correct": "Dövr ərzində mənfəət və ya zərərdə tanınmış zərərlərin və onların bərpa edilmiş məbləğlərini"
  },
  {
    "num": 328,
    "question": "Qiymətdəndüşmə zərəri bərpa edildikdən sonra aktivin amortizasiya ayırmaları ilə bağlı nə edilməlidir?",
    "options": [
      "Aktivin ilkin (zərərdən əvvəlki) amortizasiya norması dəyişmədən saxlanılmalıdır",
      "Amortizasiya hesablanması tamamilə dayandırılmalıdır",
      "Aktivin faydalı istifadə müddəti mütləq şəkildə artırılmalıdır",
      "Amortizasiya yalnız aktivin bazar qiyməti yenidən düşdükdə hesablanmalıdır",
      "Aktivin yenidən baxılmış balans dəyəri qalan xidmət müddətində mütəmadi əsasda amortizasiya edilməsi üçün korrektə olunmalıdır"
    ],
    "correct": "Aktivin yenidən baxılmış balans dəyəri qalan xidmət müddətində mütəmadi əsasda amortizasiya edilməsi üçün korrektə olunmalıdır"
  },
  {
    "num": 329,
    "question": "Yenidənqiymətləndirilmiş aktivlər üzrə əvvəllər tanınmış zərərin bərpası necə uçota alınır?",
    "options": [
      "Aktivin istifadə müddətinin qısaldılması kimi",
      "Hər bir halda birbaşa mənfəət və zərər hesabına gəlir kimi",
      "Qudvilin dəyərinin artırılması kimi",
      "Uzunmüddətli öhdəliklərin azalması kimi",
      "Yenidənqiymətləndirilmə məbləğinin artması (ehtiyatın artması) kimi"
    ],
    "correct": "Yenidənqiymətləndirilmə məbləğinin artması (ehtiyatın artması) kimi"
  },
  {
    "num": 330,
    "question": "Aktivin balans dəyəri qiymətdəndüşmə zərəri bərpa edildikdə hansı məbləğdən artıq ola bilməz?",
    "options": [
      "Aktivin bazarındakı ən yüksək satış qiymətindən",
      "Aktivin yalnız ləğv etmə (qalıq) dəyərindən",
      "Aktivin ilkin satınalma qiymətinin ikiqatından",
      "Qiymətdəndüşmə baş verməsəydi, aktivin həmin tarixə olacaq (amortizasiya çıxılmış) balans dəyərindən",
      "Müəssisənin bütün aktivlərinin ümumi orta maya dəyərindən"
    ],
    "correct": "Qiymətdəndüşmə baş verməsəydi, aktivin həmin tarixə olacaq (amortizasiya çıxılmış) balans dəyərindən"
  },
  {
    "num": 331,
    "question": "Maliyyə hesabatlarının identifikasiyası zamanı aşağıdakılardan hansı \"görünən yerdə\" yerləşdirilməli olan məlumatlara aid deyil?",
    "options": [
      "Hesabatın ayrıca bir təşkilata, yoxsa təşkilatlar qrupuna aid olması.",
      "Məbləğlərin yuvarlaqlaşdırılma səviyyəsi.",
      "Şirkətin baş mühasibinin və direktorunun ev ünvanı.",
      "Hesabatın təqdim olunma valyutası.",
      "Hesabat verən təşkilatın adı."
    ],
    "correct": "Şirkətin baş mühasibinin və direktorunun ev ünvanı."
  },
  {
    "num": 332,
    "question": "Aktivlərin rezervlər çıxılmaqla (məsələn, şübhəli borclar rezervi) əks etdirilməsi IAS 1-ə görə necə qiymətləndirilir?",
    "options": [
      "Bu, kobud qarşılıqlı əvəzetmədir və qadağandır.",
      "Bu, yalnız \"Fəaliyyətin fasiləsizliyi\" prinsipi pozulduqda mümkündür.",
      "Bu halda mütləq 3-cü maliyyə vəziyyəti hesabatı tərtib olunmalıdır.",
      "Bu, qarşılıqlı əvəzetmə hesab edilmir və standartlara uyğundur.",
      "Bu proses yalnız vergi uçotunda icazə veriləndir."
    ],
    "correct": "Bu, qarşılıqlı əvəzetmə hesab edilmir və standartlara uyğundur."
  },
  {
    "num": 333,
    "question": "Təşkilat uçot siyasətində retrospektiv dəyişiklik etdikdə və bu əvvəlki dövrə əhəmiyyətli təsir göstərdikdə neçə dənə \"Maliyyə vəziyyəti haqqında hesabat\" təqdim etməlidir?",
    "options": [
      "Retrospektiv düzəliş zamanı hesabat sayı dəyişməz qalır (2 hesabat).",
      "Yalnız son 5 ili əhatə edən 1 ümumi hesabat.",
      "3 hesabat (cari dövrün sonuna, əvvəlki dövrün sonuna və əvvəlki dövrün əvvəlinə).",
      "Hər il üçün 2 hesabat olmaqla cəmi 4 hesabat.",
      "Yalnız cari dövrün sonuna aid 1 hesabat."
    ],
    "correct": "3 hesabat (cari dövrün sonuna, əvvəlki dövrün sonuna və əvvəlki dövrün əvvəlinə)."
  },
  {
    "num": 334,
    "question": "\"Hesablama metodu\" (Accrual basis) ilə bağlı hansı fikir doğrudur?",
    "options": [
      "Bu metod Konseptual əsaslardakı tanınma kriteriyalarına ziddir.",
      "Bu metod gəlirlərin yalnız nəqd pul daxil olduqda tanınmasını tələb edir.",
      "Bütün maliyyə hesabatları, o cümlədən pul vəsaitlərinin hərəkəti hesabatı yalnız bu metodla tərtib edilir.",
      "Pul vəsaitlərinin hərəkəti haqqında hesabat istisna olmaqla, bütün hesabatlar bu metodla tərtib edilməlidir.",
      "Hesablama metodu yalnız illik dövriyyəsi yüksək olan şirkətlər üçün məcburidir."
    ],
    "correct": "Pul vəsaitlərinin hərəkəti haqqında hesabat istisna olmaqla, bütün hesabatlar bu metodla tərtib edilməlidir."
  },
  {
    "num": 335,
    "question": "\"Giriş dəyəri\" (Entry value) və \"Çıxış dəyəri\" (Exit value) bölgüsünə görə aşağıdakılardan hansı aktiv əldə edilərkən bazarda olan qiyməti (giriş dəyərini) əks etdirir?",
    "options": [
      "Yalnız amortizasiya olunmuş dəyər",
      "Yalnız aktivin satışından gözlənilən xalis daxilolmalar",
      "Ədalətli dəyər və İstifadənin qiymətliliyi",
      "İcraetmənin dəyəri və Gələcək dəyər",
      "Tarixi dəyər və Əvəzetmənin cari dəyəri"
    ],
    "correct": "Tarixi dəyər və Əvəzetmənin cari dəyəri"
  },
  {
    "num": 336,
    "question": "Maliyyə vəziyyəti haqqında hesabatda aktivin, öhdəliyin və ya xüsusi kapitalın tanınan kəmiyyəti (məbləğ) necə adlanır?",
    "options": [
      "Bazar dəyəri",
      "Balans dəyəri",
      "Nominal dəyər",
      "Gələcək dəyər",
      "Satış qiyməti"
    ],
    "correct": "Balans dəyəri"
  },
  {
    "num": 337,
    "question": "\"İcraetmənin dəyəri\" (Fulfilment value) dedikdə nə başa düşülür?",
    "options": [
      "Bazar iştirakçılarının oxşar öhdəlik üçün tələb etdikləri cari qiymətdir",
      "Təşkilatın bankdakı borclarının cəmi və onlara hesablanmış faizlərdir",
      "Müəssisənin aktivlərini bazarda satarkən əldə edə biləcəyi nağd pulun miqdarıdır",
      "Öhdəliyin yarandığı tarixdə alınmış ilkin ödənişin kəmiyyətidir",
      "Öz öhdəliklərini icra etmək üçün təşkilat tərəfindən verilməsi gözlənilən iqtisadi faydaların diskontlaşdırılmış dəyəridir"
    ],
    "correct": "Öz öhdəliklərini icra etmək üçün təşkilat tərəfindən verilməsi gözlənilən iqtisadi faydaların diskontlaşdırılmış dəyəridir"
  },
  {
    "num": 338,
    "question": "Aktivlərin və öhdəliklərin \"Cari dəyərlə\" (Current value) qiymətləndirilməsinin tarixi dəyərdən əsas fərqi nədir?",
    "options": [
      "Yalnız aktivin ilkin alınma anındakı sövdələşmə qiymətinə əsaslanır",
      "Cari dəyər heç bir halda bazar iştirakçılarının rəyini nəzərə almır",
      "Qiymətləndirmə tarixinə mövcud olan şəraitləri əks etdirmək üçün yenilənmiş informasiyadan istifadə edir",
      "Cari dəyər yalnız amortizasiya olunmuş tarixi məsrəfləri göstərir",
      "Bu bazada qiymətləndirilən maddələr heç vaxt dəyişmir və sabit qalır"
    ],
    "correct": "Qiymətləndirmə tarixinə mövcud olan şəraitləri əks etdirmək üçün yenilənmiş informasiyadan istifadə edir"
  }
];

    const els = {
      customRanges: document.getElementById('customRanges'),
      startBtn: document.getElementById('startBtn'),
      resetBtn: document.getElementById('resetBtn'),
      savedQuizBtn: document.getElementById('savedQuizBtn'),
      savedPanel: document.getElementById('savedPanel'),
      statusLine: document.getElementById('statusLine'),
      rangeLabel: document.getElementById('rangeLabel'),
      quizCount: document.getElementById('quizCount'),
      bankCount: document.getElementById('bankCount'),
      progressCard: document.getElementById('progressCard'),
      progressText: document.getElementById('progressText'),
      progressFill: document.getElementById('progressFill'),
      quizCard: document.getElementById('quizCard'),
      resultsCard: document.getElementById('resultsCard'),
      themeToggleBtn: document.getElementById('themeToggleBtn'),
      jumpInput: document.getElementById('jumpInput'),
      jumpBtn: document.getElementById('jumpBtn'),
    };

    const STORAGE_KEY = 'muhasibat.savedQuestions.v1';
    const THEME_KEY = 'politologiya.theme.v1';

    const state = {
      mode: 'setup', // setup | quiz | results
      currentIndex: 0,
      quiz: [],
      revealMap: new Set(),
      onlyReviewWrong: false,
      quizSource: 'range', // range | saved
      savedQuestionNums: loadSavedQuestions(),
      savedPanelOpen: false,
      theme: loadTheme(),
    };


    function loadTheme() {
      try {
        const raw = localStorage.getItem(THEME_KEY);
        return raw === 'light' ? 'light' : 'dark';
      } catch (err) {
        return 'dark';
      }
    }

    function persistTheme() {
      try {
        localStorage.setItem(THEME_KEY, state.theme);
      } catch (err) {
      }
    }

    function applyTheme() {
      document.body.dataset.theme = state.theme;
      if (els.themeToggleBtn) {
        els.themeToggleBtn.setAttribute('aria-label', state.theme === 'dark' ? 'İşıqlı rejimə keç' : 'Qaranlıq rejimə keç');
      }
      if (els.themeToggleText) {
        els.themeToggleText.textContent = 'Rejim';
      }
      persistTheme();
    }

    function clamp(n, min, max) {
      return Math.max(min, Math.min(max, n));
    }

    function parseCustomSelection(raw) {
      const input = String(raw || '').trim();
      if (!input) return [];

      const selected = new Set();
      const parts = input.split(',').map(part => part.trim()).filter(Boolean);

      for (const part of parts) {
        const compact = part.replace(/\s+/g, '');
        const rangeMatch = compact.match(/^(\d+)-(\d+)$/);
        if (rangeMatch) {
          let a = parseInt(rangeMatch[1], 10);
          let b = parseInt(rangeMatch[2], 10);
          if (Number.isFinite(a) && Number.isFinite(b)) {
            if (a > b) [a, b] = [b, a];
            a = clamp(a, 1, QUESTION_BANK.length);
            b = clamp(b, 1, QUESTION_BANK.length);
            for (let n = a; n <= b; n++) selected.add(n);
          }
          continue;
        }

        if (/^\d+$/.test(compact)) {
          const n = clamp(parseInt(compact, 10), 1, QUESTION_BANK.length);
          selected.add(n);
        }
      }

      return [...selected].sort((a, b) => a - b);
    }

    function shuffle(arr) {
      const a = arr.slice();
      for (let i = a.length - 1; i > 0; i--) {
        const j = Math.floor(Math.random() * (i + 1));
        [a[i], a[j]] = [a[j], a[i]];
      }
      return a;
    }

    function sample(arr, count) {
      const a = shuffle(arr);
      return a.slice(0, count);
    }

    function loadSavedQuestions() {
      try {
        const raw = localStorage.getItem(STORAGE_KEY);
        const parsed = raw ? JSON.parse(raw) : [];
        return new Set((Array.isArray(parsed) ? parsed : []).map(n => parseInt(n, 10)).filter(n => Number.isFinite(n) && n > 0));
      } catch (err) {
        return new Set();
      }
    }

    function persistSavedQuestions() {
      try {
        localStorage.setItem(STORAGE_KEY, JSON.stringify([...state.savedQuestionNums]));
      } catch (err) {
      }
    }

    function isSavedQuestion(num) {
      return state.savedQuestionNums.has(num);
    }

    function toggleSavedQuestion(num) {
      if (state.savedQuestionNums.has(num)) {
        state.savedQuestionNums.delete(num);
        els.statusLine.textContent = `Sual ${num} yadda saxlanılanlardan çıxarıldı.`;
      } else {
        state.savedQuestionNums.add(num);
        els.statusLine.textContent = `Sual ${num} yadda saxlanıldı.`;
      }
      persistSavedQuestions();
      renderSavedPanel();
      if (state.mode === 'quiz') renderQuiz();
    }

    function removeSavedQuestion(num) {
      if (!state.savedQuestionNums.has(num)) return;
      state.savedQuestionNums.delete(num);
      persistSavedQuestions();
      els.statusLine.textContent = `Sual ${num} yadda saxlanılanlardan silindi.`;
      renderSavedPanel();
      if (state.mode === 'quiz') renderQuiz();
    }

    function clearSavedQuestions() {
      if (!state.savedQuestionNums.size) {
        els.statusLine.textContent = 'Yadda saxlanılan sual yoxdur.';
        return;
      }
      const ok = confirm('Bütün yadda saxlanılan suallar silinsin?');
      if (!ok) return;
      state.savedQuestionNums.clear();
      persistSavedQuestions();
      els.statusLine.textContent = 'Bütün yadda saxlanılan suallar silindi.';
      renderSavedPanel();
      if (state.mode === 'quiz') renderQuiz();
    }

    function buildQuiz(source = state.quizSource) {
      let subset = [];
      let label = '';

      if (source === 'saved') {
        subset = QUESTION_BANK.filter(q => state.savedQuestionNums.has(q.num));
        label = 'saxlanılan suallar';
      } else {
        const customRaw = els.customRanges?.value.trim();
        if (customRaw) {
          const numbers = parseCustomSelection(customRaw);
          subset = QUESTION_BANK.filter(q => numbers.includes(q.num));
          label = `İnterval: ${customRaw}`;
        } else {
          subset = QUESTION_BANK.slice();
          label = 'Hamısı';
        }
      }

      const count = Math.min(50, subset.length);
      if (!subset.length) {
        els.statusLine.textContent = source === 'saved'
          ? 'Yadda saxlanan sual tapılmadı.'
          : 'Seçilən intervalda sual tapılmadı.';
        return;
      }

      const chosen = sample(subset, count);

      state.quiz = chosen.map((q) => {
        const shuffledOptions = shuffle(q.options.map((text, i) => ({ text, sourceIndex: i })));
        const options = shuffledOptions.map((opt) => ({
          text: opt.text,
          correct: opt.text === q.correct
        }));
        return {
          num: q.num,
          question: q.question,
          options,
          correct: q.correct,
          selected: null
        };
      });

      state.currentIndex = 0;
      state.revealMap = new Set();
      state.mode = 'quiz';
      state.onlyReviewWrong = false;
      state.quizSource = source;
      render();
      els.statusLine.textContent = source === 'saved'
        ? `Saxlanılan suallardan ${count} sual seçildi.`
        : `Sınaq başladı: ${label} aralığından ${count} sual seçildi.`;
    }

    function currentQuestion() {
      return state.quiz[state.currentIndex];
    }

    function answerQuestion(qIndex, optionText) {
      state.quiz[qIndex].selected = optionText;
      renderQuiz();
    }

    function toggleReveal(num) {
      if (state.revealMap.has(num)) state.revealMap.delete(num);
      else state.revealMap.add(num);
      renderQuiz();
    }

    function finishQuiz(confirmFirst = false) {
      if (confirmFirst && !window.confirm('Sınağı bitirmək istəyirsinizmi?')) return;
      state.mode = 'results';
      els.statusLine.textContent = 'Sınaq bitdi.';
      render();
    }

    function scoreSummary() {
      let correct = 0;
      let wrong = 0;
      let blank = 0;
      for (const q of state.quiz) {
        if (q.selected === null) {
          blank++;
        } else if (q.selected === q.correct) {
          correct++;
        } else {
          wrong++;
        }
      }
      return { correct, wrong, blank, total: state.quiz.length };
    }

    function render() {
      document.body.dataset.mode = state.mode;
      applyTheme();

      if (state.mode === 'setup') {
        els.progressCard.classList.add('hidden');
        els.quizCard.classList.add('hidden');
        els.resultsCard.classList.add('hidden');
        return;
      }
      if (state.mode === 'quiz') {
        els.progressCard.classList.remove('hidden');
        els.resultsCard.classList.add('hidden');
        els.quizCard.classList.remove('hidden');
        renderQuiz();
      }
      if (state.mode === 'results') {
        els.progressCard.classList.add('hidden');
        els.quizCard.classList.add('hidden');
        els.resultsCard.classList.remove('hidden');
        renderResults();
      }
    }

    function renderQuiz() {
      const q = currentQuestion();
      if (!q) {
        state.mode = 'results';
        renderResults();
        return;
      }

      const progress = state.currentIndex + 1;
      const total = state.quiz.length;
      els.progressText.textContent = `${progress} / ${total}`;
      els.progressFill.style.width = `${(progress / total) * 100}%`;

      const selected = q.selected;
      const reveal = state.revealMap.has(q.num);
      const saved = isSavedQuestion(q.num);

      els.quizCard.innerHTML = `
        <div class="question-meta">
          <div>Sual</div>
          <div>${progress} / ${total}</div>
        </div>
        <h2 class="qtitle">${escapeHtml(q.question)}</h2>
        <div class="options">
          ${q.options.map((opt, idx) => {
            const classes = ['option'];
            if (selected === opt.text) classes.push('selected');
            if (reveal && opt.correct) classes.push('correct');
            if (reveal && selected === opt.text && !opt.correct) classes.push('wrong');
            return `
              <button class="${classes.join(' ')}" data-q="${state.currentIndex}" data-opt="${escapeAttr(opt.text)}" type="button">
                ${letter(idx)}) ${escapeHtml(opt.text)}
              </button>
            `;
          }).join('')}
        </div>

        <div class="foot">
          <div class="btn-row">
            <button class="tiny ${saved ? 'primary' : 'ghost'}" id="saveBtn">${saved ? 'Yadda saxlanılıb' : 'Yadda saxla'}</button>
            <button class="tiny ghost" id="revealBtn">${reveal ? 'Cavabı gizlət' : 'Düzgün cavabı göstər'}</button>
          </div>
          <div class="btn-row">
            <button class="ghost tiny" id="prevBtn" ${state.currentIndex === 0 ? 'disabled' : ''}>Geri</button>
            ${state.currentIndex < total - 1 ? '<button class="ghost tiny" id="nextBtn">Növbəti</button>' : ''}
            <button class="primary tiny" id="finishBtn">Sınağı bitir</button>
          </div>
          <div class="jump-box">
            <input id="jumpInput" type="number" min="1" max="${total}" placeholder="Sual №">
            <button class="ghost tiny" id="jumpBtn">Keç</button>
          </div>
        </div>
      `;

      els.quizCard.querySelectorAll('[data-opt]').forEach(btn => {
        btn.addEventListener('click', () => {
          const qIndex = parseInt(btn.getAttribute('data-q'), 10);
          const opt = btn.getAttribute('data-opt');
          answerQuestion(qIndex, decodeAttr(opt));
        });
      });

      document.getElementById('saveBtn').onclick = () => toggleSavedQuestion(q.num);
      document.getElementById('revealBtn').onclick = () => toggleReveal(q.num);
      document.getElementById('prevBtn').onclick = () => {
        if (state.currentIndex > 0) {
          state.currentIndex--;
          renderQuiz();
        }
      };
      const nextBtn = document.getElementById('nextBtn');
      if (nextBtn) {
        nextBtn.onclick = () => {
          if (state.currentIndex < total - 1) {
            state.currentIndex++;
            renderQuiz();
          }
        };
      }
      const jumpBtn = document.getElementById('jumpBtn');
      const jumpInput = document.getElementById('jumpInput');
      if (jumpBtn && jumpInput) {
        const doJump = () => {
          const raw = parseInt(jumpInput.value, 10);
          if (!Number.isFinite(raw)) return;
          const target = clamp(raw, 1, total) - 1;
          state.currentIndex = target;
          renderQuiz();
        };
        jumpBtn.onclick = doJump;
        jumpInput.onkeydown = (e) => {
          if (e.key === 'Enter') {
            e.preventDefault();
            e.stopPropagation();
            doJump();
          }
        };
      }
      document.getElementById('finishBtn').onclick = finishQuiz;
    }

    function renderResults() {
      const s = scoreSummary();
      els.resultsCard.innerHTML = `
        <div class="result-grid">
          <div class="card result-card">
            <div class="label">Düzgün</div>
            <div class="value">${s.correct}</div>
          </div>
          <div class="card result-card">
            <div class="label">Səhv</div>
            <div class="value">${s.wrong}</div>
          </div>
          <div class="card result-card">
            <div class="label">Boş</div>
            <div class="value">${s.blank}</div>
          </div>
          <div class="card result-card">
            <div class="label">Faiz</div>
            <div class="value">${s.total ? Math.round((s.correct / s.total) * 100) : 0}%</div>
          </div>
        </div>
        <div class="card question-item">
          <div class="btn-row" style="justify-content: space-between;">
            <div class="badge good">Nəticə hazırdır</div>
            <div class="btn-row">
              <button class="ghost tiny" id="reviewToggleBtn">${state.onlyReviewWrong ? 'Hamısını göstər' : 'Yalnız səhvləri göstər'}</button>
              ${s.wrong > 0 ? `<button class="ghost tiny wrong-quiz-btn" id="wrongQuizBtn">🔁 Səhvləri sına (${s.wrong})</button>` : ''}
              <button class="primary tiny" id="restartBtn">Yeni sınaq</button>
            </div>
          </div>
          <div class="divider"></div>
          <div class="review-grid" id="reviewList"></div>
        </div>
      `;

      document.getElementById('restartBtn').onclick = () => {
        state.mode = 'setup';
        render();
      };
      document.getElementById('reviewToggleBtn').onclick = () => {
        state.onlyReviewWrong = !state.onlyReviewWrong;
        renderResults();
      };
      const wrongQuizBtn = document.getElementById('wrongQuizBtn');
      if (wrongQuizBtn) {
        wrongQuizBtn.onclick = () => buildQuizFromWrong();
      }

      const reviewList = document.getElementById('reviewList');
      const items = state.quiz.filter(q => {
        if (!state.onlyReviewWrong) return true;
        return q.selected !== q.correct;
      });

      if (!items.length) {
        reviewList.innerHTML = `<div class="mini">Bütün suallar doğrudur. Əla!</div>`;
        return;
      }

      reviewList.innerHTML = items.map((q) => {
        const isCorrect = q.selected === q.correct;
        return `
          <div class="card question-item">
            <div class="question-meta">
              <div>Sual #${q.num}</div>
              <div class="badge ${isCorrect ? 'good' : 'bad'}">${isCorrect ? 'Düzgün' : 'Səhv'}</div>
            </div>
            <h3>${escapeHtml(q.question)}</h3>
            <div class="mini">Sənin cavabın: <strong>${q.selected ? escapeHtml(q.selected) : 'Cavablanmayıb'}</strong></div>
            <div class="mini">Düzgün cavab: <strong>${escapeHtml(q.correct)}</strong></div>
            <div class="divider"></div>
            <div class="options">
              ${q.options.map((opt, optIdx) => {
                const classes = ['option'];
                if (opt.correct) classes.push('correct');
                if (q.selected === opt.text && !opt.correct) classes.push('wrong');
                if (q.selected === opt.text) classes.push('selected');
                return `
                  <div class="${classes.join(' ')}">
                    ${letter(optIdx)}) ${escapeHtml(opt.text)}
                  </div>
                `;
              }).join('')}
            </div>
          </div>
        `;
      }).join('');
    }

    function buildQuizFromWrong() {
      const wrongQuestions = state.quiz.filter(q => q.selected !== q.correct);
      if (!wrongQuestions.length) {
        els.statusLine.textContent = 'Səhv sual yoxdur!';
        return;
      }
      // Find original QUESTION_BANK entries for the wrong questions
      const wrongNums = new Set(wrongQuestions.map(q => q.num));
      const subset = QUESTION_BANK.filter(q => wrongNums.has(q.num));

      state.quiz = subset.map((q) => {
        const shuffledOptions = shuffle(q.options.map((text, i) => ({ text, sourceIndex: i })));
        const options = shuffledOptions.map((opt) => ({
          text: opt.text,
          correct: opt.text === q.correct
        }));
        return {
          num: q.num,
          question: q.question,
          options,
          correct: q.correct,
          selected: null
        };
      });

      state.currentIndex = 0;
      state.revealMap = new Set();
      state.mode = 'quiz';
      state.onlyReviewWrong = false;
      state.quizSource = 'wrong';
      render();
      els.statusLine.textContent = `Səhv suallardan ${subset.length} sual seçildi. Yeni sınaq başladı!`;
    }

    function renderSavedPanel() {
      const savedNums = [...state.savedQuestionNums]
        .filter(n => QUESTION_BANK.some(q => q.num === n))
        .sort((a, b) => a - b);
      const items = savedNums.map(num => QUESTION_BANK.find(q => q.num === num)).filter(Boolean);
      const openClass = state.savedPanelOpen ? 'open' : 'closed';
      const chevron = state.savedPanelOpen ? '⌃' : '⌄';

      els.savedPanel.innerHTML = `
        <button type="button" class="saved-panel-toggle" id="savedPanelToggle" aria-expanded="${state.savedPanelOpen ? 'true' : 'false'}">
          <div class="saved-panel-head">
            <div>
              <div class="saved-panel-title">Yadda saxlanılan suallar (${items.length})</div>
              <div class="saved-panel-sub">Sualı saxlamaq və silmək lokal yaddaşda qalır.</div>
            </div>
          </div>
          <div class="saved-chevron" aria-hidden="true">${chevron}</div>
        </button>
        <div class="saved-panel-body ${state.savedPanelOpen ? '' : 'hidden'}">
          <div class="btn-row">
            <button class="ghost tiny" id="savedQuizBtn2" ${items.length ? '' : 'disabled'}>Saxlanılanlarla sınaq</button>
            <button class="ghost tiny" id="clearSavedBtn" ${items.length ? '' : 'disabled'}>Hamısını təmizlə</button>
          </div>
          ${items.length ? '' : '<div class="saved-empty">Hələ heç nə saxlanmayıb. Sınaqdakı sualda “Yadda saxla” düyməsinə bas.</div>'}
          ${items.length ? `<div class="saved-list">${items.map((q) => `
            <div class="saved-item">
              <div>
                <strong>Sual #${q.num}</strong>
                <div class="mini">${escapeHtml(q.question)}</div>
              </div>
              <button class="ghost saved-remove" type="button" data-remove-saved="${q.num}">Sil</button>
            </div>
          `).join('')}</div>` : ''}
        </div>
      `;

      const savedPanelToggle = document.getElementById('savedPanelToggle');
      if (savedPanelToggle) {
        savedPanelToggle.onclick = () => {
          state.savedPanelOpen = !state.savedPanelOpen;
          renderSavedPanel();
        };
      }

      const savedQuizBtn2 = document.getElementById('savedQuizBtn2');
      if (savedQuizBtn2) {
        savedQuizBtn2.onclick = () => {
          state.quizSource = 'saved';
          buildQuiz('saved');
        };
      }

      const clearSavedBtn = document.getElementById('clearSavedBtn');
      if (clearSavedBtn) clearSavedBtn.onclick = clearSavedQuestions;

      els.savedPanel.querySelectorAll('[data-remove-saved]').forEach(btn => {
        btn.addEventListener('click', (e) => {
          e.stopPropagation();
          const num = parseInt(btn.getAttribute('data-remove-saved'), 10);
          removeSavedQuestion(num);
        });
      });
    }


    function letter(i) {
      return String.fromCharCode(65 + i);
    }

    function escapeHtml(s) {
      return String(s)
        .replaceAll('&', '&amp;')
        .replaceAll('<', '&lt;')
        .replaceAll('>', '&gt;')
        .replaceAll('"', '&quot;')
        .replaceAll("'", '&#39;');
    }

    function escapeAttr(s) {
      return String(s)
        .replaceAll('&', '&amp;')
        .replaceAll('<', '&lt;')
        .replaceAll('>', '&gt;')
        .replaceAll('"', '&quot;');
    }

    function decodeAttr(s) {
      const textarea = document.createElement('textarea');
      textarea.innerHTML = s;
      return textarea.value;
    }

    function renderSetup() {
      const customRaw = els.customRanges?.value.trim();
      if (customRaw) {
        const numbers = parseCustomSelection(customRaw);
        els.rangeLabel.textContent = `İnterval: ${customRaw}`;
        els.quizCount.textContent = String(Math.min(50, numbers.length));
        return;
      }

      els.rangeLabel.textContent = 'Hamısı';
      els.quizCount.textContent = String(Math.min(50, QUESTION_BANK.length));
    }

    els.startBtn.addEventListener('click', () => buildQuiz('range'));
    els.customRanges?.addEventListener('input', renderSetup);
    els.savedQuizBtn.addEventListener('click', () => {
      state.quizSource = 'saved';
      buildQuiz('saved');
    });
    if (els.themeToggleBtn) {
      els.themeToggleBtn.addEventListener('click', () => {
        state.theme = state.theme === 'dark' ? 'light' : 'dark';
        applyTheme();
      });
    }
    els.resetBtn.addEventListener('click', () => {
      els.customRanges.value = '';
      state.mode = 'setup';
      state.quiz = [];
      state.revealMap = new Set();
      state.onlyReviewWrong = false;
      state.quizSource = 'range';
      renderSetup();
      renderSavedPanel();
      render();
      els.statusLine.textContent = 'Hazırdır.';
    });
    els.customRanges.addEventListener('input', renderSetup);

    // Keyboard shortcuts: A/B/C/D/E → select option, Enter → next question
    document.addEventListener('keydown', (e) => {
      if (state.mode !== 'quiz') return;
      // Ignore if focus is on an input
      const tag = document.activeElement && document.activeElement.tagName;
      if (tag === 'INPUT' || tag === 'TEXTAREA') return;

      const q = currentQuestion();
      if (!q) return;

      const key = e.key.toUpperCase();

      // A-E → select corresponding option
      const letterMap = { A: 0, B: 1, C: 2, D: 3, E: 4 };
      if (key in letterMap) {
        const idx = letterMap[key];
        if (idx < q.options.length) {
          e.preventDefault();
          answerQuestion(state.currentIndex, q.options[idx].text);
        }
        return;
      }

      // Enter / ArrowRight → next question (or finish)
      if (e.key === 'Enter' || e.key === 'ArrowRight') {
        e.preventDefault();
        const total = state.quiz.length;
        if (state.currentIndex < total - 1) {
          state.currentIndex++;
          renderQuiz();
        } else {
          finishQuiz(true);
        }
        return;
      }

      // ArrowLeft / Backspace → previous question
      if (e.key === 'ArrowLeft' || e.key === 'Backspace') {
        e.preventDefault();
        if (state.currentIndex > 0) {
          state.currentIndex--;
          renderQuiz();
        }
      }
    });

    applyTheme();
    renderSetup();
    renderSavedPanel();
    render();
  </script>


</body></html>
