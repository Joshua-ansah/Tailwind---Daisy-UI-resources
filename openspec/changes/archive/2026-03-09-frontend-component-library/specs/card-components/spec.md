## ADDED Requirements

### Requirement: Card variants are all represented
The `components/cards.html` page SHALL display all common card layout patterns.

#### Scenario: Basic, image, and horizontal cards are shown
- **WHEN** the page renders
- **THEN** it SHALL show a plain content card, a card with a top image, and a horizontal media card

#### Scenario: Specialty cards are shown
- **WHEN** the page renders
- **THEN** it SHALL show a pricing card, a profile/user card, a stats card, and a card with actions (buttons in card-actions)

#### Scenario: Compact and glass card variants are shown
- **WHEN** the page renders
- **THEN** it SHALL show a compact DaisyUI card and a glass-style card on a gradient background
