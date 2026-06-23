<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Madhuri Khatal — Software Developer</title>
  <meta name="description"
    content="Portfolio of Madhuri Balasaheb Khatal, Software Developer specializing in React, React Native and TypeScript." />

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link
    href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@500;600;700;800&family=Inter:wght@400;500;600&family=JetBrains+Mono:wght@500;600;700&display=swap"
    rel="stylesheet">

  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.css">

  <style>
    :root {
      --ink: #161427;
      --ink-soft: #534f6b;
      --paper: #fbfaf8;
      --panel: #ffffff;
      --line: #e7e3ec;
      --indigo: #4338CA;
      --indigo-deep: #312693;
      --amber: #F59E0B;
      --teal: #0F9D8F;
      --font-display: 'Plus Jakarta Sans', sans-serif;
      --font-body: 'Inter', sans-serif;
      --font-mono: 'JetBrains Mono', monospace;
    }

    * {
      box-sizing: border-box;
    }

    body {
      background: var(--paper);
      color: var(--ink);
      font-family: var(--font-body);
      -webkit-font-smoothing: antialiased;
    }

    h1,
    h2,
    h3,
    h4,
    .brand {
      font-family: var(--font-display);
      letter-spacing: -0.01em;
    }

    .mono {
      font-family: var(--font-mono);
    }

    a {
      text-decoration: none;
    }

    /* ---------- navbar ---------- */
    .navbar-custom {
      background: rgba(251, 250, 248, 0.9);
      backdrop-filter: blur(10px);
      border-bottom: 1px solid var(--line);
      padding-top: .85rem;
      padding-bottom: .85rem;
    }

    .brand {
      font-weight: 800;
      font-size: 1.05rem;
      color: var(--ink);
      display: flex;
      align-items: center;
      gap: .5rem;
    }

    .brand .ver-chip {
      font-family: var(--font-mono);
      font-size: .66rem;
      font-weight: 700;
      background: var(--indigo);
      color: #fff;
      padding: .18rem .5rem;
      border-radius: 20px;
      letter-spacing: .02em;
    }

    .nav-link-custom {
      font-size: .92rem;
      font-weight: 600;
      color: var(--ink-soft) !important;
      padding: .4rem .9rem !important;
      border-radius: 8px;
    }

    .nav-link-custom:hover {
      color: var(--indigo) !important;
      background: #f1efff;
    }

    .btn-indigo {
      background: #483bb5;
      border: none;
      color: #fff;
      font-weight: 600;
      font-size: .9rem;
      padding: .5rem 1.1rem;
      border-radius: 9px;
    }

    .btn-indigo:hover {
      background: var(--indigo-deep);
      color: #fff;
    }

    section {
      padding: 5.5rem 0;
    }

    @media (max-width: 768px) {
      section {
        padding: 3.6rem 0;
      }
    }

    .eyebrow {
      font-family: var(--font-mono);
      font-size: .78rem;
      font-weight: 600;
      color: var(--indigo);
      letter-spacing: .06em;
      text-transform: uppercase;
      display: flex;
      align-items: center;
      gap: .5rem;
      margin-bottom: .9rem;
    }

    .eyebrow::before {
      content: "";
      width: 22px;
      height: 2px;
      background: var(--amber);
      display: inline-block;
    }

    .section-title {
      font-weight: 800;
      font-size: clamp(1.7rem, 3vw, 2.3rem);
      margin-bottom: .6rem;
    }

    .section-sub {
      color: var(--ink-soft);
      max-width: 560px;
      margin-bottom: 2.6rem;
    }

    /* ---------- hero ---------- */
    .hero {
      padding-top: 7rem;
    }

    .release-tag {
      display: inline-flex;
      align-items: center;
      gap: .55rem;
      background: #f1efff;
      border: 1px solid #ddd7fb;
      color: var(--indigo-deep);
      font-family: var(--font-mono);
      font-size: .78rem;
      font-weight: 600;
      padding: .4rem .9rem;
      border-radius: 30px;
      margin-bottom: 1.6rem;
    }

    .release-tag .pulse {
      width: 7px;
      height: 7px;
      border-radius: 50%;
      background: var(--teal);
      position: relative;
    }

    .release-tag .pulse::after {
      content: "";
      position: absolute;
      inset: -4px;
      border-radius: 50%;
      border: 1px solid var(--teal);
      animation: pulse 2s ease-out infinite;
    }

    @keyframes pulse {
      0% {
        transform: scale(.6);
        opacity: .8;
      }

      100% {
        transform: scale(1.8);
        opacity: 0;
      }
    }

    .hero h1 {
      font-size: clamp(2.4rem, 5vw, 3.6rem);
      font-weight: 800;
      line-height: 1.07;
      margin-bottom: 1.1rem;
    }

    .hero h1 .accent {
      color: var(--indigo);
    }

    .hero-lede {
      font-size: 1.08rem;
      color: var(--ink-soft);
      max-width: 620px;
      margin-bottom: 2rem;
    }

    .stat-row {
      display: flex;
      gap: 2.6rem;
      margin-top: 3rem;
      flex-wrap: wrap;
    }

    .stat .num {
      font-family: var(--font-display);
      font-weight: 800;
      font-size: 1.9rem;
      color: var(--ink);
    }

    .stat .lbl {
      font-size: .82rem;
      color: var(--ink-soft);
    }

    .btn-outline-dark-custom {
      border: 1.5px solid var(--ink);
      color: var(--ink);
      font-weight: 600;
      font-size: .9rem;
      padding: .5rem 1.1rem;
      border-radius: 9px;
      background: transparent;
    }

    .btn-outline-dark-custom:hover {
      background: var(--ink);
      color: #fff;
    }

    /* ---------- changelog / experience ---------- */
    .accordion-changelog .accordion-item {
      border: 1px solid var(--line);
      border-radius: 14px !important;
      margin-bottom: 1.1rem;
      overflow: hidden;
      background: var(--panel);
    }

    .accordion-changelog .accordion-button {
      font-family: var(--font-display);
      font-weight: 700;
      font-size: 1.05rem;
      padding: 1.4rem 1.6rem;
      background: var(--panel);
      color: var(--ink);
    }

    .accordion-changelog .accordion-button:not(.collapsed) {
      color: var(--indigo-deep);
      background: #f8f7ff;
    }

    .accordion-changelog .accordion-button:focus {
      box-shadow: none;
    }

    .accordion-changelog .accordion-button::after {
      filter: none;
    }

    .ver-badge {
      font-family: var(--font-mono);
      font-size: .74rem;
      font-weight: 700;
      background: var(--ink);
      color: #fff;
      padding: .25rem .6rem;
      border-radius: 6px;
      margin-right: .9rem;
    }

    .ver-badge.current {
      background: var(--teal);
    }

    .accordion-body-custom {
      padding: 0 1.6rem 1.6rem;
    }

    .changelog-org {
      color: var(--ink-soft);
      font-size: .92rem;
      margin-bottom: 1.1rem;
    }

    .changelog-meta {
      font-family: var(--font-mono);
      font-size: .78rem;
      color: var(--ink-soft);
    }

    .tag-added,
    .tag-improved {
      font-family: var(--font-mono);
      font-size: .68rem;
      font-weight: 700;
      letter-spacing: .03em;
      padding: .18rem .5rem;
      border-radius: 5px;
      margin-right: .6rem;
      flex-shrink: 0;
      white-space: nowrap;
    }

    .tag-added {
      background: #e8f7ed;
      color: #1c8a4f;
    }

    .tag-improved {
      background: #fff3e0;
      color: #b9750c;
    }

    .changelog-list {
      list-style: none;
      padding: 0;
      margin: 0;
      display: flex;
      flex-direction: column;
      gap: .65rem;
    }

    .changelog-list li {
      display: flex;
      gap: .7rem;
      align-items: flex-start;
      font-size: .94rem;
      color: var(--ink);
    }

    /* ---------- projects ---------- */
    .project-card {
      border: 1px solid var(--line);
      border-radius: 14px;
      background: var(--panel);
      padding: 1.7rem;
      height: 100%;
      transition: transform .18s ease, box-shadow .18s ease;
    }

    .project-card:hover {
      transform: translateY(-4px);
      box-shadow: 0 16px 34px -16px rgba(22, 20, 39, 0.18);
    }

    .project-top {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: .9rem;
    }

    .project-ver {
      font-family: var(--font-mono);
      font-size: .74rem;
      color: var(--ink-soft);
    }

    .badge-released {
      font-family: var(--font-mono);
      font-size: .68rem;
      font-weight: 700;
      background: #e8f7ed;
      color: #1c8a4f;
      padding: .25rem .55rem;
      border-radius: 20px;
    }

    .project-title {
      font-weight: 700;
      font-size: 1.08rem;
      margin-bottom: .7rem;
    }

    .project-card ul {
      padding-left: 1.1rem;
      margin-bottom: 1.1rem;
      color: var(--ink-soft);
      font-size: .91rem;
    }

    .project-card ul li {
      margin-bottom: .45rem;
    }

    .tech-pill {
      display: inline-block;
      font-size: .74rem;
      font-weight: 600;
      color: var(--indigo-deep);
      background: #f1efff;
      padding: .22rem .6rem;
      border-radius: 20px;
      margin: 0 .4rem .4rem 0;
    }

    /* ---------- skills ---------- */
    .skill-card {
      border: 1px solid var(--line);
      border-radius: 14px;
      background: var(--panel);
      padding: 1.6rem 1.7rem;
      height: 100%;
    }

    .skill-card .icon-box {
      width: 42px;
      height: 42px;
      border-radius: 10px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.2rem;
      margin-bottom: 1rem;
    }

    .skill-card h3 {
      font-size: 1rem;
      font-weight: 700;
      margin-bottom: .9rem;
    }

    .skill-pill {
      font-family: var(--font-mono);
      font-size: .78rem;
      color: var(--ink);
      border: 1px solid var(--line);
      padding: .32rem .7rem;
      border-radius: 7px;
      margin: 0 .4rem .5rem 0;
      display: inline-block;
      background: #fbfaf8;
    }

    /* ---------- education ---------- */
    .edu-card {
      border: 1px solid var(--line);
      border-radius: 14px;
      background: var(--panel);
      padding: 1.6rem 1.8rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 1.2rem;
      flex-wrap: wrap;
      margin-bottom: 1.1rem;
    }

    .edu-degree {
      font-weight: 700;
      font-size: 1.05rem;
      margin-bottom: .3rem;
    }

    .edu-school {
      color: var(--ink-soft);
      font-size: .9rem;
      margin-bottom: .25rem;
    }

    .edu-date {
      font-family: var(--font-mono);
      font-size: .76rem;
      color: var(--ink-soft);
    }

    .cgpa-chip {
      font-family: var(--font-mono);
      font-weight: 700;
      font-size: .84rem;
      color: var(--indigo-deep);
      background: #f1efff;
      padding: .45rem .9rem;
      border-radius: 9px;
      white-space: nowrap;
    }

    /* ---------- contact / footer ---------- */
    .contact-band {
      background: #483bb5;
      color: #fff;
      border-radius: 22px;
      padding: 3.4rem 3rem;
      margin: 0 auto;
    }

    .contact-band h2 {
      font-weight: 800;
      font-size: clamp(1.6rem, 3vw, 2.1rem);
      margin-bottom: .6rem;
    }

    .contact-band p {
      color: #bdb9d4;
      max-width: 480px;
    }

    .contact-link {
      display: flex;
      align-items: center;
      gap: .8rem;
      color: #fff;
      font-weight: 600;
      font-size: .96rem;
      padding: .85rem 0;
      border-bottom: 1px solid rgba(255, 255, 255, 0.12);
    }

    .contact-link:last-child {
      border-bottom: none;
    }

    .contact-link i {
      color: var(--amber);
      font-size: 1.05rem;
      width: 22px;
    }

    .contact-link:hover {
      color: var(--amber);
    }

    .btn-amber {
      background: var(--amber);
      color: var(--ink);
      font-weight: 700;
      border: none;
      border-radius: 9px;
      padding: .6rem 1.3rem;
      font-size: .92rem;
    }

    .btn-amber:hover {
      background: #e69009;
      color: var(--ink);
    }

    footer.site-footer {
      font-family: var(--font-mono);
      font-size: .78rem;
      color: var(--ink-soft);
      text-align: center;
      padding: 2.4rem 0 3rem;
    }

    .scroll-section {
      scroll-margin-top: 90px;
    }
  </style>
</head>

<body>

  <nav class="navbar navbar-expand-lg navbar-custom sticky-top">
    <div class="container">
      <a class="brand" href="#hero"><span>madhuri.khatal</span><span class="ver-chip">v3.2.0</span></a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navMenu">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navMenu">
        <ul class="navbar-nav align-items-lg-center gap-1">
          <li class="nav-item"><a class="nav-link nav-link-custom" href="#about">About</a></li>
          <li class="nav-item"><a class="nav-link nav-link-custom" href="#changelog">Changelog</a></li>
          <li class="nav-item"><a class="nav-link nav-link-custom" href="#projects">Projects</a></li>
          <li class="nav-item"><a class="nav-link nav-link-custom" href="#skills">Skills</a></li>
          <li class="nav-item"><a class="nav-link nav-link-custom" href="#education">Education</a></li>
          <li class="nav-item ms-lg-2 mt-2 mt-lg-0">
            <a class="btn-indigo d-inline-block" href="#contact">Contact</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- HERO -->
  <section class="hero scroll-section" id="hero">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-lg-9" id="about">
          <div class="release-tag"><span class="pulse"></span> Currently shipping v3.2.0 — open to new releases</div>
          <h1>Madhuri Khatal builds<br><span class="accent">interfaces that ship.</span></h1>
          <p class="hero-lede">Software Developer with 3+ years specializing in React, React Native, JavaScript and
            TypeScript. I build scalable web and mobile applications, optimize performance, and contribute to
            government-based digital platforms — currently as a Project Associate at C-DAC.</p>

          <div class="d-flex gap-2 flex-wrap">
            <a class="btn-indigo" href="mailto:khatalmadhuri18@gmail.com"><i class="bi bi-envelope-fill me-1"></i> Email
              me</a>
            <a class="btn-outline-dark-custom" href="https://www.linkedin.com/in/madhuri-khatal-939a45219/"
              target="_blank" rel="noopener"><i class="bi bi-linkedin me-1"></i> LinkedIn</a>
          </div>

          <div class="stat-row">
            <div class="stat">
              <div class="num">3+</div>
              <div class="lbl">years experience</div>
            </div>
            <div class="stat">
              <div class="num">4</div>
              <div class="lbl">platforms shipped</div>
            </div>
            <div class="stat">
              <div class="num">2</div>
              <div class="lbl">organizations</div>
            </div>
            <div class="stat">
              <div class="num">9.71</div>
              <div class="lbl">BCA CGPA / 10</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- CHANGELOG / EXPERIENCE -->
  <section class="scroll-section" id="changelog">
    <div class="container">
      <div class="eyebrow">Work history</div>
      <h2 class="section-title">Changelog</h2>
      <p class="section-sub">Each role, summarized the way I'd write it in a release note — what shipped, and what
        improved.</p>

      <div class="accordion accordion-changelog" id="changelogAccordion">

        <div class="accordion-item">
          <h3 class="accordion-header">
            <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#v2">
              <span class="ver-badge current">v2.0.0</span> Project Associate — C-DAC, Hyderabad
            </button>
          </h3>
          <div id="v2" class="accordion-collapse collapse show" data-bs-parent="#changelogAccordion">
            <div class="accordion-body-custom">
              <div class="changelog-org">Centre for Development of Advanced Computing &nbsp;·&nbsp; <span
                  class="changelog-meta">Sep 2025 – Present</span></div>
              <ul class="changelog-list">
                <li><span class="tag-added">ADDED</span> Working on Certification and Assessment projects, contributing
                  to development and maintenance of web-based modules and internal tools such as Proctor, WebSocket and
                  SEB.</li>
                <li><span class="tag-added">ADDED</span> Responsive UIs and RESTful API integrations using React and
                  JavaScript for assessment and certification workflows.</li>
                <li><span class="tag-improved">IMPROVED</span> Robustness and usability of assessment platforms through
                  requirement analysis, testing and documentation.</li>
                <li><span class="tag-improved">IMPROVED</span> Version control practices, managed using Git and GitHub.
                </li>
              </ul>
            </div>
          </div>
        </div>

        <div class="accordion-item">
          <h3 class="accordion-header">
            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#v1">
              <span class="ver-badge">v1.0.0</span> Software Developer — KIT Intellect Pvt. Ltd., Pune
            </button>
          </h3>
          <div id="v1" class="accordion-collapse collapse" data-bs-parent="#changelogAccordion">
            <div class="accordion-body-custom">
              <div class="changelog-org">Aundh, Pune &nbsp;·&nbsp; <span class="changelog-meta">Oct 2022 – Aug
                  2025</span></div>
              <ul class="changelog-list">
                <li><span class="tag-added">ADDED</span> Web and mobile applications built using React, React Native,
                  JavaScript and PHP.</li>
                <li><span class="tag-added">ADDED</span> New features designed and implemented in collaboration with
                  cross-functional teams.</li>
                <li><span class="tag-improved">IMPROVED</span> Code quality and performance through rigorous testing and
                  debugging.</li>
                <li><span class="tag-improved">IMPROVED</span> Deployment workflow using FileZilla and Hostinger, with
                  version control via Git and GitHub.</li>
              </ul>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- PROJECTS -->
  <section class="scroll-section" id="projects">
    <div class="container">
      <div class="eyebrow">Selected work</div>
      <h2 class="section-title">Projects</h2>
      <div class="row g-4">

        <div class="col-md-6">
          <div class="project-card">
            <div class="project-top"><span class="project-ver">v1.3.0</span><span class="badge-released">Released</span>
            </div>
            <div class="project-title">ISEA Assessment &amp; Certification Platform</div>
            <ul>
              <li>Responsive React + JavaScript UI for nationwide online quizzes and certifications under the
                Information Security Education and Awareness program.</li>
              <li>Quiz listing/detail pages with duration, difficulty, question count and validity; secure navigation to
                participation and results.</li>
              <li>Integrated REST APIs for adaptive quizzes, access control and certificate visibility.</li>
              <li>Optimized for high-traffic public campaigns on cyber safety and digital awareness.</li>
            </ul>
            <div><span class="tech-pill">React</span><span class="tech-pill">JavaScript</span><span
                class="tech-pill">REST APIs</span>
              <a href="https://assessment.isea.app/" target="_blank" rel="noopener noreferrer" class="tech-pill">View
                Project</a>
            </div>
          </div>
        </div>

        <div class="col-md-6">
          <div class="project-card">
            <div class="project-top"><span class="project-ver">v1.2.0</span><span class="badge-released">Released</span>
            </div>
            <div class="project-title">QuickSHG — Self-Help Group Management System</div>
            <ul>
              <li>Major UI components built with React and Material UI.</li>
              <li>Admin workflows designed using vanilla JavaScript.</li>
              <li>Reliable data handling for SHG transactions and product management.</li>
            </ul>
            <div><span class="tech-pill">React</span><span class="tech-pill">Material UI</span><span
                class="tech-pill">JavaScript</span>
              <a href="https://quickshg.com/" target="_blank" rel="noopener noreferrer" class="tech-pill">View
                Project</a>
            </div>
          </div>
        </div>

        <div class="col-md-6">
          <div class="project-card">
            <div class="project-top"><span class="project-ver">v1.1.0</span><span class="badge-released">Released</span>
            </div>
            <div class="project-title">Ahmedabad Municipal Corporation Portal</div>
            <ul>
              <li>Front-end UI built with vanilla JavaScript and HTML.</li>
              <li>Responsive design for desktop and mobile access.</li>
            </ul>
            <div><span class="tech-pill">javascript</span><span class="tech-pill"> html</span>
              <a href="https://amccsrportal.in/" target="_blank" rel="noopener noreferrer" class="tech-pill">View
                Project</a>
            </div>
          </div>
        </div>

        <div class="col-md-6">
          <div class="project-card">
            <div class="project-top"><span class="project-ver">v1.0.0</span><span class="badge-released">Released</span>
            </div>
            <div class="project-title">MarketingSHG</div>
            <ul>
              <li>Android app features built using React Native.</li>
              <li>Marketing workflows integrated for SHG product outreach.</li>
            </ul>
            <div><span class="tech-pill">React Native</span><span class="tech-pill">Android</span></div>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- SKILLS -->
  <section class="scroll-section" id="skills">
    <div class="container">
      <div class="eyebrow">Tooling</div>
      <h2 class="section-title">Skills</h2>
      <p class="section-sub">Languages, frameworks and the tools that keep the workflow moving.</p>

      <div class="row g-4">
        <div class="col-md-4">
          <div class="skill-card">
            <div class="icon-box" style="background:#f1efff; color:var(--indigo-deep);"><i class="bi bi-code-slash"></i>
            </div>
            <h3>Languages</h3>
            <div>
              <span class="skill-pill">JavaScript</span>
              <span class="skill-pill">TypeScript</span>
              <span class="skill-pill">PHP</span>
              <span class="skill-pill">HTML</span>
              <span class="skill-pill">CSS</span>
              <span class="skill-pill">SQL</span>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="skill-card">
            <div class="icon-box" style="background:#fff3e0; color:#b9750c;"><i class="bi bi-grid-1x2-fill"></i></div>
            <h3>Frameworks &amp; UI</h3>
            <div>
              <span class="skill-pill">React.js</span>
              <span class="skill-pill">React Native</span>
              <span class="skill-pill">Context Api</span>
              <span class="skill-pill">Redux</span>
              <span class="skill-pill">Node.js</span>
              <span class="skill-pill">Material UI</span>
              <span class="skill-pill">React Native Paper</span>
              <span class="skill-pill">React Native Base</span>
              <span class="skill-pill">Bootstrap</span>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="skill-card">
            <div class="icon-box" style="background:#e8f7ed; color:#1c8a4f;"><i class="bi bi-tools"></i></div>
            <h3>Tools &amp; Platforms</h3>
            <div>
              <span class="skill-pill">Git</span>
              <span class="skill-pill">GitHub</span>
              <span class="skill-pill">NPM</span>
              <span class="skill-pill">Android</span>
              <span class="skill-pill">Jira</span>
              <span class="skill-pill">WordPress</span>
              <span class="skill-pill">Postman</span>
              <span class="skill-pill">Thunder Client</span>
              <span class="skill-pill">FileZilla</span>
              <span class="skill-pill">Hostinger</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- EDUCATION -->
  <section class="scroll-section" id="education">
    <div class="container">
      <div class="eyebrow">Background</div>
      <h2 class="section-title">Education</h2>

      <div class="edu-card">
        <div>
          <div class="edu-degree">M.Sc. in Computer Application</div>
          <div class="edu-school">Modern College of Arts, Science and Commerce — Ganeshkhind Road, Pune</div>
          <div class="edu-date">July 2021 – April 2023</div>
        </div>
        <div class="cgpa-chip">CGPA 8.78 / 10</div>
      </div>

      <div class="edu-card">
        <div>
          <div class="edu-degree">BCA (Science)</div>
          <div class="edu-school">Sangamner Nagarpalika Arts, D.J. Malpani Commerce &amp; B.N. Sarda Science College
          </div>
          <div class="edu-date">July 2018 – April 2021</div>
        </div>
        <div class="cgpa-chip">CGPA 9.71 / 10</div>
      </div>
    </div>
  </section>

  <!-- CONTACT -->
  <section class="scroll-section" id="contact">
    <div class="container">
      <div class="contact-band">
        <div class="row align-items-center">
          <div class="col-lg-5 mb-4 mb-lg-0">
            <h2>Let's Build<br>something together.</h2>
            <p>Open to new roles and collaborations — reach out any time.</p>
          </div>
          <div class="col-lg-7">
            <a class="contact-link" href="mailto:khatalmadhuri18@gmail.com"><i class="bi bi-envelope-fill"></i>
              khatalmadhuri18@gmail.com</a>
            <a class="contact-link" href="tel:8010636141"><i class="bi bi-telephone-fill"></i> +91 80106 36141</a>
            <a class="contact-link" href="https://www.linkedin.com/in/madhuri-khatal-939a45219/" target="_blank"
              rel="noopener"><i class="bi bi-linkedin"></i> linkedin.com/in/madhuri-khatal</a>
            <a class="btn-amber d-inline-block mt-3" href="mailto:khatalmadhuri18@gmail.com">Send an email</a>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- <footer class="site-footer"></footer> -->

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>

</html>
