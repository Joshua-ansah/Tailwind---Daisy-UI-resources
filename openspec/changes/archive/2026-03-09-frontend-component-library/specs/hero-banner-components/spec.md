## ADDED Requirements

### Requirement: Hero and banner patterns are shown
The `components/hero-banners.html` page SHALL show full-width page hero and call-to-action banner patterns.

#### Scenario: Centered hero with headline and CTA is shown
- **WHEN** the page renders
- **THEN** it SHALL show a DaisyUI `hero` with a centered headline, sub-headline, and primary + secondary CTA buttons

#### Scenario: Split hero (text left, image right) is shown
- **WHEN** the page renders
- **THEN** it SHALL show a two-column hero with text on the left and a placeholder image on the right

#### Scenario: Feature highlight section is shown
- **WHEN** the page renders
- **THEN** it SHALL show a 3-column feature grid with icon, title, and description per feature

#### Scenario: CTA banner strip is shown
- **WHEN** the page renders
- **THEN** it SHALL show a full-width coloured banner with a headline and a button aligned right
