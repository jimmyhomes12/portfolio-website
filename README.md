# Data Analyst Portfolio Website

A clean, modern, single-page portfolio built with **Tailwind CSS** (loaded via CDN — no build step required).

## 🚀 Getting Started

Just open `index.html` in any browser — no installation needed.

```bash
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

Or drop the file into any static hosting service (GitHub Pages, Netlify, Vercel, etc.).

---

## ✏️ Customisation Guide

All editable content is in `index.html`. Search for the `✏️` emoji comments to find each section quickly.

| What to change | Where to look |
|---|---|
| **Your name & title** | `<title>` tag and Hero section (`<h1>`, `<h2>`) |
| **Profile photo** | Replace the placeholder `<div>` in the Hero with `<img src="photo.jpg" …>` |
| **Bio & contact details** | About section (`#about`) |
| **Stats** (years, projects…) | The four stat cards in `#about` |
| **Skills & tools** | Skill cards in `#skills` — duplicate/edit cards freely |
| **Projects** | Project `<article>` cards in `#projects` — update tags, title, description, links |
| **Work experience** | Timeline items in `#resume` Experience column |
| **Education** | Timeline items in `#resume` Education column |
| **Certifications** | List items in `#resume` Certifications section |
| **Resume PDF** | Add your PDF as `resume.pdf` next to `index.html` |
| **Contact form** | Update the `action` URL in `<form>` (supports Formspree, FormSubmit, EmailJS) |
| **Social links** | Footer social icon links in `#contact` |
| **Brand colour** | Change `brand` colour values in the `tailwind.config` `<script>` block |

### Changing the colour scheme

Open the `<script>` block near the top of `index.html` and edit the `brand` colours:

```js
tailwind.config = {
  theme: {
    extend: {
      colors: {
        brand: {
          50:  '#eff6ff',   // lightest tint
          100: '#dbeafe',
          500: '#3b82f6',   // mid accent
          600: '#2563eb',   // primary CTA colour  ← change this
          700: '#1d4ed8',
          900: '#1e3a8a',
        }
      }
    }
  }
}
```

Replace hex values with any Tailwind-compatible colour to re-theme the whole site instantly.

---

## 📁 Project structure

```
portfolio-website/
├── index.html      ← everything lives here
├── resume.pdf      ← add your CV here (optional)
└── images/         ← add project thumbnails & your photo here (optional)
```

## 🛠 Tech stack

- [Tailwind CSS](https://tailwindcss.com/) via CDN
- Plain HTML5 + minimal vanilla JS (copyright year only)
- [Inter](https://fonts.google.com/specimen/Inter) font via Google Fonts
