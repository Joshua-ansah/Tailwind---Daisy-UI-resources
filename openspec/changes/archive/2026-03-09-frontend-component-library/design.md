## Context

The project is a static Vite + TailwindCSS v4 + DaisyUI site. The goal is to add a `components/` directory containing self-contained HTML pages — one per component category. Each page can be opened directly via the Vite dev server and copied from freely. There is no JS framework; everything is plain HTML + Tailwind utility classes + DaisyUI component classes.

## Goals / Non-Goals

**Goals:**
- Consistent shared HTML shell across all component pages (nav back to index, page title)
- Every DaisyUI component category covered with all meaningful variants
- Each file is self-contained — copy a snippet from it into any project
- Index page with card links to every component category

**Non-Goals:**
- JavaScript interactivity (modals, drawers — rendered as open/static for visibility)
- Any build step beyond what Vite already provides
- Theming switcher (DaisyUI `data-theme` hardcoded to `light`)

## Decisions

**1. One file per category, not one file per component**
Keeps the file count manageable while still grouping logically. A single `forms.html` with all form variants is more useful for copy-paste than 10 separate files.

**2. Shared `_shell` pattern via HTML comments**
Every component file uses the same header markup (top nav back to index, page title section). No JS templating needed — developers copy the shell from any file.

**3. Components rendered in a `max-w-5xl mx-auto` content column**
Provides a realistic medium-viewport width context without a full-bleed layout disrupting component display.

**4. Variant labelling via `<h3>` headings above each component group**
Each variant group gets a clear heading (e.g., "Button Sizes", "Button States") so the page doubles as living documentation.

**5. DaisyUI `data-theme="light"` on `<html>`**
Keeps all components predictably styled without requiring users to understand theming first.

## Risks / Trade-offs

- [File length] Component category pages (especially forms, cards) will be long → Mitigation: well-commented sections make scanning easy
- [Copy-paste fidelity] Some DaisyUI components need JS to function (modals, drawers) → Mitigation: render them in their open/visible state so the HTML structure is clear
- [Vite multi-page] Each file must be referenced from `index.html` or opened directly — Vite serves all HTML files without extra config
