# Front-end Asset Library

A personal collection of UI components and layout patterns built with **TailwindCSS v4** and **DaisyUI** — curated as ready-to-use templates for AI-assisted development.

> **Disclaimer:** This is an independent personal project. I am not affiliated with, endorsed by, or connected to DaisyUI or Tailwind Labs in any way.

---

## Purpose

I built this library for one specific reason: to give AI coding assistants a concrete, working reference when helping me build UIs.

Instead of describing what I want and hoping the model guesses the right class names, I can point it at a component page and say "build me something like this." Every file is plain, readable HTML — no compiled output, no abstractions — so a model can parse it, understand the pattern, and adapt it directly.

---

## Stack

| Tool | Version | Notes |
|---|---|---|
| [Vite](https://vitejs.dev) | v7 | Dev server + build tool |
| [TailwindCSS](https://tailwindcss.com) | v4 | Loaded via `@tailwindcss/vite` plugin |
| [DaisyUI](https://daisyui.com) | latest | Loaded via `@plugin "daisyui"` in `src/style.css` |

No framework. No JSX. Just HTML files.

---

## Getting Started

```bash
npm install
npm run dev
```

Open `http://localhost:5173` to see the homepage, then navigate to `/components/index.html` for the full component library.

---

## Project Structure

```
/
├── index.html                  # Homepage — project overview
├── src/
│   ├── main.js                 # Entry point (imports style.css)
│   └── style.css               # @import "tailwindcss" + @plugin "daisyui"
├── vite.config.js              # Tailwind vite plugin registered
└── components/
    ├── index.html              # Component library grid
    ├── buttons.html
    ├── forms.html
    ├── cards.html
    ├── navigation.html
    ├── modal.html
    ├── modals-alerts.html
    ├── badges-chips.html
    ├── tables.html
    ├── typography.html
    ├── avatars-media.html
    ├── loaders-feedback.html
    ├── hero-banners.html
    ├── stats-data.html
    ├── timeline-steps.html
    ├── multi-step-form.html
    ├── calendar.html
    ├── checkbox.html
    ├── fieldset.html
    ├── file-input.html
    ├── filter.html
    ├── label.html
    ├── validator.html
    ├── text-input.html
    ├── select.html
    ├── steps.html
    ├── tooltip.html
    ├── skeleton.html
    └── pagination.html
```

---

## Component Pages

Each page is a self-contained HTML file demonstrating a single DaisyUI/Tailwind component category. Sections within each page cover:

- All variants (colors, sizes, states)
- Common use-case patterns
- Accessible markup (labels, ARIA where relevant)
- Interactive demos where applicable (modals, wizards, pickers)

Pages are browsable at `/components/index.html` when the dev server is running.

---

## Using with AI

Point your AI assistant at any component file as context. Because each file:

- Uses semantic class names (`btn`, `card`, `modal-box`, etc.)
- Follows consistent structure across all pages
- Contains no compiled or minified output
- Is fully self-contained (single `<script>` tag for Tailwind)

...it's straightforward for a model to read, understand, and reproduce patterns from.

Example prompt pattern:
> "Referring to `components/modal.html` for the modal pattern and `components/forms.html` for form layout, build me a settings dialog with a profile update form."
