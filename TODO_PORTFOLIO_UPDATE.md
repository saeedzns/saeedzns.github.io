# TODO: Redesign Saeed Zohoorian GitHub Pages Portfolio Theme

## Purpose

Update the current `saeedzns.github.io` portfolio into a modern, eye-catching, recruiter-friendly personal website.

The theme should be a custom mix of:

1. Strong visual impact
2. Recruiter-friendly project structure
3. AI / ML / Data Engineering / Computer Vision positioning

Do not copy any external website directly. Build an original theme using the design system below.

---

## Target Recruiter Audience

The page should appeal to recruiters hiring for:

- Data Analyst
- Data Scientist
- Junior Data Engineer
- Analytics Engineer
- Computer Vision Engineer
- Applied Machine Learning Engineer
- AI Automation / Agentic AI roles

The first screen must make Saeed look like a practical data/AI candidate, not only a student with academic projects.

---

## Core Positioning

Use this main positioning:

```html
<p class="subtitle">
  Data Science graduate from Sapienza University building data-driven systems across BI automation, data engineering, applied machine learning, computer vision, and AI-powered workflows.
</p>
```

Use this short headline:

```html
<h2>
  Building data-driven systems from BI dashboards and data pipelines to computer vision and AI-powered automation.
</h2>
```

Avoid weak language:

- Computer Vision Enthusiast
- Student projects
- Simple demos
- Learning projects
- Trying to build

Prefer stronger, honest language:

- Data-driven systems
- BI automation
- Data pipelines
- Applied machine learning
- Computer vision
- AI-powered automation
- Reproducible projects
- Deployed demos
- Reporting workflows
- Dashboard development

---

## Overall Page Structure

Use this structure:

```text
Sticky navbar
↓
Large hero section
↓
Metrics / highlights row
↓
About section
↓
Skills section
↓
Featured projects
↓
Experience snapshot
↓
Contact / footer
```

Required nav items:

```text
About
Skills
Projects
Experience
CV
Contact
```

---

## 1. Create / Update Global CSS Theme

Use a modern dark technical theme.

Add these CSS variables:

```css
:root {
  --bg: #0f172a;
  --bg-soft: #111827;
  --card: rgba(30, 41, 59, 0.72);
  --card-hover: rgba(51, 65, 85, 0.84);
  --text: #f8fafc;
  --muted: #cbd5e1;
  --muted-2: #94a3b8;
  --accent: #38bdf8;
  --accent-2: #818cf8;
  --accent-3: #22d3ee;
  --border: rgba(148, 163, 184, 0.25);
}
```

Use this body styling:

```css
body {
  margin: 0;
  font-family: Inter, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  background:
    radial-gradient(circle at 10% 10%, rgba(56, 189, 248, 0.18), transparent 30rem),
    radial-gradient(circle at 90% 5%, rgba(129, 140, 248, 0.20), transparent 28rem),
    radial-gradient(circle at 50% 100%, rgba(34, 211, 238, 0.10), transparent 30rem),
    var(--bg);
  color: var(--text);
}
```

Design style target:

- dark navy / charcoal background
- cyan-blue and violet accents
- rounded glass-style cards
- subtle gradients
- clean sans-serif typography
- good whitespace
- mobile responsive layout

---

## 2. Add Sticky Navbar

Use this HTML:

```html
<nav class="site-nav">
  <div class="site-nav-inner">
    <a class="brand" href="#">Saeed Zohoorian</a>
    <div class="nav-links">
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#experience">Experience</a>
      <a href="assets/Saeed_Zohoorian_CV.pdf" target="_blank">CV</a>
      <a href="mailto:zns1992@gmail.com">Contact</a>
    </div>
  </div>
</nav>
```

Use this CSS:

```css
.site-nav {
  position: sticky;
  top: 0;
  z-index: 20;
  backdrop-filter: blur(14px);
  background: rgba(15, 23, 42, 0.72);
  border-bottom: 1px solid var(--border);
}

.site-nav-inner {
  max-width: 1180px;
  margin: 0 auto;
  padding: 0.85rem 1.5rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.brand {
  color: var(--text);
  font-weight: 800;
  text-decoration: none;
}

.site-nav a {
  color: var(--muted);
  text-decoration: none;
  font-weight: 600;
  margin-left: 1rem;
}

.site-nav a:hover {
  color: var(--accent);
}
```

---

## 3. Build Strong Hero Section

Use this HTML:

```html
<section class="hero">
  <div class="hero-content">
    <p class="eyebrow">Sapienza Data Science Graduate · Rome, Italy</p>

    <h1>Saeed Zohoorian</h1>

    <p class="subtitle">
      Data Science graduate from Sapienza University building data-driven systems across BI automation, data engineering, applied machine learning, computer vision, and AI-powered workflows.
    </p>

    <h2>
      Building data-driven systems from BI dashboards and data pipelines to computer vision and AI-powered automation.
    </h2>

    <div class="cta-row">
      <a class="btn primary" href="https://github.com/saeedzns" target="_blank">GitHub</a>
      <a class="btn" href="https://linkedin.com/in/saeed-zohoorian-631a80158" target="_blank">LinkedIn</a>
      <a class="btn" href="assets/Saeed_Zohoorian_CV.pdf" target="_blank">Download CV</a>
      <a class="btn" href="mailto:zns1992@gmail.com">Email</a>
    </div>
  </div>
</section>
```

Use this CSS:

```css
.hero {
  min-height: 88vh;
  display: flex;
  align-items: center;
  max-width: 1180px;
  margin: 0 auto;
  padding: 5rem 1.5rem 3rem;
}

.hero-content {
  max-width: 980px;
}

.eyebrow {
  color: var(--accent);
  font-weight: 700;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  font-size: 0.85rem;
}

.hero h1 {
  font-size: clamp(3rem, 8vw, 6.5rem);
  line-height: 0.95;
  margin: 0.5rem 0 1rem;
  letter-spacing: -0.06em;
}

.subtitle {
  max-width: 900px;
  color: var(--muted);
  font-size: clamp(1rem, 2vw, 1.25rem);
  line-height: 1.7;
}

.hero h2 {
  max-width: 850px;
  margin-top: 1.5rem;
  font-size: clamp(1.8rem, 4vw, 3.4rem);
  line-height: 1.08;
  letter-spacing: -0.04em;
}
```

---

## 4. Add CTA Button Styling

Use this CSS:

```css
.cta-row {
  display: flex;
  flex-wrap: wrap;
  gap: 0.85rem;
  margin-top: 2rem;
}

.btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  border-radius: 999px;
  padding: 0.85rem 1.2rem;
  border: 1px solid var(--border);
  color: var(--text);
  text-decoration: none;
  font-weight: 700;
  background: rgba(15, 23, 42, 0.42);
  backdrop-filter: blur(10px);
}

.btn:hover {
  border-color: var(--accent);
  color: var(--accent);
  transform: translateY(-2px);
}

.btn.primary {
  background: linear-gradient(135deg, var(--accent), var(--accent-2));
  color: #020617;
  border-color: transparent;
}
```

---

## 5. Add Metrics / Highlights Row

Place this after the hero section:

```html
<div class="highlights-row">
  <div class="highlight-item">
    <strong>1+ year</strong>
    <span>Professional data analysis experience</span>
  </div>

  <div class="highlight-item">
    <strong>20%</strong>
    <span>Reporting workload reduction</span>
  </div>

  <div class="highlight-item">
    <strong>3+</strong>
    <span>Live ML/data demos deployed</span>
  </div>

  <div class="highlight-item">
    <strong>MSc</strong>
    <span>Data Science, Sapienza University</span>
  </div>
</div>
```

Use this CSS:

```css
.highlights-row {
  max-width: 1180px;
  margin: -2rem auto 2rem;
  padding: 0 1.5rem;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(190px, 1fr));
  gap: 1rem;
}

.highlight-item strong {
  display: block;
  font-size: 1.7rem;
  color: var(--accent);
  margin-bottom: 0.4rem;
}

.highlight-item span {
  color: var(--muted);
}
```

---

## 6. Rewrite About Section

Use this exact text:

```html
<section id="about" class="section">
  <h2>About</h2>

  <p class="section-intro">
    I am a Sapienza University Data Science graduate based in Rome, with Data Analyst experience at Allianz Trade. My work combines BI automation, reporting pipelines, dashboard development, and data-driven decision support using Python, SQL, Power BI, Excel, VBA, IBM Impromptu, and Microsoft Access.
  </p>

  <p class="section-intro">
    I build practical data systems across data analysis, data engineering foundations, applied machine learning, computer vision, and AI-powered automation. My portfolio includes deployed demos and reproducible projects in Bayesian modeling, NLP, information retrieval, and egocentric computer vision.
  </p>
</section>
```

---

## 7. Add Skills Section

Use six skill cards:

```html
<section id="skills" class="section">
  <h2>Skills</h2>
  <p class="section-intro">
    Technical skills grouped around the roles I target: data analysis, data science, data engineering, computer vision, and AI-powered workflows.
  </p>

  <div class="skill-grid">

    <div class="skill-card">
      <h3>Data Analysis & BI</h3>
      <p>Power BI, Excel, VBA, IBM Cognos Impromptu, Microsoft Access, dashboard development, reporting automation, business data analysis.</p>
    </div>

    <div class="skill-card">
      <h3>Data Engineering & Databases</h3>
      <p>SQL, PostgreSQL, PySpark, Neo4j, data cleaning, data preprocessing, web scraping, structured datasets, reproducible data pipelines.</p>
    </div>

    <div class="skill-card">
      <h3>Machine Learning & Statistics</h3>
      <p>Python, Scikit-learn, model evaluation, classification, regression, Bayesian inference, ordinal regression, probabilistic modeling, model calibration.</p>
    </div>

    <div class="skill-card">
      <h3>Computer Vision & Deep Learning</h3>
      <p>PyTorch, TensorFlow, Keras, image classification, object detection, semantic segmentation, egocentric vision, CNNs, transfer learning.</p>
    </div>

    <div class="skill-card">
      <h3>NLP & Information Retrieval</h3>
      <p>JAX, autoregressive modeling, text generation, TF-IDF, search engines, ranking, text processing, information retrieval.</p>
    </div>

    <div class="skill-card">
      <h3>AI Workflows & Deployment</h3>
      <p>Streamlit, Gradio, Hugging Face Spaces, GitHub Pages, Git, GitHub, Jupyter, Google Colab, AWS, AI-powered workflow automation.</p>
    </div>

  </div>
</section>
```

Do not claim Airflow, Kafka, dbt, Docker, Kubernetes, or cloud data warehouses unless those are actually added later.

---

## 8. Use Consistent Card Design

Apply this CSS to skills, projects, experience, and highlight cards:

```css
.skill-card,
.project-card,
.experience-card,
.highlight-item {
  border: 1px solid var(--border);
  background: linear-gradient(
    180deg,
    rgba(30, 41, 59, 0.82),
    rgba(15, 23, 42, 0.74)
  );
  border-radius: 22px;
  padding: 1.4rem;
  box-shadow: 0 24px 70px rgba(2, 6, 23, 0.28);
  backdrop-filter: blur(12px);
}

.skill-card:hover,
.project-card:hover {
  transform: translateY(-4px);
  border-color: rgba(56, 189, 248, 0.55);
  background: var(--card-hover);
  transition: 0.22s ease;
}
```

Use this layout CSS:

```css
.section {
  max-width: 1180px;
  margin: 0 auto;
  padding: 4.5rem 1.5rem;
}

.section h2 {
  font-size: clamp(2rem, 4vw, 3rem);
  margin-bottom: 1rem;
  letter-spacing: -0.04em;
}

.section-intro {
  max-width: 760px;
  color: var(--muted);
  line-height: 1.7;
  margin-bottom: 2rem;
}

.skill-grid,
.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1.25rem;
}
```

---

## 9. Improve Project Card Structure

Every featured project must include:

- Project name
- Project tag
- Problem
- Impact/result
- Tech stack
- GitHub button
- Live Demo button

Use this pattern:

```html
<div class="project-card">
  <div class="project-tag">Category · Type</div>

  <h3>Project Name</h3>

  <p class="project-problem">
    Short explanation of the problem and why it matters.
  </p>

  <p class="project-impact">
    Short explanation of what was built or achieved.
  </p>

  <p class="tech-stack">
    Python · SQL · Streamlit · etc.
  </p>

  <div class="project-links">
    <a href="GITHUB_LINK" target="_blank">GitHub</a>
    <a href="LIVE_DEMO_LINK" target="_blank">Live Demo</a>
  </div>
</div>
```

Use this CSS:

```css
.project-tag {
  display: inline-flex;
  width: fit-content;
  padding: 0.35rem 0.7rem;
  border-radius: 999px;
  background: rgba(56, 189, 248, 0.12);
  color: var(--accent);
  font-size: 0.8rem;
  font-weight: 700;
  margin-bottom: 1rem;
}

.project-card h3 {
  font-size: 1.35rem;
  margin: 0 0 0.75rem;
}

.project-problem,
.project-impact,
.tech-stack {
  color: var(--muted);
  line-height: 1.6;
}

.tech-stack {
  font-size: 0.9rem;
  color: var(--muted-2);
}

.project-links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.75rem;
  margin-top: 1rem;
}

.project-links a {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  border-radius: 999px;
  padding: 0.7rem 1rem;
  border: 1px solid var(--border);
  color: var(--text);
  text-decoration: none;
  font-weight: 700;
}

.project-links a:hover {
  border-color: var(--accent);
  color: var(--accent);
}
```

---

## 10. Featured Projects Order

The first featured projects must be:

1. Ego4D-LiteSTA
2. Bayesian Ordinal Regression
3. ADM_HW3 Book Search Engine
4. Dialog Autoregressive Modeling RNN

Older academic projects can appear lower as “Additional Academic Projects”.

---

## 11. Ego4D Project Card

Use this:

```html
<div class="project-card">
  <div class="project-tag">Computer Vision · Thesis</div>

  <h3>Ego4D-LiteSTA</h3>

  <p class="project-problem">
    Lightweight computer vision pipeline for egocentric interaction anticipation.
  </p>

  <p class="project-impact">
    Predicts interaction object, action, and time-to-contact using a three-track design focused on speed and accuracy retention.
  </p>

  <p class="tech-stack">
    Python · PyTorch · Computer Vision · Object Detection · Egocentric Vision · Gradio · Hugging Face Spaces
  </p>

  <div class="project-links">
    <a href="https://github.com/saeedzns/Ego4d-LiteSTA" target="_blank">GitHub</a>
    <a href="YOUR_EGO4D_HUGGING_FACE_LINK" target="_blank">Live Demo</a>
  </div>
</div>
```

Replace `YOUR_EGO4D_HUGGING_FACE_LINK`.

---

## 12. Bayesian Project Card

Use this:

```html
<div class="project-card">
  <div class="project-tag">Statistical Modeling · Deployed Demo</div>

  <h3>Bayesian Ordinal Regression</h3>

  <p class="project-problem">
    Statistical modeling project for obesity-level prediction using ordinal outcome categories.
  </p>

  <p class="project-impact">
    Compared proportional odds and partial proportional odds approaches with focus on calibration, interpretability, and model fit.
  </p>

  <p class="tech-stack">
    R/Python · Bayesian Inference · Ordinal Regression · Statistical Modeling · Streamlit
  </p>

  <div class="project-links">
    <a href="https://github.com/saeedzns/Bayesian-Ordinal-Regression-for-Obesity-Level-Prediction" target="_blank">GitHub</a>
    <a href="YOUR_BAYESIAN_STREAMLIT_LINK" target="_blank">Live Demo</a>
  </div>
</div>
```

Replace `YOUR_BAYESIAN_STREAMLIT_LINK`.

---

## 13. ADM_HW3 Project Card

Use this:

```html
<div class="project-card">
  <div class="project-tag">Information Retrieval · Search Demo</div>

  <h3>ADM_HW3 Book Search Engine</h3>

  <p class="project-problem">
    Information retrieval project for searching and ranking book-related content.
  </p>

  <p class="project-impact">
    Built indexing, text processing, TF-IDF scoring, and an interactive Streamlit search interface.
  </p>

  <p class="tech-stack">
    Python · Information Retrieval · TF-IDF · Search Engine · Data Processing · Streamlit
  </p>

  <div class="project-links">
    <a href="https://github.com/saeedzns/ADM_HW3" target="_blank">GitHub</a>
    <a href="YOUR_ADM_HW3_STREAMLIT_LINK" target="_blank">Live Demo</a>
  </div>
</div>
```

Replace `YOUR_ADM_HW3_STREAMLIT_LINK`.

---

## 14. Dialog RNN Project Card

Use this:

```html
<div class="project-card">
  <div class="project-tag">NLP · JAX</div>

  <h3>Dialog Autoregressive Modeling RNN</h3>

  <p class="project-problem">
    Character-level language modeling project using dialogue data.
  </p>

  <p class="project-impact">
    Implemented a minimal JAX-based RNN for autoregressive text generation with clean and reproducible code.
  </p>

  <p class="tech-stack">
    Python · JAX · NLP · RNN · Autoregressive Modeling · Google Colab
  </p>

  <div class="project-links">
    <a href="https://github.com/saeedzns/Dialog-Autoregressive-Modeling-RNN" target="_blank">GitHub</a>
  </div>
</div>
```

---

## 15. Add Experience Snapshot Section

Use this:

```html
<section id="experience" class="section">
  <h2>Experience Snapshot</h2>
  <p class="section-intro">
    Professional experience in data analysis, BI automation, reporting workflows, and business decision support.
  </p>

  <div class="experience-card">
    <h3>Data Analyst · Allianz Trade</h3>
    <p class="meta">Rome, Italy · May 2023 – Apr 2024</p>
    <ul>
      <li>Built dashboards, reports, and automated workflows using Python, SQL, Power BI, Excel, VBA, IBM Impromptu, and Microsoft Access.</li>
      <li>Reduced reporting workload through reusable reports and workflow automation.</li>
      <li>Supported international data and reporting needs across Middle East, Europe, and Africa business contexts.</li>
    </ul>
  </div>

  <div class="experience-card">
    <h3>Data Analyst · Rasoul</h3>
    <p class="meta">Tehran, Iran · Apr 2015 – Apr 2018</p>
    <ul>
      <li>Collected and analyzed trade and customer data from multiple electronics stores.</li>
      <li>Prepared Excel-based business analysis from accounting software data to support decision-making.</li>
    </ul>
  </div>
</section>
```

CSS:

```css
.experience-card {
  margin-bottom: 1rem;
}

.experience-card h3 {
  margin-top: 0;
}

.meta {
  color: var(--muted-2);
  font-size: 0.92rem;
}

.experience-card li {
  color: var(--muted);
  line-height: 1.6;
  margin-bottom: 0.4rem;
}
```

---

## 16. Add Footer

Use this:

```html
<footer class="footer">
  <p>© 2026 Saeed Zohoorian · Data Science · BI Automation · Computer Vision · AI Workflows</p>
  <div>
    <a href="https://github.com/saeedzns" target="_blank">GitHub</a>
    <a href="https://linkedin.com/in/saeed-zohoorian-631a80158" target="_blank">LinkedIn</a>
    <a href="mailto:zns1992@gmail.com">Email</a>
  </div>
</footer>
```

CSS:

```css
.footer {
  max-width: 1180px;
  margin: 0 auto;
  padding: 3rem 1.5rem;
  border-top: 1px solid var(--border);
  color: var(--muted-2);
  display: flex;
  justify-content: space-between;
  gap: 1rem;
  flex-wrap: wrap;
}

.footer a {
  color: var(--muted);
  text-decoration: none;
  margin-left: 1rem;
}

.footer a:hover {
  color: var(--accent);
}
```

---

## 17. Mobile Responsiveness

Add this CSS:

```css
@media (max-width: 760px) {
  .hero {
    min-height: auto;
    padding-top: 4rem;
  }

  .hero h1 {
    font-size: clamp(2.8rem, 15vw, 4rem);
  }

  .cta-row,
  .project-links {
    flex-direction: column;
  }

  .btn,
  .project-links a {
    width: 100%;
  }

  .site-nav-inner {
    align-items: flex-start;
    gap: 0.75rem;
    flex-direction: column;
  }

  .site-nav a {
    margin-left: 0;
    margin-right: 1rem;
  }

  .nav-links {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
  }
}
```

Check for no horizontal scrolling on mobile.

---

## 18. Final Link Checks

Before committing, check:

- GitHub button opens: `https://github.com/saeedzns`
- LinkedIn button opens: `https://linkedin.com/in/saeed-zohoorian-631a80158`
- Email button opens: `mailto:zns1992@gmail.com`
- CV button opens: `assets/Saeed_Zohoorian_CV.pdf`
- Ego4D GitHub link works
- Ego4D Hugging Face demo link works
- Bayesian GitHub link works
- Bayesian Streamlit demo link works
- ADM_HW3 GitHub link works
- ADM_HW3 Streamlit demo link works
- No placeholder links remain
- No `YOUR_LINK`, `TODO`, or `#` placeholders remain unless intentionally used for top-of-page brand link

---

## 19. Spelling Checks

Check these words carefully:

- recruiter
- engineering
- Sapienza
- statistical
- automation
- information retrieval
- Hugging Face
- Streamlit
- Bayesian
- egocentric

---

## 20. Commit Changes

Use:

```bash
git add index.html style.css assets/
git commit -m "Redesign portfolio theme for recruiter positioning"
git push
```

---

## Final Design Target

The final website should feel like:

```text
Modern dark technical portfolio
+ recruiter-friendly project structure
+ AI/data engineering/computer vision positioning
+ clean professional credibility
```

The page should communicate:

> Saeed Zohoorian is a Sapienza Data Science graduate with practical experience in data analysis, BI automation, reporting pipelines, data engineering foundations, applied ML, computer vision, and AI-powered workflows.

Do not make it look like a colorful student page.

Do not make it too minimal.

Make it look like a serious junior data scientist / data analyst / ML engineer portfolio.
