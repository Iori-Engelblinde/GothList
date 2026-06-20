<!DOCTYPE html>
<html lang="pt-BR" data-theme="kaneki">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Arquivo de Leitura</title>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=DM+Mono:wght@300;400;500&family=Cormorant:wght@700;800&display=swap" rel="stylesheet">

  <style>
    /* ══════════════════════════════════════════
       TEMA KANEKI — escuro / manchas de sangue
    ══════════════════════════════════════════ */
    [data-theme="kaneki"] {
      --black:      #080808;
      --deep:       #0e0e0e;
      --surface:    #141414;
      --raised:     #1a1a1a;
      --border:     #242424;
      --border-hi:  #2e2e2e;
      --muted:      #4a4a4a;
      --dim:        #6a6a6a;
      --text:       #c8c8c8;
      --bright:     #e8e8e8;
      --white:      #f0f0f0;

      --accent:     #8b0000;
      --accent-hi:  #a80000;
      --accent-glow:rgba(139,0,0,0.18);
      --accent-dim: #5a0000;

      --ok:         #2e6e4e;
      --ok-text:    #6fcf97;

      --body-bg:    #080808;
      --scrollbar-track: #080808;

      /* stain palette — vermelhos/bordô escuros */
      --stain-1: rgba(100,0,0,0.13);
      --stain-2: rgba(139,0,0,0.09);
      --stain-3: rgba(80,0,0,0.17);
      --stain-4: rgba(120,10,10,0.07);
    }

    /* ══════════════════════════════════════════
       TEMA SASAKI — claro / manchas de café
    ══════════════════════════════════════════ */
    [data-theme="sasaki"] {
      --black:      #eceef0;
      --deep:       #e4e7ea;
      --surface:    #f2f4f6;
      --raised:     #ffffff;
      --border:     #cdd2d8;
      --border-hi:  #b8bfc8;
      --muted:      #9aa4b0;
      --dim:        #6e7a88;
      --text:       #2c3440;
      --bright:     #141c28;
      --white:      #0a1018;

      --accent:     #8b0000;
      --accent-hi:  #a80000;
      --accent-glow:rgba(139,0,0,0.12);
      --accent-dim: #5a0000;

      --ok:         #1e5c3c;
      --ok-text:    #1a5a36;

      --body-bg:    #e8ebee;
      --scrollbar-track: #dde0e4;

      /* stain palette — azul-cinza de impressão */
      --stain-1: rgba(60,75,100,0.10);
      --stain-2: rgba(50,65,90,0.07);
      --stain-3: rgba(40,55,80,0.13);
      --stain-4: rgba(70,85,110,0.06);
    }

    /* ══════════════════════════════════════════
       BASE
    ══════════════════════════════════════════ */
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; }

    :root {
      --font-display: 'Cormorant Garamond', Georgia, serif;
      --font-title:   'Cormorant', Georgia, serif;
      --font-mono:    'DM Mono', 'Courier New', monospace;
      --transition:   0.35s cubic-bezier(0.4,0,0.2,1);
    }

    body {
      min-height: 100vh;
      background-color: var(--body-bg);
      color: var(--text);
      font-family: var(--font-display);
      font-size: 16px;
      line-height: 1.6;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 0 0 100px;
      transition:
        background-color var(--transition),
        color var(--transition);
      position: relative;
      overflow-x: hidden;
    }

    /* ── STAINS CANVAS ───────────────────────── */
    #stains-canvas {
      position: fixed;
      inset: 0;
      pointer-events: none;
      z-index: 0;
      opacity: 1;
      transition: opacity 0.4s;
    }

    /* everything above stains */
    body > *:not(#stains-canvas):not(#theme-btn) {
      position: relative;
      z-index: 1;
    }

    /* ── HEADER ──────────────────────────────── */
    .site-header {
      width: 100%;
      max-width: 760px;
      padding: 48px 24px 0;
      display: flex;
      flex-direction: column;
      gap: 2px;
    }

    .header-eyebrow {
      font-family: var(--font-mono);
      font-size: 0.68rem;
      letter-spacing: 0.22em;
      text-transform: uppercase;
      color: var(--accent-hi);
      display: flex;
      align-items: center;
      gap: 10px;
      transition: color var(--transition);
    }
    .header-eyebrow::before {
      content: '';
      display: inline-block;
      width: 22px; height: 1px;
      background: var(--accent);
      transition: background var(--transition);
    }

    .site-title {
      font-family: var(--font-title);
      font-size: clamp(2rem, 5vw, 3.2rem);
      font-weight: 800;
      color: var(--white);
      letter-spacing: 0.01em;
      line-height: 1.05;
      transition: color var(--transition);
    }

    .site-subtitle {
      font-family: var(--font-display);
      font-style: italic;
      font-size: 0.95rem;
      color: var(--dim);
      margin-top: 4px;
      transition: color var(--transition);
    }

    .header-rule {
      width: 100%; max-width: 760px;
      padding: 0 24px; margin-top: 20px;
    }
    .header-rule::after {
      content: '';
      display: block; height: 1px;
      background: linear-gradient(90deg, var(--accent) 0%, var(--accent-dim) 40%, transparent 100%);
      transition: background var(--transition);
    }

    /* ── TABS ────────────────────────────────── */
    .tab-bar {
      width: 100%; max-width: 760px;
      padding: 0 24px;
      display: flex; gap: 0;
      margin-top: 28px;
      border-bottom: 1px solid var(--border);
      transition: border-color var(--transition);
    }

    .tab-btn {
      font-family: var(--font-mono);
      font-size: 0.72rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--muted);
      padding: 10px 20px;
      background: none; border: none;
      border-bottom: 2px solid transparent;
      cursor: pointer;
      transition: color var(--transition), border-color var(--transition);
      margin-bottom: -1px;
    }
    .tab-btn:hover { color: var(--dim); }
    .tab-btn.active { color: var(--bright); border-bottom-color: var(--accent); }

    .tab-count {
      display: inline-flex; align-items: center; justify-content: center;
      min-width: 18px; height: 18px;
      background: var(--accent); color: #fff;
      border-radius: 3px; font-size: 0.6rem; padding: 0 4px;
      margin-left: 7px; opacity: 0;
      transition: opacity 0.2s, background var(--transition);
    }
    .tab-count.visible { opacity: 1; }

    /* ── PANELS ──────────────────────────────── */
    .panel { width: 100%; max-width: 760px; padding: 28px 24px 0; display: none; }
    .panel.active { display: block; animation: fadeUp 0.25s ease; }

    /* ── FORM CARD ───────────────────────────── */
    .form-card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: 4px; padding: 24px;
      position: relative;
      transition: background var(--transition), border-color var(--transition);
    }
    .form-card::before {
      content: '';
      position: absolute; top: 0; left: 0;
      width: 32px; height: 32px;
      border-top: 2px solid var(--accent);
      border-left: 2px solid var(--accent);
      border-radius: 4px 0 0 0;
      transition: border-color var(--transition);
    }

    .form-section-label {
      font-family: var(--font-mono);
      font-size: 0.6rem; letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--accent-hi);
      margin-bottom: 16px; padding-bottom: 8px;
      border-bottom: 1px solid var(--border);
      transition: color var(--transition), border-color var(--transition);
    }

    .grid { display: grid; gap: 16px; grid-template-columns: 1fr; }
    @media (min-width: 600px) { .grid { grid-template-columns: 1.3fr 0.85fr 0.85fr; } }

    .field { display: flex; flex-direction: column; gap: 6px; }

    label {
      font-family: var(--font-mono);
      font-size: 0.62rem; letter-spacing: 0.18em;
      text-transform: uppercase; color: var(--dim);
      transition: color var(--transition);
    }

    input[type="text"], input[type="number"], select {
      width: 100%; padding: 9px 12px;
      background: var(--deep);
      border: 1px solid var(--border);
      border-radius: 3px;
      color: var(--bright);
      font-family: var(--font-mono); font-size: 0.85rem;
      outline: none;
      transition: border-color 0.2s, box-shadow 0.2s,
                  background var(--transition), color var(--transition);
      appearance: none;
    }
    input:focus, select:focus {
      border-color: var(--accent);
      box-shadow: 0 0 0 2px var(--accent-glow);
    }
    input::placeholder { color: var(--muted); }

    select {
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='8' viewBox='0 0 12 8'%3E%3Cpath d='M1 1l5 5 5-5' stroke='%234a4a4a' stroke-width='1.5' fill='none' stroke-linecap='round'/%3E%3C/svg%3E");
      background-repeat: no-repeat;
      background-position: right 12px center;
      padding-right: 32px; cursor: pointer;
    }

    .number-input { display: flex; align-items: center; gap: 4px; }
    .number-input input { flex: 1; }

    .step-btn {
      width: 32px; height: 36px;
      background: var(--raised);
      border: 1px solid var(--border);
      border-radius: 3px;
      color: var(--dim); font-size: 1rem; cursor: pointer;
      display: flex; align-items: center; justify-content: center;
      flex-shrink: 0; font-family: var(--font-mono);
      transition: border-color 0.15s, color 0.15s,
                  background var(--transition);
    }
    .step-btn:hover { border-color: var(--accent); color: var(--accent-hi); }

    .status-row { margin-top: 16px; }

    /* ── BUTTONS ─────────────────────────────── */
    .btn-row { display: flex; gap: 10px; flex-wrap: wrap; margin-top: 20px; align-items: center; }

    .btn-primary {
      font-family: var(--font-mono); font-size: 0.7rem;
      letter-spacing: 0.15em; text-transform: uppercase;
      padding: 10px 22px;
      background: var(--accent); color: #f0e8e8;
      border: 1px solid var(--accent-hi); border-radius: 3px;
      cursor: pointer;
      transition: background 0.2s, box-shadow 0.2s;
    }
    .btn-primary:hover { background: var(--accent-hi); box-shadow: 0 0 16px var(--accent-glow); }

    .btn-ghost {
      font-family: var(--font-mono); font-size: 0.7rem;
      letter-spacing: 0.15em; text-transform: uppercase;
      padding: 10px 18px;
      background: transparent; color: var(--dim);
      border: 1px solid var(--border); border-radius: 3px;
      cursor: pointer;
      transition: color 0.2s, border-color 0.2s, background var(--transition);
    }
    .btn-ghost:hover { color: var(--text); border-color: var(--border-hi); }

    /* ── OUTPUT ──────────────────────────────── */
    .output {
      margin-top: 20px; padding: 18px 20px;
      background: var(--deep);
      border: 1px solid var(--border); border-radius: 3px;
      display: flex; flex-direction: column; gap: 12px;
      position: relative;
      transition: background var(--transition), border-color var(--transition);
    }
    .output::before {
      content: '';
      position: absolute; left: 0; top: 12px; bottom: 12px;
      width: 2px;
      background: linear-gradient(180deg, transparent, var(--accent), transparent);
      border-radius: 1px;
      transition: background var(--transition);
    }

    .percent-row { display: flex; align-items: baseline; gap: 14px; flex-wrap: wrap; }

    .percent-value {
      font-family: var(--font-title); font-size: 3rem; font-weight: 800;
      color: var(--white); line-height: 1; letter-spacing: -0.02em;
      transition: color var(--transition);
    }

    .percent-badge {
      font-family: var(--font-mono); font-size: 0.72rem;
      color: var(--dim); letter-spacing: 0.05em;
      transition: color var(--transition);
    }

    .progress-track {
      height: 3px; background: var(--raised);
      overflow: visible; position: relative;
      transition: background var(--transition);
    }
    .progress-fill {
      height: 100%; width: 0%;
      background: var(--accent);
      transition: width 0.4s cubic-bezier(0.25,0.46,0.45,0.94), background var(--transition);
      position: relative;
    }
    .progress-fill::after {
      content: ''; position: absolute;
      right: -1px; top: -2px; width: 3px; height: 7px;
      background: inherit; border-radius: 0 0 2px 2px; opacity: 0.8;
    }

    .output-meta { font-family: var(--font-mono); font-size: 0.72rem; color: var(--dim); letter-spacing: 0.04em; }
    .output-remaining { color: var(--accent-hi); }
    .output-complete  { color: var(--ok-text); }

    .msg { font-family: var(--font-mono); font-size: 0.68rem; letter-spacing: 0.06em; }
    .msg.error { color: var(--accent-hi); }
    .msg.fine  { color: var(--ok-text); }

    /* ── ARCHIVE ─────────────────────────────── */
    .archive-controls {
      display: flex; gap: 10px; flex-wrap: wrap;
      align-items: flex-end; margin-bottom: 18px;
    }
    .search-wrap { flex: 1; min-width: 180px; display: flex; flex-direction: column; gap: 6px; }
    .sort-group { display: flex; gap: 10px; flex-wrap: wrap; }
    .sort-group .field { min-width: 120px; }

    .archive-stats {
      display: flex; gap: 20px; flex-wrap: wrap;
      padding: 12px 16px;
      background: var(--surface); border: 1px solid var(--border); border-radius: 3px;
      margin-bottom: 16px;
      transition: background var(--transition), border-color var(--transition);
    }
    .stat-item { display: flex; flex-direction: column; gap: 2px; }
    .stat-label {
      font-family: var(--font-mono); font-size: 0.58rem;
      letter-spacing: 0.18em; text-transform: uppercase; color: var(--muted);
      transition: color var(--transition);
    }
    .stat-value {
      font-family: var(--font-title); font-size: 1.5rem; font-weight: 700;
      color: var(--white); line-height: 1;
      transition: color var(--transition);
    }
    .stat-value.blood { color: var(--accent-hi); }

    .saved-list-inner { display: flex; flex-direction: column; gap: 4px; }

    .saved-item {
      cursor: pointer; padding: 11px 14px;
      background: var(--surface); border: 1px solid var(--border); border-radius: 3px;
      display: flex; justify-content: space-between; align-items: center; gap: 12px;
      transition: background 0.15s, border-color 0.15s;
      position: relative; overflow: hidden;
      animation: fadeUp 0.2s ease both;
    }
    .saved-item::before {
      content: ''; position: absolute; left: 0; top: 0; bottom: 0; width: 2px;
      background: var(--border); transition: background 0.2s;
    }
    .saved-item:hover { background: var(--raised); }
    .saved-item:hover::before { background: var(--accent-dim); }
    .saved-item.active { border-color: var(--border-hi); background: var(--raised); }
    .saved-item.active::before { background: var(--accent); }

    .saved-left { display: flex; flex-direction: column; gap: 4px; min-width: 0; flex: 1; }
    .saved-name-row { display: flex; align-items: center; gap: 8px; flex-wrap: wrap; }
    .saved-name {
      font-family: var(--font-display); font-size: 0.97rem; color: var(--bright);
      white-space: nowrap; overflow: hidden; text-overflow: ellipsis; max-width: 300px;
      transition: color var(--transition);
    }

    .status-pill {
      font-family: var(--font-mono); font-size: 0.58rem;
      letter-spacing: 0.12em; text-transform: uppercase;
      padding: 2px 7px; border-radius: 2px;
      border: 1px solid var(--border); color: var(--muted); white-space: nowrap; flex-shrink: 0;
    }
    .status-pill.lendo     { border-color: #2a4a6a; color: #6aafd4; }
    .status-pill.completo  { border-color: #1e4a32; color: var(--ok-text); }
    .status-pill.hiato     { border-color: #4a3a10; color: #c4943a; }
    .status-pill.abandonado{ border-color: #3a1010; color: #a05050; }

    .saved-meta {
      font-family: var(--font-mono); font-size: 0.62rem; color: var(--muted);
      display: flex; gap: 10px; flex-wrap: wrap;
      transition: color var(--transition);
    }

    .mini-bar-wrap {
      width: 60px; height: 2px; background: var(--raised);
      flex-shrink: 0; position: relative; align-self: center;
      transition: background var(--transition);
    }
    .mini-bar { position: absolute; left: 0; top: 0; bottom: 0; background: var(--accent-dim); transition: width 0.3s; }
    .mini-bar.complete { background: var(--ok); }

    .saved-right { display: flex; align-items: center; gap: 10px; flex-shrink: 0; }
    .saved-pct { font-family: var(--font-mono); font-size: 0.75rem; color: var(--dim); min-width: 38px; text-align: right; }
    .saved-pct.complete { color: var(--ok-text); }

    .delete-btn {
      background: transparent; border: none; color: var(--muted);
      cursor: pointer; font-size: 0.85rem; padding: 4px; border-radius: 2px;
      line-height: 1; transition: color 0.15s, background 0.15s;
    }
    .delete-btn:hover { color: var(--accent-hi); background: var(--accent-glow); }

    .empty-state {
      text-align: center; padding: 40px 20px; color: var(--muted);
      font-family: var(--font-mono); font-size: 0.72rem; letter-spacing: 0.1em;
    }

    /* ── FOOTER ──────────────────────────────── */
    footer {
      width: 100%; max-width: 760px;
      padding: 28px 24px 0;
      font-family: var(--font-mono); font-size: 0.62rem;
      color: var(--muted); letter-spacing: 0.08em;
      display: flex; justify-content: space-between; flex-wrap: wrap; gap: 6px;
      border-top: 1px solid var(--border); margin-top: 36px;
      transition: border-color var(--transition), color var(--transition);
    }

    /* ── THEME PILL BUTTON ───────────────────── */
    #theme-btn {
      position: fixed;
      bottom: 28px; right: 28px;
      z-index: 9999;
      font-family: var(--font-mono);
      font-size: 0.65rem;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      padding: 9px 20px;
      border-radius: 999px;       /* pílula */
      border: 1px solid var(--border);
      background: var(--surface);
      color: var(--dim);
      cursor: pointer;
      display: flex; align-items: center; gap: 8px;
      box-shadow: 0 4px 20px rgba(0,0,0,0.3);
      transition:
        background var(--transition),
        border-color var(--transition),
        color var(--transition),
        box-shadow 0.2s;
    }
    #theme-btn:hover {
      border-color: var(--accent);
      color: var(--text);
      box-shadow: 0 4px 24px var(--accent-glow);
    }
    #theme-btn .pill-dot {
      width: 6px; height: 6px; border-radius: 50%;
      background: var(--accent);
      flex-shrink: 0;
      transition: background var(--transition);
    }

    /* ── ANIMATIONS ──────────────────────────── */
    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(10px); }
      to   { opacity: 1; transform: translateY(0); }
    }

    /* ── SCROLLBAR ───────────────────────────── */
    ::-webkit-scrollbar { width: 6px; }
    ::-webkit-scrollbar-track { background: var(--scrollbar-track); }
    ::-webkit-scrollbar-thumb { background: var(--border); border-radius: 3px; }
    ::-webkit-scrollbar-thumb:hover { background: var(--accent-dim); }
  </style>
</head>
<body>

  <!-- STAINS CANVAS (background texture) -->
  <canvas id="stains-canvas"></canvas>

  <!-- THEME PILL -->
  <button id="theme-btn" aria-label="Alternar tema">
    <span class="pill-dot"></span>
    <span id="theme-label">Kaneki</span>
  </button>

  <header class="site-header">
    <div class="header-eyebrow">Sistema de Catalogação Pessoal</div>
    <h1 class="site-title">Arquivo de Leitura</h1>
    <p class="site-subtitle">Registro e progresso de obras catalogadas</p>
  </header>

  <div class="header-rule"></div>

  <nav class="tab-bar" role="tablist">
    <button class="tab-btn active" role="tab" data-panel="catalogar" aria-selected="true">Catalogar</button>
    <button class="tab-btn" role="tab" data-panel="arquivos" aria-selected="false">
      Arquivos <span class="tab-count" id="tab-count">0</span>
    </button>
  </nav>

  <!-- PANEL: CATALOGAR -->
  <section class="panel active" id="panel-catalogar" role="tabpanel">
    <div class="form-card">
      <div class="form-section-label">Identificação da obra</div>
      <div class="grid">
        <div class="field">
          <label for="manga">Título</label>
          <input id="manga" type="text" placeholder="Ex.: Tokyo Ghoul" autocomplete="off" />
        </div>
        <div class="field">
          <label for="total">Total de capítulos</label>
          <div class="number-input">
            <button type="button" class="step-btn" data-target="total" data-step="-1">−</button>
            <input id="total" type="number" min="0" step="1" placeholder="000" />
            <button type="button" class="step-btn" data-target="total" data-step="1">+</button>
          </div>
        </div>
        <div class="field">
          <label for="lidos">Capítulos lidos</label>
          <div class="number-input">
            <button type="button" class="step-btn" data-target="lidos" data-step="-1">−</button>
            <input id="lidos" type="number" min="0" step="1" placeholder="000" />
            <button type="button" class="step-btn" data-target="lidos" data-step="1">+</button>
          </div>
        </div>
      </div>
      <div class="status-row">
        <div class="field">
          <label for="status">Status</label>
          <select id="status">
            <option value="">— Não definido —</option>
            <option value="lendo">Lendo</option>
            <option value="completo">Concluído</option>
            <option value="hiato">Em hiato</option>
            <option value="abandonado">Abandonado</option>
          </select>
        </div>
      </div>
    </div>

    <div class="btn-row">
      <button class="btn-primary" id="btnSalvar" type="button">Registrar</button>
      <button class="btn-ghost"   id="btnCalcular" type="button">Calcular</button>
      <button class="btn-ghost"   id="btnZerar" type="button">Limpar</button>
    </div>

    <div class="output">
      <div class="percent-row">
        <span class="percent-value" id="perc">0%</span>
        <span class="percent-badge" id="resumo">0 de 0 capítulos</span>
      </div>
      <div class="progress-track"><div class="progress-fill" id="bar"></div></div>
      <div id="remaining" class="output-meta"></div>
      <div id="msg" class="msg fine">Pronto.</div>
    </div>
  </section>

  <!-- PANEL: ARQUIVOS -->
  <section class="panel" id="panel-arquivos" role="tabpanel">
    <div class="archive-stats" id="archive-stats"></div>
    <div class="archive-controls">
      <div class="search-wrap">
        <label for="searchManga">Buscar</label>
        <input id="searchManga" type="text" placeholder="Filtrar título..." autocomplete="off" />
      </div>
      <div class="sort-group">
        <div class="field">
          <label for="sortBy">Ordenar</label>
          <select id="sortBy">
            <option value="titulo">Título</option>
            <option value="percent">Progresso</option>
            <option value="lidos">Capítulos lidos</option>
            <option value="atualizado">Atualizado</option>
          </select>
        </div>
        <div class="field">
          <label for="sortOrder">Ordem</label>
          <select id="sortOrder">
            <option value="asc">↑ Asc</option>
            <option value="desc">↓ Desc</option>
          </select>
        </div>
      </div>
    </div>
    <div class="saved-list-inner" id="listaSalvos"></div>
  </section>

  <footer>
    <span>Enter calcular · Shift+Enter registrar · Ctrl+S salvar</span>
    <span>Dados armazenados localmente</span>
  </footer>

  <script>
  // ════════════════════════════════════════════
  //  STAINS — manchas aleatórias no canvas
  // ════════════════════════════════════════════
  const canvas = document.getElementById('stains-canvas');
  const ctx    = canvas.getContext('2d');

  function resizeCanvas() {
    canvas.width  = window.innerWidth;
    canvas.height = Math.max(document.body.scrollHeight, window.innerHeight);
  }

  // Seeded random para padrão diferente a cada chamada
  function mulberry32(seed) {
    return function() {
      seed |= 0; seed = seed + 0x6D2B79F5 | 0;
      let t = Math.imul(seed ^ seed >>> 15, 1 | seed);
      t = t + Math.imul(t ^ t >>> 7, 61 | t) ^ t;
      return ((t ^ t >>> 14) >>> 0) / 4294967296;
    };
  }

  function drawStains(theme) {
    resizeCanvas();
    ctx.clearRect(0, 0, canvas.width, canvas.height);

    const seed = Math.floor(Math.random() * 0xffffffff);
    const rng  = mulberry32(seed);

    const isKaneki = theme === 'kaneki';

    // número de manchas — poucas, discretas
    const count = Math.floor(rng() * 6) + 5; // 5–10

    for (let i = 0; i < count; i++) {
      const x = rng() * canvas.width;
      const y = rng() * canvas.height;
      const type = rng(); // 0..1 decide o tipo de mancha

      ctx.save();
      ctx.translate(x, y);
      ctx.rotate(rng() * Math.PI * 2);

      if (isKaneki) {
        drawBloodStain(ctx, rng, type);
      } else {
        // Sasaki: mistura anéis de café + manchas de tinta
        if (type < 0.60) drawCoffeeStain(ctx, rng, type);
        else             drawInkStain(ctx, rng);
      }

      ctx.restore();
    }
  }

  // ── Mancha de sangue ──────────────────────
  function drawBloodStain(ctx, rng, type) {
    const baseAlpha = 0.22 + rng() * 0.18;

    // sempre: círculo distorcido como base
    const rx = 10 + rng() * 30;
    const ry = rx * (0.55 + rng() * 0.9);
    const grad = ctx.createRadialGradient(rng()*4-2, rng()*4-2, 0, 0, 0, Math.max(rx, ry) * 1.1);
    grad.addColorStop(0,    `rgba(185,15,15,${baseAlpha})`);
    grad.addColorStop(0.45, `rgba(160,5,5,${baseAlpha * 0.82})`);
    grad.addColorStop(0.78, `rgba(130,0,0,${baseAlpha * 0.38})`);
    grad.addColorStop(1,    `rgba(90,0,0,0)`);
    ctx.fillStyle = grad;

    // forma irregular via bezier em vez de ellipse perfeita
    ctx.beginPath();
    const pts = 6 + Math.floor(rng() * 4);
    for (let j = 0; j < pts; j++) {
      const angle = (j / pts) * Math.PI * 2;
      const jitter = 0.78 + rng() * 0.44;
      const px = Math.cos(angle) * rx * jitter;
      const py = Math.sin(angle) * ry * jitter;
      if (j === 0) ctx.moveTo(px, py);
      else {
        const prev = (j - 1) / pts * Math.PI * 2;
        const mx = Math.cos(prev + (angle-prev)*0.5) * rx * (0.7 + rng()*0.6);
        const my = Math.sin(prev + (angle-prev)*0.5) * ry * (0.7 + rng()*0.6);
        ctx.quadraticCurveTo(mx, my, px, py);
      }
    }
    ctx.closePath();
    ctx.fill();

    // micro-respingos ao redor — só pontinhos, sem rastros
    const n = Math.floor(rng() * 9) + 4;
    const spread = Math.max(rx, ry) * (0.9 + rng() * 1.1);
    for (let j = 0; j < n; j++) {
      const ang  = rng() * Math.PI * 2;
      const dist = spread * (0.6 + rng() * 0.7);
      const pr   = 0.5 + rng() * 2.2;
      const a    = baseAlpha * (0.25 + rng() * 0.45);
      ctx.fillStyle = `rgba(${170 + (rng()*20|0)},${rng()*10|0},${rng()*10|0},${a})`;
      ctx.beginPath();
      ctx.arc(Math.cos(ang) * dist, Math.sin(ang) * dist, pr, 0, Math.PI * 2);
      ctx.fill();
    }
  }

  // ── Mancha de café (anel pontilhado marrom) ──
  function drawCoffeeStain(ctx, rng, type) {
    const baseAlpha = 0.11 + rng() * 0.09;

    if (type < 0.60) {
      // anel de xícara — pontos marrons com tamanho bem variado
      const r    = 22 + rng() * 36;
      const ringW = 4 + rng() * 6;
      const dots  = Math.floor(r * 2.8 + rng() * r);

      for (let j = 0; j < dots; j++) {
        const angle = (j / dots) * Math.PI * 2 + (rng() - 0.5) * 0.22;
        const rVar  = r + (rng() - 0.5) * ringW * 1.6;
        const px    = Math.cos(angle) * rVar;
        const py    = Math.sin(angle) * rVar;

        // tamanho bem variado — o que pediu
        const dotR  = 0.4 + rng() * rng() * 4.5; // rng()*rng() favorece valores pequenos com exceções grandes
        const edgeF = Math.abs((rVar - r) / ringW);
        const alpha = baseAlpha * (1 - edgeF * 0.45) * (0.45 + rng() * 0.85);

        // tom marrom claro — sem componente azul
        const rv = 130 + (rng() * 50 | 0);
        const gv = 75  + (rng() * 35 | 0);
        const bv = 20  + (rng() * 20 | 0);
        ctx.fillStyle = `rgba(${rv},${gv},${bv},${alpha})`;
        ctx.beginPath();
        ctx.arc(px, py, dotR, 0, Math.PI * 2);
        ctx.fill();
      }

      // acúmulo interno leve
      if (rng() > 0.3) {
        const innerR = r * (0.45 + rng() * 0.35);
        const iDots  = Math.floor(innerR * 1.4);
        for (let j = 0; j < iDots; j++) {
          const ang  = rng() * Math.PI * 2;
          const dist = rng() * innerR;
          const rv   = 120 + (rng()*40|0);
          const gv   = 65  + (rng()*30|0);
          ctx.fillStyle = `rgba(${rv},${gv},15,${baseAlpha * 0.22 * rng()})`;
          ctx.beginPath();
          ctx.arc(Math.cos(ang)*dist, Math.sin(ang)*dist, 0.4+rng()*1.4, 0, Math.PI*2);
          ctx.fill();
        }
      }

      // segundo anel incompleto
      if (rng() > 0.45) {
        const r2   = r + ringW + rng() * 6;
        const d2   = Math.floor(r2 * 1.5);
        for (let j = 0; j < d2; j++) {
          if (rng() > 0.48) continue;
          const ang  = (j / d2) * Math.PI * 2 + (rng()-0.5)*0.25;
          const rV2  = r2 + (rng()-0.5)*3;
          const rv   = 115 + (rng()*40|0);
          const gv   = 60  + (rng()*30|0);
          ctx.fillStyle = `rgba(${rv},${gv},15,${baseAlpha * 0.3 * rng()})`;
          ctx.beginPath();
          ctx.arc(Math.cos(ang)*rV2, Math.sin(ang)*rV2, 0.4+rng()*1.8, 0, Math.PI*2);
          ctx.fill();
        }
      }

    } else {
      // respingos de café — pontinhos marrons dispersos
      const n = Math.floor(rng() * 8) + 3;
      const sp = 16 + rng() * 26;
      for (let j = 0; j < n; j++) {
        const r  = 0.8 + rng() * rng() * 4;
        const ox = (rng() - 0.5) * sp * 2;
        const oy = (rng() - 0.5) * sp;
        const rv = 125 + (rng()*45|0);
        const gv = 70  + (rng()*30|0);
        ctx.fillStyle = `rgba(${rv},${gv},18,${baseAlpha * (0.5 + rng()*0.7)})`;
        ctx.beginPath();
        ctx.arc(ox, oy, r, 0, Math.PI * 2);
        ctx.fill();
      }
    }
  }

  // ── Mancha de tinta (impressão) ───────────
  function drawInkStain(ctx, rng) {
    const baseAlpha = 0.10 + rng() * 0.09;
    const size = 12 + rng() * 28;
    const n    = Math.floor(size * 3.5 + rng() * size * 2);

    // forma irregular: raios distintos por setor angular
    const sectors = 7 + Math.floor(rng() * 5);
    const radii   = Array.from({length: sectors}, () => size * (0.5 + rng() * 0.7));

    function getRadius(angle) {
      const norm  = ((angle % (Math.PI*2)) + Math.PI*2) % (Math.PI*2);
      const idx   = norm / (Math.PI*2) * sectors;
      const lo    = Math.floor(idx) % sectors;
      const hi    = (lo + 1) % sectors;
      const t     = idx - Math.floor(idx);
      return radii[lo] * (1-t) + radii[hi] * t;
    }

    for (let j = 0; j < n; j++) {
      const ang   = rng() * Math.PI * 2;
      const maxR  = getRadius(ang);
      const dist  = Math.pow(rng(), 0.6) * maxR;
      const pr    = 0.3 + rng() * 1.6;
      const edge  = dist / maxR; // 0=centro 1=borda
      const alpha = baseAlpha * (1 - edge * 0.5) * (0.35 + rng() * 0.75);

      // cinza-azulado frio — sem marrom
      const rv = 55 + (rng()*25|0);
      const gv = 65 + (rng()*28|0);
      const bv = 90 + (rng()*35|0);
      ctx.fillStyle = `rgba(${rv},${gv},${bv},${alpha})`;
      ctx.beginPath();
      ctx.arc(Math.cos(ang)*dist, Math.sin(ang)*dist, pr, 0, Math.PI*2);
      ctx.fill();
    }

    // borda irregular mais escura
    const edgeDots = Math.floor(n * 0.35);
    for (let j = 0; j < edgeDots; j++) {
      const ang  = rng() * Math.PI * 2;
      const maxR = getRadius(ang);
      const dist = maxR * (0.75 + rng() * 0.35);
      const pr   = 0.3 + rng() * 1.1;
      ctx.fillStyle = `rgba(45,55,82,${baseAlpha * (0.3 + rng()*0.5)})`;
      ctx.beginPath();
      ctx.arc(Math.cos(ang)*dist, Math.sin(ang)*dist, pr, 0, Math.PI*2);
      ctx.fill();
    }
  }

  // ════════════════════════════════════════════
  //  TEMA TOGGLE
  // ════════════════════════════════════════════
  let currentTheme = localStorage.getItem('manga-theme') || 'kaneki';

  function applyTheme(theme, redrawStains = true) {
    document.documentElement.setAttribute('data-theme', theme);
    document.getElementById('theme-label').textContent =
      theme === 'kaneki' ? 'Kaneki' : 'Sasaki';
    localStorage.setItem('manga-theme', theme);
    currentTheme = theme;
    if (redrawStains) drawStains(theme);
  }

  document.getElementById('theme-btn').addEventListener('click', () => {
    const next = currentTheme === 'kaneki' ? 'sasaki' : 'kaneki';
    applyTheme(next, true);
  });

  // aplica tema salvo sem redesenhar ainda
  applyTheme(currentTheme, false);

  // desenha manchas após layout estar pronto
  window.addEventListener('load', () => drawStains(currentTheme));
  window.addEventListener('resize', () => drawStains(currentTheme));

  // ════════════════════════════════════════════
  //  APP LOGIC
  // ════════════════════════════════════════════
  const elId = id => document.getElementById(id);

  const manga      = elId('manga');
  const total      = elId('total');
  const lidos      = elId('lidos');
  const statusSel  = elId('status');
  const perc       = elId('perc');
  const bar        = elId('bar');
  const resumo     = elId('resumo');
  const remaining  = elId('remaining');
  const msg        = elId('msg');
  const lista      = elId('listaSalvos');
  const sortBy     = elId('sortBy');
  const sortOrder  = elId('sortOrder');
  const searchManga= elId('searchManga');

  let activeKey = null;

  // ── Tabs ────────────────────────────────────
  document.querySelectorAll('.tab-btn').forEach(btn => {
    btn.addEventListener('click', () => {
      document.querySelectorAll('.tab-btn').forEach(b => {
        b.classList.remove('active'); b.setAttribute('aria-selected','false');
      });
      document.querySelectorAll('.panel').forEach(p => p.classList.remove('active'));
      btn.classList.add('active'); btn.setAttribute('aria-selected','true');
      const panel = elId('panel-' + btn.dataset.panel);
      if (panel) panel.classList.add('active');
      if (btn.dataset.panel === 'arquivos') renderSaved();
    });
  });

  // ── Utils ────────────────────────────────────
  function makeKey(name) { return 'manga:' + name.trim().toLowerCase(); }

  const STATUS_LABELS = { lendo:'Lendo', completo:'Concluído', hiato:'Em hiato', abandonado:'Abandonado' };

  function formatDate(iso) {
    if (!iso) return null;
    try {
      const diff = Math.floor((Date.now() - new Date(iso)) / 60000);
      if (diff < 1)   return 'agora mesmo';
      if (diff < 60)  return `${diff}min atrás`;
      const h = Math.floor(diff / 60);
      if (h < 24)     return `${h}h atrás`;
      const d = Math.floor(h / 24);
      if (d === 1)    return 'ontem';
      if (d < 30)     return `${d}d atrás`;
      return new Date(iso).toLocaleDateString('pt-BR');
    } catch { return null; }
  }

  function escapeHtml(str) {
    return str.replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;').replace(/"/g,'&quot;');
  }

  // ── Calc ─────────────────────────────────────
  function calc() {
    const name = manga.value.trim();
    const t = Number(total.value);
    const r = Number(lidos.value);

    remaining.textContent = '';

    if (!name) { msg.textContent = 'Informe o título da obra.'; msg.className = 'msg error'; }
    else        { msg.textContent = 'Pronto.';                  msg.className = 'msg fine';  }

    if (!Number.isFinite(t) || !Number.isFinite(r)) return;

    if (t < 0 || r < 0) {
      perc.textContent = '—'; resumo.textContent = 'valores inválidos';
      msg.textContent = 'Use apenas inteiros não negativos.'; msg.className = 'msg error';
      bar.style.width = '0%'; return;
    }

    if (t === 0) {
      perc.textContent = '0%'; resumo.textContent = `${r} de 0 capítulos`;
      msg.textContent = 'Defina o total de capítulos.'; msg.className = 'msg error';
      bar.style.width = '0%'; return;
    }

    const safeRead = Math.max(0, Math.min(r, t));
    if (r > t) lidos.value = String(safeRead);

    const pFloat = Math.round((safeRead / t) * 10000) / 100;
    const pInt   = Math.round((safeRead / t) * 100);

    perc.textContent  = `${pFloat}%`;
    resumo.textContent = `${safeRead} de ${t} capítulos${name ? ' — ' + name : ''}`;
    bar.style.width   = `${Math.min(100, pFloat)}%`;
    bar.style.background = pInt === 100 ? 'var(--ok)' : 'var(--accent)';
    perc.setAttribute('data-percent-int', String(pInt));

    const rest = t - safeRead;
    if (rest > 0) { remaining.textContent = `Faltam ${rest} capítulo${rest !== 1 ? 's' : ''}.`; remaining.className = 'output-meta output-remaining'; }
    else          { remaining.textContent = 'Obra concluída.'; remaining.className = 'output-meta output-complete'; }
  }

  // ── Save ─────────────────────────────────────
  function save() {
    const nameRaw = manga.value.trim();
    if (!nameRaw) { msg.textContent = 'Informe o título antes de registrar.'; msg.className = 'msg error'; return; }

    const key = makeKey(nameRaw);
    const t   = Number(total.value) || 0;
    const r   = Math.max(0, Math.min(Number(lidos.value) || 0, t));
    const isUpdate = !!localStorage.getItem(key);

    localStorage.setItem(key, JSON.stringify({
      displayName: nameRaw, total: t, lidos: r,
      status: statusSel.value, updatedAt: new Date().toISOString(),
    }));

    msg.textContent = isUpdate ? `"${nameRaw}" — registro atualizado.` : `"${nameRaw}" — catalogado.`;
    msg.className = 'msg fine';
    activeKey = key;
    updateTabCount();
    renderSaved();
  }

  // ── Load for name ─────────────────────────────
  function loadForName(inputName) {
    if (!inputName) return;
    const key = makeKey(inputName);
    let raw = localStorage.getItem(key);
    if (!raw) {
      const found = Object.keys(localStorage).filter(k => k.startsWith('manga:'))
        .find(k => k.replace('manga:','') === inputName.trim().toLowerCase());
      if (found) raw = localStorage.getItem(found);
    }
    if (raw) {
      try {
        const d = JSON.parse(raw);
        if (typeof d.total === 'number') total.value = String(d.total);
        if (typeof d.lidos === 'number') lidos.value = String(d.lidos);
        if (d.displayName)               manga.value = d.displayName;
        if (d.status !== undefined)       statusSel.value = d.status;
        activeKey = makeKey(d.displayName || inputName);
      } catch {}
    }
    calc(); renderSaved();
  }

  // ── Stats ─────────────────────────────────────
  function renderStats(items) {
    const concluidos = items.filter(i => i.percent === 100).length;
    const lendoN     = items.filter(i => i.status === 'lendo').length;
    const totalCap   = items.reduce((s, i) => s + i.lidos, 0);
    elId('archive-stats').innerHTML = `
      <div class="stat-item"><span class="stat-label">Catalogados</span><span class="stat-value">${items.length}</span></div>
      <div class="stat-item"><span class="stat-label">Concluídos</span><span class="stat-value blood">${concluidos}</span></div>
      <div class="stat-item"><span class="stat-label">Em leitura</span><span class="stat-value">${lendoN}</span></div>
      <div class="stat-item"><span class="stat-label">Cap. lidos</span><span class="stat-value">${totalCap.toLocaleString('pt-BR')}</span></div>
    `;
  }

  // ── Render saved ──────────────────────────────
  function renderSaved() {
    lista.innerHTML = '';
    const query = searchManga.value.trim().toLowerCase();
    const keys  = Object.keys(localStorage).filter(k => k.startsWith('manga:'));

    if (keys.length === 0) {
      lista.innerHTML = '<div class="empty-state">Nenhuma obra catalogada.</div>';
      renderStats([]); return;
    }

    let items = keys.map(k => {
      let d; try { d = JSON.parse(localStorage.getItem(k)); } catch { d = {}; }
      const display  = d?.displayName || k.replace('manga:','');
      const safeRead = typeof d?.lidos === 'number' ? d.lidos : 0;
      const t        = typeof d?.total === 'number'  ? d.total  : 0;
      const percent  = t > 0 ? Math.round((safeRead / t) * 100) : 0;
      return { key: k, name: display, lidos: safeRead, total: t, percent,
               status: d?.status || '', updatedAt: d?.updatedAt || null };
    });

    renderStats(items);
    if (query) items = items.filter(it => it.name.toLowerCase().includes(query));
    if (items.length === 0) { lista.innerHTML = '<div class="empty-state">Nenhum resultado.</div>'; return; }

    const by = sortBy.value, order = sortOrder.value;
    items.sort((a,b) => {
      let c = 0;
      if (by==='titulo')     c = a.name.localeCompare(b.name, undefined, {sensitivity:'base'});
      if (by==='percent')    c = a.percent - b.percent;
      if (by==='lidos')      c = a.lidos - b.lidos;
      if (by==='atualizado') c = (a.updatedAt||'').localeCompare(b.updatedAt||'');
      return order==='asc' ? c : -c;
    });

    items.forEach((it, idx) => {
      const isComplete = it.percent === 100;
      const div = document.createElement('div');
      div.className = 'saved-item' + (it.key === activeKey ? ' active' : '');
      div.style.animationDelay = `${idx * 28}ms`;
      div.innerHTML = `
        <div class="saved-left">
          <div class="saved-name-row">
            <span class="saved-name">${escapeHtml(it.name)}</span>
            ${it.status ? `<span class="status-pill ${it.status}">${STATUS_LABELS[it.status]||it.status}</span>` : ''}
          </div>
          <div class="saved-meta">
            <span>${it.lidos}/${it.total} cap.</span>
            ${it.updatedAt ? `<span>${formatDate(it.updatedAt)}</span>` : ''}
          </div>
        </div>
        <div class="saved-right">
          <div class="mini-bar-wrap"><div class="mini-bar${isComplete?' complete':''}" style="width:${it.percent}%"></div></div>
          <span class="saved-pct${isComplete?' complete':''}">${it.percent}%</span>
          <button class="delete-btn" aria-label="Remover ${escapeHtml(it.name)}">✕</button>
        </div>
      `;
      div.querySelector('.delete-btn').addEventListener('click', e => {
        e.stopPropagation();
        if (confirm(`Remover "${it.name}" do arquivo?`)) {
          localStorage.removeItem(it.key);
          if (activeKey===it.key) activeKey=null;
          updateTabCount(); renderSaved();
        }
      });
      div.addEventListener('click', () => {
        manga.value = it.name; total.value = String(it.total);
        lidos.value = String(it.lidos); statusSel.value = it.status||'';
        activeKey = it.key;
        calc(); renderSaved();
        document.querySelector('[data-panel="catalogar"]').click();
        manga.scrollIntoView({behavior:'smooth',block:'center'});
      });
      lista.appendChild(div);
    });
  }

  function updateTabCount() {
    const count = Object.keys(localStorage).filter(k => k.startsWith('manga:')).length;
    const badge = elId('tab-count');
    badge.textContent = count;
    badge.classList.toggle('visible', count > 0);
  }

  // ── Events ────────────────────────────────────
  elId('btnZerar').addEventListener('click', () => {
    manga.value=''; total.value=''; lidos.value=''; statusSel.value='';
    perc.textContent='0%'; resumo.textContent='0 de 0 capítulos';
    remaining.textContent=''; bar.style.width='0%'; bar.style.background='var(--accent)';
    msg.textContent='Campos limpos.'; msg.className='msg fine';
    activeKey=null; renderSaved(); manga.focus();
  });

  elId('btnCalcular').addEventListener('click', calc);
  elId('btnSalvar').addEventListener('click', save);

  document.querySelectorAll('.step-btn').forEach(btn => {
    btn.addEventListener('click', () => {
      const tid = btn.dataset.target, step = Number(btn.dataset.step)||0;
      const inp = elId(tid); if (!inp) return;
      let next = (Number(inp.value)||0) + step;
      if (next < 0) next = 0;
      if (tid==='lidos') { const tv=Number(total.value); if (Number.isFinite(tv)&&tv>=0&&next>tv) next=tv; }
      inp.value = String(next); calc();
    });
  });

  [manga, total, lidos].forEach(inp => {
    inp.addEventListener('input', calc);
    inp.addEventListener('change', calc);
    inp.addEventListener('keydown', e => {
      if (e.key==='Enter'&&!e.shiftKey){ e.preventDefault(); calc(); }
      if (e.key==='Enter'&& e.shiftKey){ e.preventDefault(); save(); }
    });
  });

  manga.addEventListener('blur',   () => { if (manga.value.trim()) loadForName(manga.value.trim()); });
  manga.addEventListener('change', () => loadForName(manga.value.trim()));

  window.addEventListener('keydown', e => {
    if ((e.ctrlKey||e.metaKey) && e.key.toLowerCase()==='s') { e.preventDefault(); save(); }
  });

  sortBy.addEventListener('change', renderSaved);
  sortOrder.addEventListener('change', renderSaved);
  searchManga.addEventListener('input', renderSaved);

  updateTabCount();
  renderSaved();
  calc();
  </script>
</body>
</html>
