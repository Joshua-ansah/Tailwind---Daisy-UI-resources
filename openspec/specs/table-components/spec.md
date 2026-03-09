## ADDED Requirements

### Requirement: Table variants are all represented
The `components/tables.html` page SHALL show common HTML table patterns styled with DaisyUI and Tailwind.

#### Scenario: Basic and striped tables are shown
- **WHEN** the page renders
- **THEN** it SHALL show a default table and a zebra-striped table using DaisyUI `table-zebra`

#### Scenario: Table with actions is shown
- **WHEN** the page renders
- **THEN** it SHALL show a table row with inline action buttons (edit, delete) and a checkbox column for selection

#### Scenario: Responsive table wrapper is shown
- **WHEN** the page renders
- **THEN** it SHALL wrap the table in an overflow-x-auto container for mobile compatibility
