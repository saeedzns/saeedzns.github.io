# TODO: Update Saeed Zohoorian GitHub Pages Portfolio

## Goal

Update the existing `index.html` portfolio page to better match Saeed Zohoorian's CV and current positioning.

The page should present him as:

> Data Scientist with experience in BI automation, data engineering foundations, computer vision, statistical modeling, and applied machine learning.

Avoid weak wording like:

- "Computer Vision Enthusiast"
- "Turning machine learning projects into usable demos"

Use stronger but honest wording based on the CV:

- Data Scientist
- BI Automation
- Data Engineering Foundations
- Computer Vision
- Statistical Modeling
- Applied Machine Learning

---

## 1. Update the hero/title section

Find the current hero text that contains something similar to:

```html
<h1>Saeed Zohoorian</h1>
<p>Data Scientist · Computer Vision Enthusiast · Sapienza Graduate</p>
<p>Turning machine learning projects into usable demos.</p>
```

Replace it with:

```html
<h1>Saeed Zohoorian</h1>

<p class="subtitle">
  Data Scientist · BI Automation · Data Engineering · Computer Vision · Statistical Modeling
</p>

<p class="hero-lead">
  Data Science graduate from Sapienza University with professional experience in data analysis, reporting automation, dashboard development, and applied machine learning.
</p>

<p class="hero-text">
  I build practical data systems using Python, SQL, Power BI, PostgreSQL, PySpark, and machine learning. My work connects business intelligence, data engineering foundations, computer vision, Bayesian modeling, NLP, and search-engine systems.
</p>
```

If the current CSS uses different class names, keep the existing classes and only replace the text.

---

## 2. Add or rewrite the About section

If there is an existing About section, rewrite it as:

```html
<section id="about" class="section">
  <h2>About</h2>
  <p>
    I am a Data Scientist based in Rome with experience as a Data Analyst at Allianz Trade, where I worked with Python, SQL, Power BI, Excel, VBA, IBM Impromptu, and Microsoft Access to automate reporting workflows and support data-driven decisions.
  </p>
  <p>
    My technical focus is applied data science: building reproducible projects, developing dashboards and reporting pipelines, preparing structured data, and deploying interactive demos for machine learning, computer vision, Bayesian modeling, NLP, and information retrieval.
  </p>
</section>
```

Keep this section direct and readable. Do not make it too long.

---

## 3. Add or update a Skills section

Create or update this section:

```html
<section id="skills" class="section">
  <h2>Skills</h2>
  <div class="skill-grid">

    <div class="skill-card">
      <h3>Data Science & Machine Learning</h3>
      <p>Python, Scikit-learn, PyTorch, TensorFlow, Keras, JAX, NumPy, Pandas, model evaluation, classification, regression, NLP, computer vision.</p>
    </div>

    <div class="skill-card">
      <h3>Data Engineering & Databases</h3>
      <p>SQL, PostgreSQL, PySpark, Neo4j, data cleaning, data preprocessing, web scraping, structured datasets, reproducible data pipelines.</p>
    </div>

    <div class="skill-card">
      <h3>BI, Reporting & Automation</h3>
      <p>Power BI, IBM Cognos Impromptu, Excel, VBA, Microsoft Access, automated reporting, dashboard development, workflow optimization.</p>
    </div>

    <div class="skill-card">
      <h3>Computer Vision & Deep Learning</h3>
      <p>Object detection, image classification, semantic segmentation, egocentric vision, CNNs, transfer learning, action anticipation.</p>
    </div>

    <div class="skill-card">
      <h3>Statistical & Probabilistic Modeling</h3>
      <p>Bayesian inference, ordinal regression, probabilistic modeling, model calibration, statistical analysis.</p>
    </div>

    <div class="skill-card">
      <h3>Cloud & Tools</h3>
      <p>AWS, Git, GitHub, Hugging Face Spaces, Streamlit Cloud, Gradio, Jupyter, Google Colab.</p>
    </div>

  </div>
</section>
```

Important: keep the label as **Data Engineering & Databases** or **Data Engineering Foundations**. Do not present Saeed as a full Data Engineer unless more production ETL/orchestration/cloud warehouse projects are added.

---

## 4. Update project ordering

Make sure the strongest projects appear first:

1. Ego4D-LiteSTA
2. Bayesian Ordinal Regression for Obesity Level Prediction
3. ADM_HW3 Book Search Engine
4. Dialog Autoregressive Modeling RNN
5. Other academic projects

Each project card should include:

- short problem description
- tech stack
- GitHub button
- Live Demo button if available
- optional screenshot or GIF

---

## 5. Update Ego4D project card

Use this text:

```html
<h3>Ego4D-LiteSTA</h3>
<p>
  Lightweight three-track computer vision pipeline for egocentric interaction anticipation, predicting interaction object, action, and time-to-contact with reduced latency.
</p>
<p class="tech-stack">
  Python · PyTorch · Computer Vision · Object Detection · Egocentric Vision · Gradio · Hugging Face Spaces
</p>
```

Buttons:

```html
<a href="https://github.com/saeedzns/Ego4d-LiteSTA" target="_blank">GitHub</a>
<a href="YOUR_EGO4D_HUGGING_FACE_LINK" target="_blank">Live Demo</a>
```

Replace `YOUR_EGO4D_HUGGING_FACE_LINK` with the real Hugging Face Space URL.

---

## 6. Update Bayesian project card

Use this text:

```html
<h3>Bayesian Ordinal Regression for Obesity Level Prediction</h3>
<p>
  Statistical modeling project comparing proportional odds and partial proportional odds approaches for obesity category prediction, with focus on calibration, interpretability, and model fit.
</p>
<p class="tech-stack">
  R/Python · Bayesian Inference · Ordinal Regression · Statistical Modeling · Streamlit
</p>
```

Buttons:

```html
<a href="https://github.com/saeedzns/Bayesian-Ordinal-Regression-for-Obesity-Level-Prediction" target="_blank">GitHub</a>
<a href="YOUR_BAYESIAN_STREAMLIT_LINK" target="_blank">Live Demo</a>
```

Replace `YOUR_BAYESIAN_STREAMLIT_LINK` with the real Streamlit URL.

---

## 7. Update ADM_HW3 project card

Use this text:

```html
<h3>ADM_HW3 Book Search Engine</h3>
<p>
  Information retrieval project built around book search, indexing, text processing, and ranking. Converted into an interactive Streamlit demo for querying and exploring results.
</p>
<p class="tech-stack">
  Python · Information Retrieval · TF-IDF · Search Engine · Data Processing · Streamlit
</p>
```

Buttons:

```html
<a href="https://github.com/saeedzns/ADM_HW3" target="_blank">GitHub</a>
<a href="YOUR_ADM_HW3_STREAMLIT_LINK" target="_blank">Live Demo</a>
```

Replace `YOUR_ADM_HW3_STREAMLIT_LINK` with the real Streamlit URL.

---

## 8. Add an Experience Snapshot section

Add this after About or before Projects:

```html
<section id="experience" class="section">
  <h2>Experience Snapshot</h2>

  <div class="experience-card">
    <h3>Data Analyst · Allianz Trade</h3>
    <p class="meta">Rome, Italy · May 2023 – Apr 2024</p>
    <ul>
      <li>Analyzed business data using Python, SQL, Power BI, Excel, VBA, IBM Impromptu, and Microsoft Access.</li>
      <li>Built dashboards and reusable reports to reduce manual work and improve reporting efficiency.</li>
      <li>Supported international reporting needs across Middle East, Europe, and Africa business contexts.</li>
    </ul>
  </div>

  <div class="experience-card">
    <h3>Data Analyst · Rasoul</h3>
    <p class="meta">Tehran, Iran · Apr 2015 – Apr 2018</p>
    <ul>
      <li>Collected and analyzed trade and customer data from multiple electronics stores.</li>
      <li>Prepared Excel-based analysis from accounting software data to support business decisions.</li>
    </ul>
  </div>
</section>
```

---

## 9. Add a Thesis Highlight section

Add this if the page has enough space:

```html
<section id="thesis" class="section">
  <h2>Thesis Highlight</h2>
  <div class="highlight-card">
    <h3>Ego4D-LiteSTA</h3>
    <p>
      A lightweight three-track pipeline for egocentric interaction anticipation, focused on predicting the interaction object, action, and time-to-contact while reducing latency.
    </p>
  </div>
</section>
```

Keep this short. The detailed explanation belongs in the project card, GitHub README, or Hugging Face demo.

---

## 10. Add stronger CTA buttons

In the hero area, make sure there are buttons for:

```html
<a href="https://github.com/saeedzns" target="_blank">GitHub</a>
<a href="https://linkedin.com/in/saeed-zohoorian-631a80158" target="_blank">LinkedIn</a>
<a href="mailto:zns1992@gmail.com">Email</a>
<a href="assets/Saeed_Zohoorian_CV.pdf" target="_blank">Download CV</a>
```

If the CV PDF is not uploaded yet:

1. Create an `assets/` folder.
2. Upload the CV as `Saeed_Zohoorian_CV.pdf`.
3. Use this link:

```html
<a href="assets/Saeed_Zohoorian_CV.pdf" target="_blank">Download CV</a>
```

---

## 11. Improve wording across the page

Search the whole `index.html` and replace weak/generic wording.

Replace:

```text
Computer Vision Enthusiast
```

With:

```text
Computer Vision
```

Replace:

```text
Turning machine learning projects into usable demos.
```

With:

```text
Building practical data systems from dashboards to machine-learning demos.
```

Replace:

```text
I build practical data science, computer vision, Bayesian modeling, and search-engine systems.
```

With:

```text
I build practical data systems across business intelligence, data engineering foundations, machine learning, computer vision, Bayesian modeling, and information retrieval.
```

---

## 12. CSS improvements

If `style.css` exists, add or update styles for skill cards and experience cards.

Use this simple card layout:

```css
.skill-grid,
.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 1.25rem;
}

.skill-card,
.project-card,
.experience-card,
.highlight-card {
  padding: 1.25rem;
  border-radius: 16px;
  border: 1px solid rgba(148, 163, 184, 0.25);
  background: rgba(255, 255, 255, 0.04);
}

.tech-stack,
.meta {
  font-size: 0.9rem;
  opacity: 0.85;
}
```

Do not destroy the existing design. Only improve spacing, readability, and consistency.

---

## 13. Final checks

Before committing:

- Check the page opens locally.
- Check it works on mobile width.
- Check all links work.
- Check there are no placeholder links like `#`, `YOUR_LINK`, or `TODO`.
- Check the project cards are not too long.
- Check Data Engineering is included but not exaggerated.
- Check the hero section immediately tells recruiters what Saeed does.
- Check the "Download CV" button opens the correct PDF.
- Check GitHub, LinkedIn, Streamlit, and Hugging Face links open in new tabs.

---

## 14. Commit changes

Use this commit message:

```bash
git add index.html style.css assets/
git commit -m "Update portfolio positioning and add data engineering skills"
git push
```

---

## Final positioning target

The page should make Saeed look like:

> A Data Scientist with practical experience in data analysis, BI automation, reporting pipelines, data engineering foundations, computer vision, statistical modeling, and deployed ML demos.

Not like:

> A student who only uploaded school projects.
