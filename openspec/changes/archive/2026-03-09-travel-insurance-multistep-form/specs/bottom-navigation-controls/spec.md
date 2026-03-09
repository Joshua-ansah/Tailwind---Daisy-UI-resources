## ADDED Requirements

### Requirement: Bottom navigation button bar
The form area SHALL include a bottom navigation bar with Back, Save Draft, and Next (or Submit on the final step) buttons.

#### Scenario: Back button is disabled on the first step
- **WHEN** Step 1 is active
- **THEN** the Back button SHALL be visually disabled and non-interactive

#### Scenario: Back button is enabled on steps 2-4
- **WHEN** any step other than Step 1 is active
- **THEN** the Back button SHALL be enabled and clickable

#### Scenario: Next button label changes on last step
- **WHEN** Step 4 (Confirm) is active
- **THEN** the primary action button label SHALL read "Submit Application" instead of "Next"

#### Scenario: Save Draft button is always present
- **WHEN** any step is active
- **THEN** a "Save Draft" secondary button SHALL be visible between the Back and Next buttons

#### Scenario: Navigation bar is pinned to the bottom of the form panel
- **WHEN** the form panel renders
- **THEN** the button bar SHALL appear at the bottom with a visible top border separator
