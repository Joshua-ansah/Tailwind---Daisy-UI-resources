## ADDED Requirements

### Requirement: Navigation patterns are all represented
The `components/navigation.html` page SHALL show all common navigation UI patterns.

#### Scenario: Navbar variants are shown
- **WHEN** the page renders
- **THEN** it SHALL show a top navbar with logo + links + actions, a navbar with a dropdown menu, and a centered navbar

#### Scenario: Breadcrumb, tabs, and pagination are shown
- **WHEN** the page renders
- **THEN** it SHALL show a breadcrumb trail, a tabbed interface (boxed and bordered variants), and a pagination control

#### Scenario: Sidebar navigation is shown
- **WHEN** the page renders
- **THEN** it SHALL show a vertical sidebar menu using DaisyUI `menu` with icons and active states

#### Scenario: Bottom navigation bar is shown
- **WHEN** the page renders
- **THEN** it SHALL show a mobile-style bottom navigation strip with icons and labels
