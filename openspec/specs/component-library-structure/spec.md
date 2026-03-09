## ADDED Requirements

### Requirement: Component library directory exists
The project SHALL contain a `components/` directory at the root containing all component HTML files and an index page.

#### Scenario: Index page links to all component categories
- **WHEN** a user opens `components/index.html`
- **THEN** they SHALL see a card grid linking to every component category page

#### Scenario: Each component page has a back link
- **WHEN** a user opens any component category page
- **THEN** they SHALL see a navigation link back to `components/index.html`

#### Scenario: All pages share the same visual shell
- **WHEN** any component page renders
- **THEN** it SHALL use the same header, background, and content column as all other pages
