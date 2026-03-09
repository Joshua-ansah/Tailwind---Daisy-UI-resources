## ADDED Requirements

### Requirement: Loading and feedback patterns are shown
The `components/loaders-feedback.html` page SHALL show loading states, progress indicators, and user feedback components.

#### Scenario: Spinners and loading states are shown
- **WHEN** the page renders
- **THEN** it SHALL show DaisyUI `loading` spinners in all sizes and variants (spinner, dots, ring, bars)

#### Scenario: Progress bars and radial progress are shown
- **WHEN** the page renders
- **THEN** it SHALL show a linear progress bar and a DaisyUI radial progress circle at various percentages

#### Scenario: Skeleton loaders are shown
- **WHEN** the page renders
- **THEN** it SHALL show skeleton placeholder blocks mimicking a card and a list item layout

#### Scenario: Rating and tooltip are shown
- **WHEN** the page renders
- **THEN** it SHALL show a DaisyUI star rating component and tooltip examples (top, bottom, left, right)
