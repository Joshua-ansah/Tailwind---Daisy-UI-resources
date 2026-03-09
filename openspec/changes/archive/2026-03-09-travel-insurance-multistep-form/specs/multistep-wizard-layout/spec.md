## ADDED Requirements

### Requirement: Two-column page layout
The page SHALL render a two-column layout on desktop viewports (≥1024px) with a fixed-width left sidebar and a flex-grow right form panel arranged horizontally.

#### Scenario: Desktop layout renders two columns
- **WHEN** the page is viewed at viewport width ≥1024px
- **THEN** the sidebar and form panel SHALL appear side-by-side horizontally

#### Scenario: Mobile layout stacks vertically
- **WHEN** the page is viewed at viewport width <1024px
- **THEN** the sidebar SHALL be hidden and a horizontal step indicator SHALL appear above the form panel

#### Scenario: Sidebar has fixed width
- **WHEN** the layout renders on desktop
- **THEN** the sidebar SHALL have a fixed width of 18rem (w-72) and SHALL NOT grow or shrink
