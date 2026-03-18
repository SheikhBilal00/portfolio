# portfolio
My AI/ML Engineer Portfolio 
# ⚡ SHEIKH BILAL AHMAD — Cyberpunk Portfolio

> Live Site → [SheikhBilal00.github.io/portfolio](https://SheikhBilal00.github.io/portfolio)

A high-performance, single-file cyberpunk portfolio built for an AI/ML Engineer. Features a reactive 3D Neural Core, generative ambient music, glitch effects, and a full professional profile — all in one `index.html` with zero dependencies to install.

## ✨ Features

### 🎨 Visual
- **Cyberpunk Noir** aesthetic — neon cyan, magenta, yellow on deep dark background
- **3D Neural Core** — live deforming sphere that tracks mouse movement and pulses
- **Orbiting particle rings** with neon glow
- **Background star field** that responds to scrolling (camera flight effect)
- **Scanlines + grid overlay** for authentic CRT feel
- **Random glitch bursts** across the page
- **Custom cursor** with lag-follow and hover reactions

### 🔤 Typography & Animation
- **Glitch hover effect** on all major headings — cyan/magenta ghost layers shift on hover
- **Idle glitch** on the main name — triggers automatically every ~5 seconds
- **Scramble text decoder** on project names — re-triggers on hover
- **Scroll reveal** animations on every section
- **Animated skill bars** that fill on scroll into view
- **Stats counter** that counts up when visible
- **Scrolling tech ticker** across the full width
- **Boot sequence** with sequential loading messages

### 🎵 Generative Music
- 4 cyberpunk ambient tracks synthesized live in the browser (Web Audio API)
- No external audio files — music is generated mathematically, zero download cost
- Music player widget (bottom-right) with animated EQ bars, track switcher, volume slider
- Opt-in prompt** on boot screen — visitors choose to enable or skip audio

| Track | Style | BPM |
|---|---|---|
| `NEURAL_AMBIENT_01` | Deep drone pads + soft arpeggio | 75 |
| `CYBER_NOIR_02` | Dark jazz-noir tones + bass | 90 |
| `DATA_PULSE_03` | Driving pulse with percussion | 110 |
| `VOID_SIGNAL_04` | Slow atmospheric void | 60 |

### 📄 Sections
- Hero — Name, role, key achievements, CTA buttons
- Stats Bar — Animated counters (models deployed, accuracy, requests, etc.)
- Experience — Timeline layout with ONGC & Robotic Technologies
- Projects — Customer Churn Prediction, NLP Sentiment Analyzer, OCR Text Extractor
- Skills — Categorized bars across ML/AI, Data Engineering, Cloud, Full-Stack
- Certifications — AWS, TensorFlow, Deep Learning, BERT, PySpark + SIH 2023
- Terminal — Hacker-style identity dump with blinking cursor
- Contact — Links + live message form with transmission animation

---

## 🛠️ Tech Stack

 Layer                          Technology 

Structure               HTML5 (single file) 
Styling                 CSS3 with custom properties 
3D Engine               Three.js r128 (via CDN) 
Animations              CSS keyframes + Vanilla JS 
Music                   Web Audio API (generative, no files) 
Fonts                   Google Fonts — Orbitron, Share Tech Mono, Rajdhani 
Deployment              GitHub Pages 

> No build tool. No npm. No framework. Just one file.


## 🚀 Deployment

This portfolio is deployed via GitHub Pages.

To deploy your own fork:

1. Fork this repository
2. Go to Settings → Pages
3. Set source to `main` branch, `/ (root)` folder
4. Click Save
5. Live at `https://yourusername.github.io/portfolio`

---

## ✏️ How to Customize

Everything is in `index.html`. Open it in any text editor and use Ctrl+F to find sections.

### Change Colors
Find the `:root` block at the top of the `<style>` tag:

```css
:root {
  --c:   #00fff5;   /* cyan  — primary accent    */
  --m:   #ff2d78;   /* magenta — secondary accent */
  --y:   #ffe600;   /* yellow — metrics/numbers   */
  --g:   #00ff41;   /* green — status indicators  */
  --bg:  #020509;   /* page background            */
  --txt: #e8f8ff;   /* main text color            */
}
```

Changing any of these cascades through the **entire site instantly**.

### Add a New Job

Find the `exp-list` div and copy-paste this block:

```html
<div class="exp-item rv">
  <div class="exp-date">
    <div class="yr">MON YEAR</div>
    <div>— PRESENT</div>
    <div class="badge">● ACTIVE</div>
  </div>
  <div class="exp-content">
    <div class="exp-company glitch-el" data-g="COMPANY NAME">COMPANY NAME</div>
    <div class="exp-role">YOUR ROLE · LOCATION</div>
    <div class="exp-bullets">
      <div class="exp-bullet">Your achievement here with <b>metric</b>.</div>
      <div class="exp-bullet">Another bullet point here.</div>
    </div>
  </div>
</div>
```

### Add a New Project

Find the `proj-grid` div and copy-paste:

```html
<div class="proj-card rv">
  <div class="proj-hover-bg"></div>
  <div class="proj-id">// PROJECT_ID: 004 · CATEGORY</div>
  <div class="proj-stack"><b>Tech · Stack · Here</b></div>
  <div class="proj-name glitch-el" data-sc="PROJECT NAME" data-g="PROJECT NAME">PROJECT NAME</div>
  <p class="proj-desc">Your project description here.</p>
  <div class="proj-metrics">
    <span class="metric">KEY METRIC</span>
  </div>
  <div class="proj-tags">
    <span class="ptag c">TAG</span>
  </div>
  <a href="https://github.com/yourusername/repo" target="_blank" class="proj-link">GITHUB_REPOSITORY</a>
</div>
```

### Add a New Skill

Find the `skills-wrap` div and copy-paste inside a `skill-category`:

```html
<div class="skill-row rv">
  <div class="sk-top">
    <span class="sk-name">SKILL NAME</span>
    <span class="sk-pct">85%</span>
  </div>
  <div class="sk-bar">
    <div class="sk-fill" data-w="85"></div>
  </div>
</div>
```

### Add a New Certification

Find the `certs-grid` div and copy-paste:

```html
<div class="cert-card rv">
  <div class="cert-icon">SHORT<br>CODE</div>
  <div>
    <div class="cert-name">FULL CERTIFICATION NAME</div>
    <div class="cert-by">Issuing Organization</div>
  </div>
</div>
```

### Add Glitch Effect to Any Heading

Add `class="glitch-el"` and `data-g="YOUR TEXT"` to any element:

```html
<span class="glitch-el" data-g="YOUR HEADING">YOUR HEADING</span>
```

For the idle auto-glitch (like the main name), also add `glitch-idle`:

```html
<span class="glitch-el glitch-idle" data-g="YOUR HEADING">YOUR HEADING</span>
```

---

## 📁 File Structure

```
portfolio/
└── index.html        ← Everything. The entire portfolio.
└── README.md         ← This file
```

---

## 👤 About

**Sheikh Bilal Ahmad**
AI/ML Engineer · Full-Stack Developer · Data Scientist

- 📧 sheikhbial000@gmail.com
- 📞 +91 7355767856
- 🔗 [linkedin.com/in/sheikh-bilal-ahmad](https://linkedin.com/in/sheikh-bilal-ahmad)
- 🐙 [github.com/SheikhBilal00](https://github.com/SheikhBilal00)
- 🌐 [arama-web.web.app](https://arama-web.web.app)

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).

Feel free to fork and adapt for your own portfolio — just replace the personal details with your own!

---

<div align="center">

**Built with Three.js · Web Audio API · Pure CSS · No frameworks**

*"Building at the edge of computation and intelligence."*

</div>
