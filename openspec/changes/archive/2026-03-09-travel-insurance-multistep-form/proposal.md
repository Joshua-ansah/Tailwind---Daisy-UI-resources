## Why

The project needs a professional, conversion-optimised multi-step form for a Travel Insurance application. Breaking a complex insurance application into guided wizard steps reduces cognitive load, improves completion rates, and aligns with modern SaaS onboarding patterns.

## What Changes

- **New**: `travel-insurance.html` — a self-contained, static HTML page that implements the full 4-step wizard UI
- **New**: Wizard step navigation sidebar (left panel) with step indicators, connecting lines, and active/completed states
- **New**: Form content area (right panel) with per-step field layouts, validation placeholders, and bottom navigation controls
- **New**: Responsive layout that collapses the sidebar into a horizontal step indicator on mobile

## Capabilities

### New Capabilities

- `multistep-wizard-layout`: Two-column page layout (sidebar step nav + form content area) with flex/grid, responsive breakpoints, and step state management
- `step-navigation-sidebar`: Vertical list of steps with circular indicators, connecting lines, and active/completed/upcoming visual states
- `form-fields`: Per-step form fields (text, email, phone, select, date, file upload, checkbox) with labels, helper text, and error placeholders
- `bottom-navigation-controls`: Back / Save Draft / Next (Submit on last step) button bar at the bottom of the form area

### Modified Capabilities

## Impact

- Adds `travel-insurance.html` to the project root
- Uses existing TailwindCSS v4 + DaisyUI setup (no additional dependencies)
- No changes to `index.html`, `vite.config.js`, or any existing files
