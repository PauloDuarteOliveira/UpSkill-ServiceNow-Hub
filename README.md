<div align="center">

<img src="docs/banner.png" alt="UpSkill ServiceNow Hub: your learning track, in one place." width="100%">

<br>

<a href="https://pauloduarteoliveira.github.io/UpSkill-ServiceNow-Hub/"><img src="https://img.shields.io/badge/▶_Live_demo-86BC25?style=for-the-badge&logoColor=white" alt="Live demo"></a> <a href="#-screenshots"><img src="https://img.shields.io/badge/Screenshots-1E293B?style=for-the-badge" alt="Screenshots"></a> <a href="#-run-it-locally"><img src="https://img.shields.io/badge/Run_it-1E293B?style=for-the-badge" alt="Run it"></a>

<br><br>

<img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" alt="HTML5">
<img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white" alt="CSS3">
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript">
<img src="https://img.shields.io/badge/frameworks-none-293E40?style=flat-square" alt="No frameworks">
<img src="https://img.shields.io/badge/UPskill-2026-86BC25?style=flat-square" alt="UPskill 2026">

</div>

<br>

> **A learning portal for ServiceNow trainees.** Follow your progress through the track, read the lessons, and try the code in a built-in sandbox, all in hand-written HTML, CSS and JavaScript.

Built as the practice project for the **JavaScript Programming** module of the **UPskill ServiceNow** programme (2026 class): the goal was to put the HTML5, CSS3 and JavaScript fundamentals together in something that looks and works like a real company tool.

## 📸 Screenshots

<p align="center">
  <img src="docs/screenshots/dashboard.png" alt="The dashboard: overall progress, summary cards and the module grid" width="100%">
  <br><sub><b>Dashboard.</b> Overall progress, summary cards, featured modules and the roadmap.</sub>
</p>

<table>
  <tr>
    <td width="50%"><img src="docs/screenshots/lesson-1.png" alt="Lesson 1: syntax, variables and the var / let / const grid"><br><sub><b>Lesson 1.</b> Syntax, variables and a <code>var</code> / <code>let</code> / <code>const</code> comparison.</sub></td>
    <td width="50%"><img src="docs/screenshots/lesson-2.png" alt="Lesson 2: the urgency validator sandbox"><br><sub><b>Lesson 2.</b> The DOM, Client Scripts and the urgency validator sandbox.</sub></td>
  </tr>
  <tr>
    <td><img src="docs/screenshots/dashboard-dark.png" alt="The dashboard in dark mode"><br><sub><b>Dark mode.</b> One tap on the moon icon.</sub></td>
    <td align="center"><img src="docs/screenshots/phone.png" alt="The dashboard on a phone" width="45%"><br><sub><b>On a phone.</b> The layout stacks into one column.</sub></td>
  </tr>
</table>

## ✨ Highlights

<table>
  <tr>
    <td width="33%" valign="top">
      <h3>🏠 Dashboard</h3>
      Progress ring, summary cards, featured and completed modules, and what's next on the roadmap.
    </td>
    <td width="33%" valign="top">
      <h3>📘 Lessons</h3>
      Two lessons on JavaScript for ServiceNow: the basics (variables, scope, logic) and the DOM with Client Scripts (<code>g_form</code>).
    </td>
    <td width="33%" valign="top">
      <h3>🧪 Sandbox</h3>
      Pick a ticket priority and watch the page react: a small, safe place to try dynamic classes.
    </td>
  </tr>
  <tr>
    <td valign="top">
      <h3>🌙 Dark mode</h3>
      The whole workspace switches colours with a single <code>classList.toggle</code>.
    </td>
    <td valign="top">
      <h3>👤 CSS-only menu</h3>
      The profile dropdown opens by click or keyboard with <code>:focus-within</code>, with no JavaScript.
    </td>
    <td valign="top">
      <h3>🧭 Smart cards</h3>
      One card, two destinations: the module or straight to the current lesson, using layered links and <code>z-index</code>.
    </td>
  </tr>
</table>

## 🛠 How it's built

| Part | How |
|---|---|
| 🧱 **Structure** | Semantic HTML5: `<header>`, `<aside>`, `<main>`, `<article>`, `<footer>` |
| 🎨 **Theme** | CSS variables in `:root` for the whole palette: lime `#86BC25` on slate `#0F172A` |
| 📐 **Layout** | CSS Grid for the page (fixed 280px sidebar + flexible workspace) and the auto-fitting card grids; Flexbox for headers, buttons and summary cards |
| 📱 **Responsive** | Media queries reflow everything for tablets and phones |
| ✂️ **Clean styles** | One shared `style.css`, no inline styles |
| ⚡ **JavaScript** | Plain JavaScript, only where it's needed: dark mode and the sandbox |

<details>
<summary><b>🐙 How the work was organised with Git</b></summary>
<br>

- **Feature branches:** `main` always held a working version; each part (header, sidebar, each lesson) was built on its own branch, like `feature/homepage-layout` or `feature/licao1-matriz`.
- **Conventional Commits:** short, clear messages with prefixes such as `feat:`, `fix:` and `style:`.
- **Checked before merging:** every change was tested with Live Server at different screen sizes before it reached `main`.

</details>

## 🚀 Run it locally

```bash
git clone https://github.com/PauloDuarteOliveira/UpSkill-ServiceNow-Hub.git
```

Open the folder in **VS Code**, right-click `index.html` → **Open with Live Server**. Or simply open `index.html` in your browser.

## 📁 Project structure

```
UpSkill-ServiceNow-Hub/
├── index.html              → Dashboard
├── js-modulo-licao1.html   → Lesson 1: syntax, variables and logic
├── js-modulo-licao2.html   → Lesson 2: the DOM, Client Scripts and the sandbox
├── style.css               → All the styles
├── assets/                 → Logo and profile pictures
├── referencias/            → Design references (Google Stitch)
└── docs/                   → README banner and screenshots
```

## 🎨 Design

The layout was based on a dashboard designed with **Google Stitch**; the reference images are in [`referencias`](referencias).

<br>

<div align="center">
  <img src="assets/Logo-Hub.png" alt="UpSkill ServiceNow Hub logo" height="48">
  <br>
  <sub>Made for the UPskill ServiceNow programme by <a href="https://github.com/PauloDuarteOliveira"><b>Paulo Duarte Oliveira</b></a> · 2026</sub>
</div>
