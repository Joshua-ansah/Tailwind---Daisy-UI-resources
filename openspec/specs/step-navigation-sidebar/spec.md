## ADDED Requirements

### Requirement: Vertical step list with indicators
The sidebar SHALL contain a vertically stacked list of 4 steps, each with a circular step number indicator, step title, and short description.

#### Scenario: All four steps are displayed
- **WHEN** the sidebar renders
- **THEN** it SHALL display exactly four steps: Personal Info, Travel & Insurance, Documents & Agreements, Confirm

#### Scenario: Active step is visually highlighted
- **WHEN** a step is the current active step
- **THEN** its circular indicator SHALL use a filled primary color and its title SHALL use bold text

#### Scenario: Completed step shows a check mark
- **WHEN** a step has been completed
- **THEN** its indicator SHALL show a checkmark icon and use a success/muted color

#### Scenario: Upcoming steps appear muted
- **WHEN** a step has not yet been reached
- **THEN** its indicator and title SHALL appear in a muted/gray color

#### Scenario: Vertical connecting line links steps
- **WHEN** the sidebar renders
- **THEN** a vertical line SHALL visually connect consecutive step indicators
