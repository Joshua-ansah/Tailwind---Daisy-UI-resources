## ADDED Requirements

### Requirement: Button variants are all represented
The `components/buttons.html` page SHALL display all meaningful DaisyUI button variants.

#### Scenario: Button colours are displayed
- **WHEN** the page renders
- **THEN** it SHALL show buttons for every DaisyUI colour: default, primary, secondary, accent, info, success, warning, error, ghost, link

#### Scenario: Button sizes are displayed
- **WHEN** the page renders
- **THEN** it SHALL show buttons in xs, sm, md (default), and lg sizes

#### Scenario: Button states are displayed
- **WHEN** the page renders
- **THEN** it SHALL show disabled, loading (with spinner), and active states

#### Scenario: Button shapes and icon buttons are displayed
- **WHEN** the page renders
- **THEN** it SHALL show outline variants, wide button, block button, and icon-only square/circle buttons

#### Scenario: Button group is displayed
- **WHEN** the page renders
- **THEN** it SHALL show a joined button group using DaisyUI `join`
