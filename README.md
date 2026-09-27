# 🧩 Basic HTML Website

A simple, multi-page, HTML-only personal portfolio website built as part of the 
[roadmap.sh](https://roadmap.sh/projects/basic-html-website) project series.

This project focuses on **semantic HTML structure**, **multi-page architecture**, 
and **SEO fundamentals** — without any CSS or JavaScript.

---

## 📋 Project Overview

This is the **first step** in a series of web development projects from 
[roadmap.sh](https://roadmap.sh/projects/basic-html-website). The goal is to 
master the fundamentals of **HTML structure** and **semantic markup** before 
moving on to CSS styling in the next project.

The website consists of **four pages** with a shared navigation bar, built 
entirely with **HTML** — no CSS, no JavaScript.

---

## 🎯 Goals & Requirements

Based on the original [project requirements](https://roadmap.sh/projects/basic-html-website):

- [x] Create a multi-page website (Home, Projects, Articles, Contact)
- [x] Include a navigation bar present on **all** pages
- [x] Use **semantically correct** HTML tags
- [x] Structure the code for easy future styling
- [ ] Add **SEO meta tags** to the `<head>` of each page
- [x] Include a **contact form** with name, email, and message fields
- [x] **No CSS or styling** — structure only
- [ ] Fix HTML validity issues (see TODO section below)

---

## 📁 Project Structure

```

Basic-HTML-Website/
│
├── home.html          # Homepage
├── projects.html      # Projects page
├── articles.html      # Articles page
├── contact.html       # Contact page (with form)
├── images/            # Image assets
│   ├── banner.jpeg
│   └── avatar.jpeg
└── README.md          # Project documentation

```

---

## 📄 Pages Description

| Page | File | Description | Status |
|------|------|-------------|--------|
| **Home** | `home.html` | Landing page with hero, projects, experience, education & reviews | ✅ Done |
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
</main>

<footer>
  <!-- Footer content -->
</footer>
```

**Semantic tags used:** `<header>`, `<nav>`, `<main>`, `<section>`, 
`<article>`, `<aside>`, `<footer>`, `<form>`, `<blockquote>`, `<cite>`.

---

## 🔍 SEO Meta Tags

Currently, each page's `<head>` only contains:

- `<meta charset="UTF-8">`
- `<meta name="viewport">`
- `<title>`

⚠️ **Missing SEO tags** (to be added — see TODO):

- `<meta name="description">`
- `<meta name="keywords">`
- `<meta name="author">`
- Open Graph tags (`og:title`, `og:description`, `og:type`)
- `<meta name="robots">`

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

3. Open `home.html` in your browser:

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
- **No CSS** — Styling will be added in the [next project](https://roadmap.sh/projects/basic-html-website)

---

## ⚠️ Known Issues & TODO

The following issues were identified during a code review. They are listed 
in priority order and will be fixed progressively.

### 🔴 High Priority (must fix)

- [ ] **Add SEO meta tags** to all pages (`description`, `keywords`, `author`, Open Graph)
- [ ] **Remove invalid `<hr>` tags** inside `<ol>` and between `<li>` elements 
      in `projects.html` (W3C invalid)
- [ ] **Move `<h3>`, `<h4>`, and `<p>`** out of `<ul>` in `home.html` 
      (invalid children of `<ul>`)
- [ ] **Remove `<p>` nested inside `<span>`** in `projects.html` 
      (invalid block-in-inline)
- [ ] **Add `type="email"` and `required`** to the email input in `contact.html`
- [ ] **Add `required`** to name and message fields in `contact.html`
- [ ] **Fix duplicate `<h1>` tags** inside `<article>` elements in `articles.html` 
      (should be `<h2>`)
- [ ] **Replace `action="https://"`** with a valid endpoint or `#` in `contact.html`

### 🟠 Medium Priority

- [ ] **Convert navbar to a semantic `<ul>` list** instead of `<a> / <a>` pattern
- [ ] **Add `<footer>`** to `contact.html`, `projects.html`, and `articles.html` 
      for consistency with `home.html`
- [ ] **Rename `home.html` to `index.html`** (web standard for the homepage)
- [ ] **Add `aria-current="page"`** to the active page link in the navigation
- [ ] **Remove duplicate `<hr><hr>`** occurrences across all pages

### 🟡 Low Priority

- [ ] **Improve ID naming** in `projects.html` (`#PUP` → `#product-upcoming`, etc.)
- [ ] **Replace empty `http://` and `https://` links** with `#` or real URLs
- [ ] **Use `<ul>` with `<li>`** for the reviews list in `home.html` (currently uses bare `<blockquote>`)

### 🧪 Validation

- [ ] **Validate all pages** with [W3C Validator](https://validator.w3.org) 
      and fix reported errors

---

## 📚 Reference

- **Project Source:** [roadmap.sh — Basic HTML Website](https://roadmap.sh/projects/basic-html-website)
- **Author:** [@ehsanidev-frontend](https://github.com/ehsanidev-frontend)

---

## 🗺️ Roadmap Progress

This project is part of my learning journey on [roadmap.sh](https://roadmap.sh):

- [x] **Basic HTML Website** ← *you are here*
- [ ] Styling with CSS (upcoming)
- [ ] Responsive Design
- [ ] JavaScript Basics

---

## 📝 License

This project is open-source and available for learning purposes.

---

## 🙌 Acknowledgments

- [roadmap.sh](https://roadmap.sh) for providing the project guidelines
- The open-source community for inspiration

---

⭐ If you found this project helpful, feel free to give it a star!

