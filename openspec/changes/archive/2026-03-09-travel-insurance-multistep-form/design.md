## Context

The project is a static Vite + TailwindCSS v4 + DaisyUI site. The goal is to add a single `travel-insurance.html` page that implements a 4-step wizard UI for a Travel Insurance application. No JavaScript framework is used — the page is pure HTML/CSS with Tailwind utility classes and DaisyUI components.

## Goals / Non-Goals

**Goals:**
- Two-column layout: fixed-width left sidebar (step nav) + flex-grow right panel (form content)
- Four wizard steps: Personal Info → Travel & Insurance → Documents & Agreements → Confirm
- Step indicators with active / completed / upcoming states and vertical connecting lines
- Per-step form fields using DaisyUI `input`, `select`, `file-input`, `checkbox`, `label`, `form-control`
- Bottom navigation bar: Back (disabled on step 1) | Save Draft | Next → Submit on step 4
- Responsive: stacks to horizontal step pill indicator on mobile

**Non-Goals:**
- JavaScript step switching logic (UI-only, static HTML)
- Backend form submission
- Accessibility beyond semantic HTML labels

## Decisions

**1. Use DaisyUI components over hand-rolled inputs**
DaisyUI provides consistent `input`, `select`, `btn`, `badge`, `steps` components out of the box. This reduces custom CSS and ensures visual consistency with the existing site.

**2. CSS-only step state via data attributes / classes**
Step active/completed/upcoming states are expressed purely through Tailwind and DaisyUI utility classes applied directly in HTML. No JavaScript needed for the static mockup.

**3. Sidebar width: fixed `w-72` (18rem)**
Gives enough room for step title + description on desktop without crowding the form area. Collapses via `hidden lg:flex` on mobile.

**4. Mobile: DaisyUI `steps` horizontal component above form**
On small screens, the sidebar is hidden and a compact DaisyUI horizontal `steps` strip appears above the form panel. This keeps the step context visible without consuming vertical space.

**5. Grid for form fields: `grid-cols-1 md:grid-cols-2`**
Standard SaaS form pattern — full width on mobile, two columns on desktop for natural field grouping (e.g., First Name / Last Name side by side).

## Risks / Trade-offs

- [Static only] No real step switching → Mitigation: clearly comment each step section in HTML so developers can wire it up with JS
- [DaisyUI `steps` mobile] Horizontal steps can overflow on very small screens → Mitigation: use `overflow-x-auto` on the steps container
- [Long forms] Step 3 (Documents & Agreements) has more fields → Mitigation: generous padding and `gap-6` grid spacing maintain readability
