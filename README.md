<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Suhail Malik – GitHub README</title>
<link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;500;600&family=Rajdhani:wght@500;600;700&family=Source+Sans+3:ital,wght@0,300;0,400;0,600;1,300&display=swap" rel="stylesheet"/>
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}

body{
  background:#0d1117;
  color:#c9d1d9;
  font-family:'Source Sans 3',sans-serif;
  font-weight:300;
  min-height:100vh;
  display:flex;
  flex-direction:column;
  align-items:center;
  padding:0;
}

/* ── GITHUB CHROME ── */
.gh-topbar{
  width:100%;
  background:#161b22;
  border-bottom:1px solid #30363d;
  padding:0.7rem 1.4rem;
  display:flex;
  align-items:center;
  gap:1rem;
}
.gh-logo{color:#f0f6fc;font-size:1.5rem;}
.gh-search{
  background:#0d1117;
  border:1px solid #30363d;
  border-radius:6px;
  padding:0.3rem 0.8rem;
  color:#8b949e;
  font-size:0.8rem;
  font-family:'Fira Code',monospace;
  width:240px;
}
.gh-nav{display:flex;gap:1.4rem;margin-left:auto;}
.gh-nav a{color:#c9d1d9;font-size:0.82rem;text-decoration:none;opacity:0.8;}

.gh-repo-header{
  width:100%;
  max-width:1200px;
  padding:1.2rem 1.6rem 0.6rem;
  border-bottom:1px solid #30363d;
  display:flex;
  align-items:center;
  gap:0.5rem;
  flex-wrap:wrap;
}
.gh-repo-path{font-size:1.1rem;color:#58a6ff;font-family:'Fira Code',monospace;}
.gh-repo-path span{color:#8b949e;}
.gh-badge{
  background:#21262d;
  border:1px solid #30363d;
  border-radius:2rem;
  padding:0.12rem 0.7rem;
  font-size:0.72rem;
  color:#8b949e;
  margin-left:0.4rem;
}

.gh-tabs{
  width:100%;
  max-width:1200px;
  padding:0 1.6rem;
  display:flex;
  gap:0;
  border-bottom:1px solid #30363d;
}
.gh-tab{
  padding:0.7rem 1rem;
  font-size:0.85rem;
  color:#8b949e;
  cursor:pointer;
  border-bottom:2px solid transparent;
  display:flex;
  align-items:center;
  gap:0.4rem;
}
.gh-tab.active{color:#f0f6fc;border-bottom:2px solid #f78166;}
.gh-tab-count{
  background:#21262d;
  border:1px solid #30363d;
  border-radius:2rem;
  padding:0 0.5rem;
  font-size:0.7rem;
}

/* ── MAIN LAYOUT ── */
.gh-main{
  width:100%;
  max-width:1200px;
  display:grid;
  grid-template-columns:1fr 296px;
  gap:1.6rem;
  padding:1.4rem 1.6rem;
}

/* ── FILE HEADER ── */
.file-header{
  background:#161b22;
  border:1px solid #30363d;
  border-radius:6px 6px 0 0;
  padding:0.6rem 1rem;
  display:flex;
  align-items:center;
  justify-content:space-between;
  border-bottom:1px solid #30363d;
}
.file-name{font-family:'Fira Code',monospace;font-size:0.82rem;color:#8b949e;}
.file-name strong{color:#c9d1d9;}
.file-actions{display:flex;gap:0.4rem;}
.file-btn{
  background:#21262d;
  border:1px solid #30363d;
  border-radius:6px;
  color:#c9d1d9;
  font-size:0.75rem;
  padding:0.2rem 0.6rem;
  cursor:pointer;
}

/* ── README BOX ── */
.readme-box{
  background:#0d1117;
  border:1px solid #30363d;
  border-top:none;
  border-radius:0 0 6px 6px;
  overflow:hidden;
}

/* ── README CONTENT ── */
.readme-content{padding:2rem 2.4rem 2.4rem;}

.hero-banner{
  background:linear-gradient(135deg,#96281b 0%,#c0392b 55%,#a93226 100%);
  border-radius:6px;
  padding:2.6rem 2rem 2.2rem;
  text-align:center;
  position:relative;
  overflow:hidden;
  margin-bottom:1.6rem;
}
.hero-banner::before{
  content:'';
  position:absolute;inset:0;
  background:repeating-linear-gradient(45deg,transparent,transparent 20px,rgba(0,0,0,0.07) 20px,rgba(0,0,0,0.07) 21px);
}
.hero-banner h1{
  font-family:'Rajdhani',sans-serif;
  font-size:2.8rem;
  font-weight:700;
  color:#fff;
  letter-spacing:0.05em;
  position:relative;z-index:1;
  text-shadow:0 2px 10px rgba(0,0,0,0.5);
  animation:fadeDown 0.6s ease both;
}
.hero-banner .sub{
  font-size:0.95rem;
  color:rgba(255,255,255,0.8);
  letter-spacing:0.14em;
  text-transform:uppercase;
  position:relative;z-index:1;
  margin-top:0.35rem;
  animation:fadeDown 0.6s 0.15s ease both;
}

@keyframes fadeDown{from{opacity:0;transform:translateY(-12px)}to{opacity:1;transform:none}}

/* tagline */
.tagline{text-align:center;margin-bottom:1.8rem;padding-bottom:1.6rem;border-bottom:1px solid #30363d;}
.tagline .exploring{
  font-family:'Rajdhani',sans-serif;
  font-size:1rem;
  color:#f1c40f;
  font-weight:600;
  letter-spacing:0.15em;
  text-transform:uppercase;
  margin-bottom:0.55rem;
  display:flex;align-items:center;justify-content:center;gap:0.5rem;
}
.tagline p{font-size:0.9rem;color:#8b949e;line-height:1.75;}
.tagline p strong{color:#c9d1d9;}

/* sections */
.section{margin-bottom:1.8rem;padding-bottom:1.8rem;border-bottom:1px solid #30363d;}
.section:last-child{border-bottom:none;margin-bottom:0;}
.sec-title{
  font-family:'Rajdhani',sans-serif;
  font-size:0.95rem;
  font-weight:600;
  color:#f1c40f;
  text-transform:uppercase;
  letter-spacing:0.18em;
  display:flex;align-items:center;gap:0.5rem;
  margin-bottom:1rem;
}
.focus-item{
  display:flex;align-items:flex-start;gap:0.7rem;
  margin-bottom:0.6rem;font-size:0.88rem;color:#8b949e;
}
.focus-item strong{color:#c9d1d9;}

/* tech badges */
.tech-grid{display:flex;flex-wrap:wrap;gap:0.5rem;margin-top:0.6rem;}
.tbadge{
  display:flex;align-items:center;gap:0.35rem;
  background:#21262d;border:1px solid #30363d;border-radius:4px;
  padding:0.3rem 0.7rem;
  font-family:'Fira Code',monospace;font-size:0.75rem;color:#8b949e;
  transition:border-color 0.2s,color 0.2s;
  animation:popIn 0.4s ease both;
}
.tbadge:hover{border-color:#f1c40f;color:#f1c40f;}
.tbadge .dot{width:8px;height:8px;border-radius:50%;}

@keyframes popIn{from{opacity:0;transform:scale(0.9)}to{opacity:1;transform:scale(1)}}

/* ── SIDEBAR ── */
.sidebar{}
.about-box{
  background:#161b22;border:1px solid #30363d;border-radius:6px;
  padding:1rem 1.1rem;margin-bottom:1rem;
}
.about-box h3{font-size:0.85rem;font-weight:600;color:#f0f6fc;margin-bottom:0.7rem;}
.about-box p{font-size:0.82rem;color:#8b949e;line-height:1.6;margin-bottom:0.9rem;}
.about-item{
  display:flex;align-items:center;gap:0.5rem;
  font-size:0.8rem;color:#8b949e;margin-bottom:0.4rem;
}
.about-item a{color:#58a6ff;text-decoration:none;}
.lang-bar{margin-top:0.5rem;}
.lang-bar-track{
  height:8px;border-radius:6px;overflow:hidden;
  display:flex;margin-bottom:0.6rem;
}
.lang-seg{height:100%;}
.lang-list{display:flex;flex-wrap:wrap;gap:0.5rem;}
.lang-dot{display:flex;align-items:center;gap:0.35rem;font-size:0.75rem;color:#8b949e;}
.lang-dot::before{content:'';display:inline-block;width:10px;height:10px;border-radius:50%;background:var(--c);}
</style>
</head>
<body>

<!-- GITHUB TOPBAR -->
<div class="gh-topbar">
  <div class="gh-logo">
    <svg height="22" viewBox="0 0 16 16" fill="currentColor">
      <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"/>
    </svg>
  </div>
  <input class="gh-search" value="Search or jump to…" readonly/>
  <nav class="gh-nav">
    <a href="#">Pull requests</a>
    <a href="#">Issues</a>
    <a href="#">Marketplace</a>
    <a href="#">Explore</a>
  </nav>
</div>

<!-- REPO HEADER -->
<div class="gh-repo-header">
  <span class="gh-repo-path">
    <span>suhail05509 </span>/ <strong>suhail05509</strong>
  </span>
  <span class="gh-badge">Public</span>
</div>

<!-- TABS -->
<div class="gh-tabs">
  <div class="gh-tab active">📄 Code</div>
  <div class="gh-tab">⚠ Issues <span class="gh-tab-count">0</span></div>
  <div class="gh-tab">🔀 Pull requests <span class="gh-tab-count">0</span></div>
  <div class="gh-tab">▶ Actions</div>
  <div class="gh-tab">☰ Projects</div>
  <div class="gh-tab">📦 Packages</div>
  <div class="gh-tab">⭐ Stars <span class="gh-tab-count">6</span></div>
</div>

<!-- MAIN -->
<div class="gh-main">

  <!-- LEFT: README -->
  <div>
    <div class="file-header">
      <span class="file-name"><strong>suhail05509</strong> / README.md</span>
      <div class="file-actions">
        <button class="file-btn">✏️ Edit</button>
        <button class="file-btn">⋯</button>
      </div>
    </div>

    <div class="readme-box">
      <div class="readme-content">

        <!-- HERO -->
        <div class="hero-banner">
          <h1>Suhail Malik</h1>
          <p class="sub">Aspiring Software Engineer &nbsp;|&nbsp; AI Systems Student</p>
        </div>

        <!-- TAGLINE -->
        <div class="tagline">
          <div class="exploring">🔍 Exploring LLM RAG Pipe</div>
          <p>
            Engineering <strong>intelligent tools</strong>, seamless automations, and resilient architectures.<br/>
            Bridging the gap between sophisticated AI models and production-ready software.
          </p>
        </div>

        <!-- STRATEGIC FOCUS -->
        <div class="section">
          <div class="sec-title">🎯 Strategic Focus</div>
          <div class="focus-item"><span>🚀</span><span><strong>Core Mission:</strong> Designing autonomous AI agents and modern SaaS architectures as a student builder.</span></div>
          <div class="focus-item"><span>🔬</span><span><strong>Researching:</strong> Advanced Vector Databases, low-latency LLM inference, and CI/CD for AI.</span></div>
          <div class="focus-item"><span>🛡️</span><span><strong>Infrastructure:</strong> Building with a "Security-First" mindset and high-concurrency performance.</span></div>
          <div class="focus-item"><span>📖</span><span><strong>Principles:</strong> Writing self-documenting code and building systems that scale horizontally.</span></div>
        </div>

        <!-- TECH ECOSYSTEM -->
        <div class="section">
          <div class="sec-title">🛠️ Technical Ecosystem</div>
          <div class="tech-grid">
            <div class="tbadge" style="animation-delay:0.05s"><span class="dot" style="background:#f7df1e"></span>JavaScript</div>
            <div class="tbadge" style="animation-delay:0.1s"><span class="dot" style="background:#3178c6"></span>TypeScript</div>
            <div class="tbadge" style="animation-delay:0.15s"><span class="dot" style="background:#61dafb"></span>React</div>
            <div class="tbadge" style="animation-delay:0.2s"><span class="dot" style="background:#68a063"></span>Node.js</div>
            <div class="tbadge" style="animation-delay:0.25s"><span class="dot" style="background:#000"></span>Express</div>
            <div class="tbadge" style="animation-delay:0.3s"><span class="dot" style="background:#fff"></span>Next.js</div>
            <div class="tbadge" style="animation-delay:0.35s"><span class="dot" style="background:#3572A5"></span>Python</div>
            <div class="tbadge" style="animation-delay:0.4s"><span class="dot" style="background:#009485"></span>FastAPI</div>
            <div class="tbadge" style="animation-delay:0.45s"><span class="dot" style="background:#4DB33D"></span>MongoDB</div>
            <div class="tbadge" style="animation-delay:0.5s"><span class="dot" style="background:#336791"></span>PostgreSQL</div>
            <div class="tbadge" style="animation-delay:0.55s"><span class="dot" style="background:#FF9900"></span>AWS</div>
            <div class="tbadge" style="animation-delay:0.6s"><span class="dot" style="background:#2496ED"></span>Docker</div>
            <div class="tbadge" style="animation-delay:0.65s"><span class="dot" style="background:#1C3C3C"></span>LangChain</div>
            <div class="tbadge" style="animation-delay:0.7s"><span class="dot" style="background:#7c3aed"></span>Vector DBs</div>
            <div class="tbadge" style="animation-delay:0.75s"><span class="dot" style="background:#f39c12"></span>LLM APIs</div>
          </div>
        </div>

      </div>
    </div>
  </div>

  <!-- SIDEBAR -->
  <div class="sidebar">
    <div class="about-box">
      <h3>About</h3>
      <p>I'm a full-stack developer (MERN) currently transitioning into the world of AI Automation & AI Agents and Voice-based AI agents. I love building products.</p>
      <div class="about-item">🌐 <a href="#">Botfessor.Ai</a></div>
      <div class="about-item">📍 Moradabad</div>
      <div class="about-item">✉️ mohdsuhail895@gmail.com</div>
      <div class="about-item">🔗 <a href="#">LinkedIn</a></div>
      <div class="about-item">𝕏 <a href="#">@MohdSuhail05509</a></div>
    </div>

    <div class="about-box">
      <h3>Languages</h3>
      <div class="lang-bar">
        <div class="lang-bar-track">
          <div class="lang-seg" style="width:40%;background:#f7df1e"></div>
          <div class="lang-seg" style="width:25%;background:#3572A5"></div>
          <div class="lang-seg" style="width:20%;background:#3178c6"></div>
          <div class="lang-seg" style="width:15%;background:#68a063"></div>
        </div>
        <div class="lang-list">
          <div class="lang-dot" style="--c:#f7df1e">JavaScript 40%</div>
          <div class="lang-dot" style="--c:#3572A5">Python 25%</div>
          <div class="lang-dot" style="--c:#3178c6">TypeScript 20%</div>
          <div class="lang-dot" style="--c:#68a063">Other 15%</div>
        </div>
      </div>
    </div>

    <div class="about-box">
      <h3>Stats</h3>
      <div class="about-item">👁 2 followers</div>
      <div class="about-item">👣 6 following</div>
    </div>
  </div>

</div>
</body>
</html>
