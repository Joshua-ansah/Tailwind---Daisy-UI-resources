## ADDED Requirements

### Requirement: Timeline and steps patterns are shown
The `components/timeline-steps.html` page SHALL show vertical timeline and horizontal wizard step patterns.

#### Scenario: Vertical activity timeline is shown
- **WHEN** the page renders
- **THEN** it SHALL show a vertical timeline with at least 5 entries each containing a date, icon dot, title, and description

#### Scenario: DaisyUI horizontal steps wizard is shown
- **WHEN** the page renders
- **THEN** it SHALL show DaisyUI `steps` in a horizontal layout with completed, active, and upcoming states and step content below

#### Scenario: Activity feed (compact list) is shown
- **WHEN** the page renders
- **THEN** it SHALL show a compact vertical activity feed with avatar, action description, and timestamp per row
