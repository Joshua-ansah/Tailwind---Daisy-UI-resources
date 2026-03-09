## 1. Page Shell

- [ ] 1.1 Create `travel-insurance.html` in project root with full HTML boilerplate
- [ ] 1.2 Link `src/style.css` (Tailwind v4 + DaisyUI) via `<script type="module" src="/src/main.js">`
- [ ] 1.3 Set page title to "Travel Insurance Application"

## 2. Page Layout Structure

- [ ] 2.1 Create outer full-height flex container (`min-h-screen bg-base-200`)
- [ ] 2.2 Add left sidebar with `w-72 shrink-0 bg-base-100 border-r` hidden on mobile (`hidden lg:flex`)
- [ ] 2.3 Add right form panel as `flex-1` flex column with scroll

## 3. Mobile Step Indicator

- [ ] 3.1 Add DaisyUI `steps` horizontal strip above form on mobile (`lg:hidden`)
- [ ] 3.2 Mark current step with `step-primary`, completed with `step-primary`, upcoming default

## 4. Sidebar Step Navigation

- [ ] 4.1 Add sidebar header ("Application Steps" label)
- [ ] 4.2 Create step indicator list — 4 items with circular number badge, title, and description
- [ ] 4.3 Style active step (filled primary badge, bold title)
- [ ] 4.4 Style completed steps (checkmark icon, muted color)
- [ ] 4.5 Style upcoming steps (gray/muted badge and text)
- [ ] 4.6 Add vertical connecting lines between step indicators

## 5. Form Panel Header

- [ ] 5.1 Add step counter text ("Step 1 / 4") above the title
- [ ] 5.2 Add step title in large bold heading
- [ ] 5.3 Add helper description paragraph below title

## 6. Step 1 — Personal Info

- [ ] 6.1 Add two-column responsive grid (`grid grid-cols-1 md:grid-cols-2 gap-6`)
- [ ] 6.2 Add First Name and Last Name fields
- [ ] 6.3 Add Email and Phone fields
- [ ] 6.4 Add Date of Birth and Nationality (select) fields
- [ ] 6.5 Add label, helper text, and error placeholder to each field

## 7. Step 2 — Travel & Insurance

- [ ] 7.1 Add Departure Date and Return Date fields
- [ ] 7.2 Add Destination Country (select) and Trip Purpose (select) fields
- [ ] 7.3 Add Insurance Plan (select) and Number of Travellers (number input) fields
- [ ] 7.4 Add label, helper text, and error placeholder to each field

## 8. Step 3 — Documents & Agreements

- [ ] 8.1 Add Passport Photo file upload field
- [ ] 8.2 Add ID Document file upload field
- [ ] 8.3 Add Terms & Conditions checkbox with link
- [ ] 8.4 Add Privacy Policy checkbox with link
- [ ] 8.5 Add label and helper text to each field

## 9. Step 4 — Confirm

- [ ] 9.1 Add read-only summary card grouped by section (Personal, Travel, Documents)
- [ ] 9.2 Display summary rows as label/value pairs in a clean definition list or grid
- [ ] 9.3 Add declaration checkbox ("I confirm all information is correct")

## 10. Bottom Navigation Bar

- [ ] 10.1 Create sticky bottom bar with top border separator
- [ ] 10.2 Add Back button (disabled state on step 1)
- [ ] 10.3 Add Save Draft secondary button
- [ ] 10.4 Add Next button (primary) — label "Submit Application" on step 4
