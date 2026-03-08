<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Suhail Malik — README</title>
<link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;500;600&family=Rajdhani:wght@500;600;700&family=Source+Sans+3:wght@300;400;600&display=swap" rel="stylesheet"/>
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --bg: #0d1117;
    --surface: #161b22;
    --border: #30363d;
    --red: #c0392b;
    --red-dark: #96281b;
    --yellow: #f39c12;
    --yellow-bright: #f1c40f;
    --text: #c9d1d9;
    --text-muted: #8b949e;
    --text-dim: #6e7681;
    --green: #3fb950;
    --blue: #58a6ff;
    --white: #f0f6fc;
  }

  body {
    background: var(--bg);
    color: var(--text);
    font-family: 'Source Sans 3', sans-serif;
    font-weight: 300;
    line-height: 1.7;
    min-height: 100vh;
    padding: 2rem 1rem;
  }

  .readme-wrap {
    max-width: 860px;
    margin: 0 auto;
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 6px;
    overflow: hidden;
  }

  /* ── HERO BANNER ── */
  .hero {
    background: linear-gradient(135deg, var(--red-dark) 0%, var(--red) 60%, #a93226 100%);
    padding: 2.8rem 2rem 2.4rem;
    text-align: center;
    position: relative;
    overflow: hidden;
  }
  .hero::before {
    content: '';
    position: absolute;
    inset: 0;
    background: repeating-linear-gradient(
      45deg,
      transparent,
      transparent 18px,
      rgba(0,0,0,0.06) 18px,
      rgba(0,0,0,0.06) 19px
    );
  }
  .hero h1 {
    font-family: 'Rajdhani', sans-serif;
    font-size: 3rem;
    font-weight: 700;
    color: #fff;
    letter-spacing: 0.04em;
    position: relative;
    z-index: 1;
    text-shadow: 0 2px 12px rgba(0,0,0,0.4);
  }
  .hero .subtitle {
    font-family: 'Source Sans 3', sans-serif;
    font-size: 1rem;
    font-weight: 300;
    color: rgba(255,255,255,0.82);
    letter-spacing: 0.12em;
    text-transform: uppercase;
    margin-top: 0.4rem;
    position: relative;
    z-index: 1;
  }

  /* ── BODY ── */
  .body {
    padding: 2rem 2.4rem 2.6rem;
  }

  /* ── SECTION HEADING ── */
  .section-title {
    font-family: 'Rajdhani', sans-serif;
    font-size: 1.05rem;
    font-weight: 600;
    color: var(--yellow-bright);
    text-transform: uppercase;
    letter-spacing: 0.18em;
    margin-bottom: 0.9rem;
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }
  .section-title .icon { font-size: 1rem; }

  /* ── TAGLINE BLOCK ── */
  .tagline-block {
    text-align: center;
    padding: 1.2rem 1rem 1.6rem;
    border-bottom: 1px solid var(--border);
    margin-bottom: 1.8rem;
  }
  .tagline-block p {
    font-size: 0.95rem;
    color: var(--text-muted);
    max-width: 540px;
    margin: 0 auto;
    line-height: 1.75;
  }
  .tagline-block p strong {
    color: var(--text);
    font-weight: 600;
  }

  /* ── STRATEGIC FOCUS ── */
  .focus-block {
    margin-bottom: 2rem;
    padding-bottom: 1.8rem;
    border-bottom: 1px solid var(--border);
  }
  .focus-item {
    display: flex;
    align-items: flex-start;
    gap: 0.75rem;
    margin-bottom: 0.65rem;
    font-size: 0.9rem;
    color: var(--text-muted);
  }
  .focus-item .bullet { font-size: 0.95rem; flex-shrink: 0; margin-top: 0.1rem; }
  .focus-item strong { color: var(--text); font-weight: 600; }

  /* ── TECH ECOSYSTEM ── */
  .tech-block { margin-bottom: 2rem; }
  .tech-icons {
    display: flex;
    flex-wrap: wrap;
    gap: 0.6rem;
    margin-top: 0.8rem;
  }
  .tech-badge {
    background: #21262d;
    border: 1px solid var(--border);
    border-radius: 4px;
    padding: 0.35rem 0.75rem;
    font-family: 'Fira Code', monospace;
    font-size: 0.78rem;
    color: var(--text-muted);
    transition: border-color 0.2s, color 0.2s;
    cursor: default;
  }
  .tech-badge:hover { border-color: var(--yellow); color: var(--yellow-bright); }

  /* ── DIVIDER ── */
  hr.divider {
    border: none;
    border-top: 1px solid var(--border);
    margin: 1.6rem 0;
  }

  /* ── FOOTER NOTE ── */
  .footer-note {
    text-align: center;
    font-family: 'Fira Code', monospace;
    font-size: 0.75rem;
    color: var(--text-dim);
    letter-spacing: 0.05em;
    padding-top: 1rem;
  }
  .footer-note span { color: var(--red); }
</style>
</head>
<body>

<div class="readme-wrap">

  <!-- HERO -->
  <div class="hero">
    <h1>Suhail Malik</h1>
    <p class="subtitle">Aspiring Software Engineer &nbsp;|&nbsp; AI Systems Student</p>
  </div>

  <!-- BODY -->
  <div class="body">

    <!-- TAGLINE -->
    <div class="tagline-block">
      <p class="section-title" style="justify-content:center; margin-bottom:0.6rem;">
        <span class="icon">🔍</span> Exploring LLM RAG Pipe
      </p>
      <p>
        Engineering <strong>intelligent tools</strong>, seamless automations, and resilient architectures.<br/>
        Bridging the gap between sophisticated AI models and production-ready software.
      </p>
    </div>

    <!-- STRATEGIC FOCUS -->
    <div class="focus-block">
      <p class="section-title"><span class="icon">🎯</span> Strategic Focus</p>

      <div class="focus-item">
        <span class="bullet">🚀</span>
        <span><strong>Core Mission:</strong> Designing autonomous AI agents and modern SaaS architectures as a student builder.</span>
      </div>
      <div class="focus-item">
        <span class="bullet">🔬</span>
        <span><strong>Researching:</strong> Advanced Vector Databases, low-latency LLM inference, and CI/CD for AI.</span>
      </div>
      <div class="focus-item">
        <span class="bullet">🛡️</span>
        <span><strong>Infrastructure:</strong> Building with a "Security-First" mindset and high-concurrency performance.</span>
      </div>
      <div class="focus-item">
        <span class="bullet">📖</span>
        <span><strong>Principles:</strong> Writing self-documenting code and building systems that scale horizontally.</span>
      </div>
    </div>

    <!-- TECHNICAL ECOSYSTEM -->
    <div class="tech-block">
      <p class="section-title"><span class="icon">🛠️</span> Technical Ecosystem</p>
      <div class="tech-icons">
        <span class="tech-badge">JavaScript</span>
        <span class="tech-badge">TypeScript</span>
        <span class="tech-badge">React</span>
        <span class="tech-badge">Node.js</span>
        <span class="tech-badge">Express</span>
        <span class="tech-badge">Next.js</span>
        <span class="tech-badge">Python</span>
        <span class="tech-badge">FastAPI</span>
        <span class="tech-badge">MongoDB</span>
        <span class="tech-badge">PostgreSQL</span>
        <span class="tech-badge">AWS</span>
        <span class="tech-badge">Docker</span>
        <span class="tech-badge">LangChain</span>
        <span class="tech-badge">Vector DBs</span>
        <span class="tech-badge">LLM APIs</span>
      </div>
    </div>

    <hr class="divider"/>

    <p class="footer-note">
      Built with <span>♥</span> &nbsp;·&nbsp; github.com/suhail05509
    </p>

  </div>
</div>

</body>
</html>
