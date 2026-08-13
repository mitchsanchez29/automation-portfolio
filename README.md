<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Michelle Sanchez — Automation, Reporting & Operations portfolio.">
<title>Michelle Sanchez | Automation, Reporting & Operations</title>

<style>
:root{
  --bg:#0a0d12;
  --surface:#11161d;
  --surface-2:#151c24;
  --border:#27313d;
  --text:#f4f7f8;
  --muted:#a2adb8;
  --dim:#6f7c89;
  --accent:#65e6b5;
  --accent-soft:rgba(101,230,181,.08);
  --sans:Inter,system-ui,-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;
  --mono:ui-monospace,SFMono-Regular,Consolas,"Liberation Mono",monospace;
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{
  background:var(--bg);
  color:var(--text);
  font-family:var(--sans);
  line-height:1.65;
}
a{color:inherit}
.container{max-width:1120px;margin:auto;padding:0 28px}

nav{
  position:fixed;
  z-index:100;
  top:0;left:0;right:0;
  background:rgba(10,13,18,.9);
  backdrop-filter:blur(16px);
  border-bottom:1px solid var(--border);
}
.nav-inner{
  max-width:1120px;
  margin:auto;
  padding:15px 28px;
  display:flex;
  align-items:center;
  justify-content:space-between;
}
.logo{
  font:500 12px var(--mono);
  color:var(--accent);
  letter-spacing:.05em;
  text-decoration:none;
}
nav ul{display:flex;gap:25px;list-style:none}
nav ul a{
  color:var(--muted);
  text-decoration:none;
  font:400 11px var(--mono);
}
nav ul a:hover{color:var(--text)}
.nav-contact{
  border:1px solid var(--accent);
  color:var(--accent)!important;
  padding:7px 12px;
  border-radius:5px;
}

.hero{
  min-height:100vh;
  display:flex;
  align-items:center;
  border-bottom:1px solid var(--border);
}
.hero-content{padding:150px 0 100px}
.eyebrow,.section-label{
  color:var(--accent);
  font:400 11px var(--mono);
  letter-spacing:.13em;
  text-transform:uppercase;
}
.eyebrow{margin-bottom:24px}
.hero h1{
  max-width:900px;
  font-size:clamp(44px,7vw,78px);
  line-height:1.03;
  letter-spacing:-.05em;
}
.hero h1 span{color:var(--accent)}
.hero-sub{
  max-width:720px;
  margin:28px 0 34px;
  color:var(--muted);
  font-size:18px;
}
.actions{display:flex;gap:12px;flex-wrap:wrap}
.btn{
  display:inline-block;
  padding:11px 17px;
  border:1px solid var(--border);
  border-radius:5px;
  text-decoration:none;
  font:500 11px var(--mono);
  transition:.2s ease;
}
.btn-primary{
  background:var(--accent);
  border-color:var(--accent);
  color:#07110d;
}
.btn-primary:hover{transform:translateY(-1px)}
.btn-secondary{color:var(--muted)}
.btn-secondary:hover{border-color:#596777;color:var(--text)}

section{padding:92px 0;border-bottom:1px solid var(--border)}
.section-label{margin-bottom:12px}
.section-title{
  font-size:34px;
  line-height:1.15;
  letter-spacing:-.035em;
  margin-bottom:15px;
}
.section-intro{
  max-width:700px;
  color:var(--muted);
  margin-bottom:42px;
}

.about-grid{
  display:grid;
  grid-template-columns:1.15fr .85fr;
  gap:70px;
}
.about-copy p{
  color:var(--muted);
  margin-bottom:18px;
  font-size:16px;
}
.process{display:grid;gap:10px}
.process-item{
  padding:17px 18px;
  background:var(--surface);
  border:1px solid var(--border);
  border-radius:7px;
}
.process-item strong{font-size:14px}
.process-item small{
  display:block;
  margin-top:3px;
  color:var(--dim);
  font:400 10px var(--mono);
}

.services{
  display:grid;
  grid-template-columns:repeat(2,1fr);
  gap:16px;
}
.service{
  padding:27px;
  background:var(--surface);
  border:1px solid var(--border);
  border-radius:8px;
}
.service h3{font-size:18px;margin-bottom:9px}
.service p{color:var(--muted);font-size:14px}
.output{
  margin-top:20px;
  padding-top:15px;
  border-top:1px solid var(--border);
  color:var(--accent);
  font:400 10px var(--mono);
  text-transform:uppercase;
  letter-spacing:.04em;
}

.projects{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:16px;
}
.project{
  display:flex;
  flex-direction:column;
  padding:25px;
  background:var(--surface);
  border:1px solid var(--border);
  border-radius:8px;
}
.project:hover{border-color:#3b4856}
.project-number{
  color:var(--accent);
  font:400 10px var(--mono);
  letter-spacing:.08em;
  margin-bottom:18px;
}
.project h3{
  font-size:19px;
  line-height:1.3;
  margin-bottom:12px;
}
.label{
  color:var(--dim);
  font:400 9px var(--mono);
  letter-spacing:.1em;
  text-transform:uppercase;
  margin-top:14px;
  margin-bottom:3px;
}
.project p{color:var(--muted);font-size:13px}
.project .result{color:var(--text)}
.project-link{
  margin-top:22px;
  color:var(--accent);
  font:400 10px var(--mono);
  text-decoration:none;
}
.project-link:hover{text-decoration:underline}


.feedback-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:16px}
.feedback-card{background:var(--surface);border:1px solid var(--border);border-radius:8px;overflow:hidden}
.feedback-card img{display:block;width:100%;height:auto}
.feedback-meta{padding:13px 16px;color:var(--accent);font:400 10px var(--mono);letter-spacing:.06em}
@media(max-width:850px){.feedback-grid{grid-template-columns:1fr}}
.feedback{
  padding:32px;
  background:var(--surface);
  border:1px solid var(--border);
  border-radius:8px;
}
.feedback-quote{
  max-width:850px;
  font-size:20px;
  line-height:1.55;
}
.feedback-note{
  margin-top:18px;
  color:var(--dim);
  font:400 10px var(--mono);
  letter-spacing:.08em;
}

.experience{
  display:grid;
  grid-template-columns:repeat(2,1fr);
  gap:14px;
}
.experience-card{
  padding:21px;
  background:var(--surface);
  border:1px solid var(--border);
  border-radius:7px;
}
.experience-card h3{font-size:15px;margin-bottom:5px}
.experience-card p{color:var(--muted);font-size:13px}

.full-portfolio{
  background:
    linear-gradient(135deg,rgba(101,230,181,.07),transparent 60%),
    var(--surface);
  border:1px solid #30443c;
  border-radius:10px;
  padding:54px 30px;
  text-align:center;
}
.full-portfolio h2{
  font-size:34px;
  line-height:1.15;
  margin:12px 0;
}
.full-portfolio p{
  max-width:680px;
  margin:0 auto 26px;
  color:var(--muted);
}

footer{
  padding:55px 0 70px;
  text-align:center;
  color:var(--dim);
  font:400 10px var(--mono);
}
.footer-links{margin-top:14px}
.footer-links a{
  color:var(--muted);
  text-decoration:none;
  margin:0 9px;
}
.footer-links a:hover{color:var(--accent)}

@media(max-width:850px){
  nav ul{display:none}
  .about-grid,.services,.projects,.experience{grid-template-columns:1fr}
  .hero h1{font-size:clamp(42px,12vw,65px)}
}
@media(max-width:560px){
  .container{padding:0 21px}
  .nav-inner{padding:14px 21px}
  section{padding:72px 0}
  .hero-content{padding:125px 0 80px}
  .hero-sub{font-size:16px}
  .section-title{font-size:29px}
  .feedback{padding:24px}
}
</style>
</head>

<body>

<nav>
  <div class="nav-inner">
    <a class="logo" href="#top">MICHELLE / PORTFOLIO</a>
    <ul>
      <li><a href="#about">About</a></li>
      <li><a href="#services">Services</a></li>
      <li><a href="#projects">Work</a></li>
      <li><a href="#feedback">Feedback</a></li>
    </ul>
    <a class="nav-contact" href="mailto:sanchezmitch77@gmail.com">Contact</a>
  </div>
</nav>

<main id="top">

  <!-- LANDING PAGE -->
  <header class="hero">
    <div class="container">
      <div class="hero-content">
        <div class="eyebrow">Automation · Reporting · Operations</div>

        <h1>
          Better Processes.<br>
          Clearer Reporting.<br>
          <span>Less Manual Work.</span>
        </h1>

        <p class="hero-sub">
          Automation, reporting, and operations solutions built to turn
          repetitive processes and scattered data into reliable, usable systems.
        </p>

        <div class="actions">
          <a class="btn btn-primary" href="#projects">View Featured Work →</a>
          <a class="btn btn-secondary" href="mailto:sanchezmitch77@gmail.com">Work With Me →</a>
        </div>
      </div>
    </div>
  </header>

  <!-- ABOUT -->
  <section id="about">
    <div class="container">
      <div class="section-label">01 / About</div>
      <h2 class="section-title">Built around the business problem.</h2>

      <div class="about-grid">
        <div class="about-copy">
          <p>
            Strong systems start with understanding how the work actually moves.
            The focus is on finding where information gets stuck, where manual
            work creates unnecessary effort, and where reporting becomes difficult
            to trust.
          </p>

          <p>
            Experience across marketing agencies, high-ticket sales operations, real estate, finance, e-commerce, research, reporting, and automation brings together the revenue, operational, and technical sides of a business.
          </p>
        </div>

        <div class="process">
          <div class="process-item">
            <strong>Understand</strong>
            <small>Map the process and identify the real bottleneck.</small>
          </div>
          <div class="process-item">
            <strong>Organize</strong>
            <small>Create a reliable structure and source of truth.</small>
          </div>
          <div class="process-item">
            <strong>Improve</strong>
            <small>Remove unnecessary steps and friction.</small>
          </div>
          <div class="process-item">
            <strong>Automate</strong>
            <small>Reduce repetitive work where automation makes sense.</small>
          </div>
          <div class="process-item">
            <strong>Measure</strong>
            <small>Make the output visible through useful reporting.</small>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- SERVICES -->
  <section id="services">
    <div class="container">
      <div class="section-label">02 / What Gets Delivered</div>
      <h2 class="section-title">Services built around the output.</h2>

      <p class="section-intro">
        The tools are only part of the work. The focus is on what the business
        can actually use when the project is finished.
      </p>

      <div class="services">

        <article class="service">
          <h3>Workflow Automation</h3>
          <p>
            Connected workflows that reduce repetitive manual steps and move
            information between systems more efficiently.
          </p>
          <div class="output">Output → Working, repeatable workflow</div>
        </article>

        <article class="service">
          <h3>Reporting & Dashboards</h3>
          <p>
            Structured reporting systems that turn raw business data into
            clear operational and performance visibility.
          </p>
          <div class="output">Output → Reliable reporting layer</div>
        </article>

        <article class="service">
          <h3>Finance & Operations</h3>
          <p>
            Organized trackers, payment workflows, AR monitoring, and
            operational reporting that make financial processes easier to manage.
          </p>
          <div class="output">Output → Centralized operational visibility</div>
        </article>

        <article class="service">
          <h3>AI-Assisted Operations</h3>
          <p>
            AI-supported workflows for research, documentation, data processing,
            and repetitive operational tasks.
          </p>
          <div class="output">Output → Faster, more structured execution</div>
        </article>

      </div>
    </div>
  </section>

  <!-- FEATURED PROJECTS -->
  <section id="projects">
    <div class="container">
      <div class="section-label">03 / Featured Projects</div>
      <h2 class="section-title">Selected work. Practical solutions.</h2>

      <p class="section-intro">
        Three projects that show how automation, reporting, and finance
        operations can work together to create usable business systems.
      </p>

      <div class="projects">

        <article class="project">
          <div class="project-number">01 / BUSINESS AUTOMATION</div>
          <h3>Lead Operations Management System</h3>

          <div class="label">Problem</div>
          <p>
            A 8-stage lead coordination process depended on multiple
            spreadsheets and manual updates, making progress difficult to monitor.
          </p>

          <div class="label">Output</div>
          <p>
            Centralized workflow with lead intake, approval, unique IDs,
            Drive folders, coordinator workspace, stage progression,
            master tracking, and live dashboard.
          </p>

          <div class="label">Result</div>
          <p class="result">
            A standardized workflow with one source of truth and real-time
            operational visibility.
          </p>

          <a class="project-link"
             href="https://github.com/mitchsanchez29/business-automation"
             target="_blank" rel="noopener">
            View project →
          </a>
        </article>

        <article class="project">
          <div class="project-number">02 / REPORTING</div>
          <h3>Client Reporting Management System</h3>

          <div class="label">Problem</div>
          <p>
            Weekly client reporting was tracked manually, making it easy to
            miss reports and lose visibility into reporting history.
          </p>

          <div class="label">Output</div>
          <p>
            Client overview, weekly report queue, status tracking, automated
            report logs, reporting history, and analytics dashboard.
          </p>

          <div class="label">Result</div>
          <p class="result">
            A repeatable reporting process with a clear audit trail and
            less manual tracking.
          </p>

          <a class="project-link"
             href="https://github.com/mitchsanchez29/reporting-analytics"
             target="_blank" rel="noopener">
            View project →
          </a>
        </article>

        <article class="project">
          <div class="project-number">03 / FINANCE OPERATIONS</div>
          <h3>Upcoming & Delayed Payments Tracker</h3>

          <div class="label">Problem</div>
          <p>
            Payment data across spreadsheets required manual checking to
            identify upcoming and overdue accounts.
          </p>

          <div class="label">Output</div>
          <p>
            Automated aging logic, upcoming and delayed trackers, overdue
            alerts, and management dashboards.
          </p>

          <div class="label">Result</div>
          <p class="result">
            Better cash-flow visibility and faster follow-up without manually
            cross-checking spreadsheets.
          </p>

          <a class="project-link"
             href="https://github.com/mitchsanchez29/finance-operations"
             target="_blank" rel="noopener">
            View project →
          </a>
        </article>

      </div>
    </div>
  </section>

  <!-- CLIENT FEEDBACK -->
  <section id="feedback">
    <div class="container">
      <div class="section-label">04 / Client Feedback</div>
      <h2 class="section-title">What clients say.</h2>
      <p class="section-intro">
        Real feedback from clients across different projects and platforms.
      </p>

      <div class="feedback-grid">
Upwork Client
“Great work! Will be having Michelle do more work for us when we can.”

Upwork Client
5.0 — Data Extraction / eBay Information Collection/Data Entry

OLJ Client
“We had a great experience working with Michelle. She performed her tasks efficiently and promptly and were very happy with her performance.”

OLJ Client
“We’re thankful for employees like you that are putting in the hard work to move our company forward.”
     
      </div>
    </div>
  </section>

  <!-- FULL PORTFOLIO -->
  <section id="portfolio">
    <div class="container">
      <div class="full-portfolio">
        <div class="section-label">06 / Full Portfolio</div>

        <h2>See the work behind the results.</h2>

        <p>
          Explore the full collection of automation, reporting, analytics,
          and finance operations projects, including workflows, documentation,
          screenshots, and implementation details.
        </p>

        <a class="btn btn-primary"
           href="https://github.com/mitchsanchez29"
           target="_blank" rel="noopener">
          View Full Portfolio on GitHub →
        </a>
      </div>
    </div>
  </section>

</main>

<footer>
  MICHELLE SANCHEZ · AUTOMATION, REPORTING & OPERATIONS

  <div class="footer-links">
    <a href="https://github.com/mitchsanchez29" target="_blank" rel="noopener">GitHub</a>
    <a href="https://www.linkedin.com/in/michelle29/" target="_blank" rel="noopener">LinkedIn</a>
    <a href="mailto:sanchezmitch77@gmail.com">Email</a>
  </div>
</footer>

</body>
</html>
