<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Md. Shaharia Hossen | ETE Engineer · RUET</title>

  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">

  <style>
    * { margin:0; padding:0; box-sizing:border-box; }

    body {
      font-family: 'Inter', sans-serif;
      background: var(--bg-primary);
      color: var(--text-primary);
      line-height: 1.6;
      scroll-behavior: smooth;
      transition: 0.3s;
    }

    :root {
      --bg-primary:#0b1120;
      --bg-secondary:#111827;
      --card-bg:rgba(30,41,59,0.6);
      --text-primary:#f1f5f9;
      --text-secondary:#cbd5e1;
      --accent:#38bdf8;
      --accent-hover:#7dd3fc;
      --border:rgba(56,189,248,0.2);
      --shadow:0 20px 35px -10px rgba(0,0,0,0.4);
      --navbar-blur:rgba(15,23,42,0.85);
    }

    body.light {
      --bg-primary:#f8fafc;
      --bg-secondary:#e2e8f0;
      --card-bg:rgba(255,255,255,0.75);
      --text-primary:#0f172a;
      --text-secondary:#334155;
      --accent:#0284c7;
      --accent-hover:#0ea5e9;
      --border:rgba(2,132,199,0.25);
      --navbar-blur:rgba(248,250,252,0.9);
    }

    .container { max-width:1200px; margin:auto; padding:0 1.5rem; }

    nav {
      position:fixed; top:0; width:100%;
      backdrop-filter:blur(12px);
      background:var(--navbar-blur);
      padding:1rem 0;
      border-bottom:1px solid var(--border);
      z-index:1000;
    }

    .nav-content {
      display:flex;
      justify-content:space-between;
      align-items:center;
      flex-wrap:wrap;
      gap:1rem;
    }

    .logo {
      font-weight:700;
      font-size:1.3rem;
      color:var(--accent);
    }

    .nav-links {
      display:flex;
      gap:1.5rem;
      flex-wrap:wrap;
    }

    .nav-links a {
      text-decoration:none;
      color:var(--text-primary);
      font-weight:500;
    }

    .nav-links a:hover,
    .nav-links a.active {
      color:var(--accent);
    }

    .theme-toggle {
      width:40px; height:40px;
      border-radius:50%;
      border:none;
      cursor:pointer;
      background:var(--bg-secondary);
      color:var(--text-primary);
    }

    section { padding:90px 0 60px; }

    .hero { min-height:100vh; display:flex; align-items:center; padding-top:80px; }

    .avatar {
      width:120px; height:120px;
      border-radius:50%;
      background:var(--accent);
      display:flex;
      align-items:center;
      justify-content:center;
      font-size:2.5rem;
      font-weight:bold;
      color:#0f172a;
      margin-bottom:1rem;
    }

    h1 {
      font-size:2.8rem;
      background:linear-gradient(90deg,#fff,var(--accent));
      -webkit-background-clip:text;
      color:transparent;
    }

    .typed-text { color:var(--accent); font-size:1.3rem; margin:1rem 0; }

    .hero-desc { color:var(--text-secondary); max-width:600px; }

    .btn {
      padding:0.7rem 1.5rem;
      border-radius:30px;
      text-decoration:none;
      font-weight:600;
      display:inline-flex;
      gap:0.5rem;
      align-items:center;
    }

    .btn-primary { background:var(--accent); color:#0f172a; }
    .btn-outline { border:1px solid var(--accent); color:var(--accent); }

    .btn-primary:hover { background:var(--accent-hover); }
    .btn-outline:hover { background:var(--accent); color:#0f172a; }

    .grid-2 {
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
      gap:1.5rem;
    }

    .card {
      background:var(--card-bg);
      padding:1.5rem;
      border-radius:20px;
      border:1px solid var(--border);
      transition:0.3s;
    }

    .card:hover {
      transform:translateY(-5px);
      box-shadow:var(--shadow);
    }

    .section-title {
      font-size:2rem;
      margin-bottom:2rem;
      position:relative;
    }

    .section-title::after {
      content:'';
      width:60px;
      height:3px;
      background:var(--accent);
      position:absolute;
      left:0;
      bottom:-8px;
    }

    footer {
      text-align:center;
      padding:2rem;
      background:var(--bg-secondary);
    }
  </style>
</head>

<body>

<nav>
  <div class="container nav-content">
    <div class="logo">Shaharia.dev</div>

    <div class="nav-links">
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </div>

    <button class="theme-toggle" id="themeToggle">
      <i class="fas fa-moon"></i>
    </button>
  </div>
</nav>

<main>

<section id="home" class="hero">
  <div class="container">
    <div class="avatar">SH</div>
    <h1>Md. Shaharia Hossen</h1>
    <div class="typed-text" id="typed"></div>

    <p class="hero-desc">
      ETE Undergraduate @ RUET | Data Analyst | YouTuber | Tech Enthusiast
    </p>

    <div style="margin-top:1.2rem; display:flex; gap:1rem; flex-wrap:wrap;">
      <a class="btn btn-primary" href="https://github.com/shahariar0007"><i class="fab fa-github"></i> GitHub</a>
      <a class="btn btn-outline" href="https://youtube.com/@SmarterDotcom"><i class="fab fa-youtube"></i> YouTube</a>
    </div>
  </div>
</section>

<section id="about">
  <div class="container">
    <h2 class="section-title">About Me</h2>
    <p>
      Electronics & Telecommunication Engineering student at RUET.
      Passionate about data analysis, embedded systems, and content creation.
      I also run a YouTube channel and work as a tutor.
    </p>
  </div>
</section>

<section id="skills" style="background:var(--bg-secondary);">
  <div class="container">
    <h2 class="section-title">Skills</h2>

    <div class="grid-2">
      <div class="card">
        <h3>Programming</h3>
        <p>HTML, CSS, JavaScript, Python, C++</p>
      </div>

      <div class="card">
        <h3>Data</h3>
        <p>Pandas, Matplotlib, Seaborn</p>
      </div>

      <div class="card">
        <h3>Electronics</h3>
        <p>Arduino, Circuit Design, MATLAB</p>
      </div>

      <div class="card">
        <h3>Soft Skills</h3>
        <p>Public Speaking, Leadership, Teaching</p>
      </div>
    </div>
  </div>
</section>

<section id="projects">
  <div class="container">
    <h2 class="section-title">Projects</h2>

    <div class="grid-2">
      <div class="card">
        <h3>Data Visualization</h3>
        <p>Real-world dataset analysis using Python.</p>
      </div>

      <div class="card">
        <h3>Portfolio Website</h3>
        <p>This responsive portfolio built with HTML/CSS/JS.</p>
      </div>
    </div>
  </div>
</section>

<section id="contact" style="background:var(--bg-secondary);">
  <div class="container">
    <h2 class="section-title">Contact</h2>

    <p>Email: shahariar0007@ruet.ac.bd</p>
    <p>GitHub: github.com/shahariar0007</p>
    <p>Location: Rajshahi, Bangladesh</p>
  </div>
</section>

</main>

<footer>
  © 2026 Md. Shaharia Hossen | RUET ETE
</footer>

<script>
  const roles = ["ETE Student @ RUET", "Data Analyst", "YouTuber"];
  let i = 0, j = 0;
  const typed = document.getElementById("typed");

  function type() {
    if (j < roles[i].length) {
      typed.textContent += roles[i][j++];
      setTimeout(type, 80);
    } else {
      setTimeout(erase, 1500);
    }
  }

  function erase() {
    if (j > 0) {
      typed.textContent = roles[i].slice(0, --j);
      setTimeout(erase, 50);
    } else {
      i = (i + 1) % roles.length;
      setTimeout(type, 300);
    }
  }

  type();

  const btn = document.getElementById("themeToggle");
  btn.onclick = () => document.body.classList.toggle("light");
</script>

</body>
</html>
