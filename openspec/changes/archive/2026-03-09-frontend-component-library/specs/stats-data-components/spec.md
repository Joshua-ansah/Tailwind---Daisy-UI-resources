## ADDED Requirements

### Requirement: Stats and data display patterns are shown
The `components/stats-data.html` page SHALL show stat cards and data visualisation placeholder patterns.

#### Scenario: DaisyUI stat components are shown
- **WHEN** the page renders
- **THEN** it SHALL show DaisyUI `stats` in horizontal and vertical layout with title, value, description, and figure

#### Scenario: KPI grid with trend indicators is shown
- **WHEN** the page renders
- **THEN** it SHALL show a responsive 4-column grid of KPI cards each with a metric value, label, and up/down trend badge

#### Scenario: Comparison / stacked bar and countdown are shown
- **WHEN** the page renders
- **THEN** it SHALL show a labelled stacked progress bar for comparison and a DaisyUI countdown component
