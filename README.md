# 🧩 Personal Portfolio

A responsive, multi-page personal portfolio website built as part of the 
[roadmap.sh](https://roadmap.sh/projects/portfolio-website) project series.

This project is the **second step** in the roadmap: taking the HTML-only structure 
from the previous project and styling it with modern CSS techniques.

---

## 📋 Project Overview

This project converts the previous [Basic HTML Website](https://roadmap.sh/projects/basic-html-website) 
into a **fully styled, responsive personal portfolio** using pure CSS.

The goal is to practice:
- Responsive layouts with **Flexbox**
- **Media queries** for different screen sizes
- **Box model** and modern CSS techniques
- **Typography** and color schemes
- **Dark mode** support via CSS variables

The website still consists of **four pages** with a shared navigation bar, 
now fully styled and responsive.

---

## 🎯 Goals & Requirements

Based on the original [project requirements](https://roadmap.sh/projects/portfolio-website):

- [x] Fully styled, responsive website
- [x] Same structure as the previous HTML-only project
- [x] Consistent color scheme and typography
- [x] Use of Flexbox, media queries, and box model
- [x] Responsive navigation bar
- [x] Well-styled contact form
- [x] Use of Google Fonts (Caveat + Roboto)
- [x] Dark mode support via CSS variables
- [ ] Host on GitHub Pages or Cloudflare Pages (bonus)
- [ ] Add SEO meta tags to all pages
- [ ] Fix remaining HTML validity issues

---

## 📁 Project Structure

```

Basic-HTML-Website/
│
├── index.html              # Homepage (rename home.html → index.html)
├── projects.html           # Projects page
├── articles.html           # Articles page
├── contact.html            # Contact page (with form)
├── images/                 # Image assets
│   ├── banner.jpeg
│   └── avatar.jpeg
├── css/
│   ├── reset.css           # Modern CSS reset
│   ├── fonts.css           # Design tokens (typography, colors, spacing)
│   └── style.css           # Main stylesheet
└── README.md               # Project documentation

```

---

## 🎨 Design System

### Typography
- **Headings:** [Caveat](https://fonts.google.com/specimen/Caveat) (cursive)
- **Body:** [Roboto](https://fonts.google.com/specimen/Roboto) (sans-serif)
- **Fluid sizing** with `clamp()` for responsive headings

### Color Scheme
| Token | Value | Usage |
|-------|-------|-------|
| Primary | `#00c8d7` | Accents, links, borders |
| Secondary | `#ff9dff` | Header gradient |
| Text | `#333333` | Body text |
| Heading | `#1a1a1a` | Headings |
| Muted | `#6b7280` | Footer, secondary text |

### Dark Mode
Automatically respects `prefers-color-scheme: dark` via CSS variables.

---

## 📄 Pages Description

| Page | File | Description | Status |
|------|------|-------------|--------|
| **Home** | `home.html` | Hero, projects, experience, education & reviews | ✅ Done |
| **Projects** | `projects.html` | Showcase of 5 sample projects | ✅ Done |
| **Articles** | `articles.html` | Blog-style articles listing | ✅ Done |
| **Contact** | `contact.html` | Contact form (name, email, message) | ✅ Done |

---

## 🧱 Semantic HTML Structure

Each page follows a consistent semantic layout:

```html
<header>
  <nav> <!-- Navigation links --> </nav>
</header>

<main>
  <section> <!-- Main content --> </section>
  <article> <!-- Article content --> </article>
</main>

<footer>
  <!-- Footer content -->
</footer>
```

**Semantic tags used:** `<header>`, `<nav>`, `<main>`, `<section>`, 
`<article>`, `<hgroup>`, `<blockquote>`, `<cite>`, `<time>`, `<footer>`, `<form>`.

---

## 🚀 How to Run

1. Clone the repository:

```bash
git clone https://github.com/ehsanidev-frontend/Basic-HTML-Website.git
```

2. Navigate to the project folder:

```bash
cd Basic-HTML-Website
```

3. Open `home.html` (or `index.html` after rename) in your browser:

```bash
# On macOS
open home.html

# On Windows
start home.html

# Or use a local server (recommended)
npx serve .
```

No build step or dependencies required. ✅

---

## 🛠️ Built With

- **HTML5** — Semantic markup
- **CSS3** — Custom properties, Flexbox, `clamp()`, cascade layers
- **Google Fonts** — Caveat & Roboto
- **Modern CSS Reset** — `@layer reset` approach

---

## ⚠️ Known Issues & TODO

The following issues were identified during a code review. They are listed 
in priority order and will be fixed progressively.

### 🔴 High Priority (must fix)

- [ ] **Add SEO meta tags** to all pages (`description`, `keywords`, `author`, Open Graph)
- [ ] **Remove invalid `<hr>` tags** inside `<ol>` and between `<li>` elements 
      in `projects.html` (W3C invalid)
- [ ] **Remove `<p>` nested inside `<span>`** in `projects.html` 
      (invalid block-in-inline)
- [ ] **Add `type="email"` and `required`** to the email input in `contact.html`
- [ ] **Add `required`** to name and message fields in `contact.html`
- [ ] **Fix duplicate `<hr><hr>`** occurrences across all pages
- [ ] **Replace `action="https://"`** with a valid endpoint or `#` in `contact.html`

### 🟠 Medium Priority

- [ ] **Convert navbar to a semantic `<ul>` list** instead of `<a> / <a>` pattern
- [ ] **Add `<footer>`** to `contact.html`, `projects.html`, and `articles.html` 
      for consistency with `home.html`
- [ ] **Rename `home.html` to `index.html`** (web standard for the homepage)
- [ ] **Add `aria-current="page"`** to the active page link in the navigation
- [ ] **Add media queries** for mobile-first responsive behavior
- [ ] **Replace empty `http://` and `https://` links** with `#` or real URLs

### 🟡 Low Priority

- [ ] **Improve ID naming** in `projects.html` (`#PUP` → `#product-upcoming`, etc.)
- [ ] **Use `<ul>` with `<li>`** for the reviews list in `home.html`
- [ ] **Add transitions/animations** for hover states
- [ ] **Host on GitHub Pages** or Cloudflare Pages (bonus)

### 🧪 Validation

- [ ] **Validate all pages** with [W3C Validator](https://validator.w3.org) 
      and fix reported errors
- [ ] **Validate CSS** with [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)

---

## 📚 Reference

- **Project Source:** [roadmap.sh — Personal Portfolio](https://roadmap.sh/projects/portfolio-website)
- **Previous Project:** [roadmap.sh — Basic HTML Website](https://roadmap.sh/projects/basic-html-website)
- **Author:** [@ehsanidev-frontend](https://github.com/ehsanidev-frontend)

---

## 🗺️ Roadmap Progress

This project is part of my learning journey on [roadmap.sh](https://roadmap.sh):

- [x] **Basic HTML Website** — HTML structure
- [x] **Personal Portfolio** ← *you are here* (CSS styling)
- [ ] Responsive Design (advanced)
- [ ] CSS Grid & Animations
- [ ] JavaScript Basics

---

## 📝 License

This project is open-source and available for learning purposes.

---

## 🙌 Acknowledgments

- [roadmap.sh](https://roadmap.sh) for providing the project guidelines
- Google Fonts for Caveat & Roboto
- The open-source community for inspiration

---

⭐ If you found this project helpful, feel free to give it a star!
