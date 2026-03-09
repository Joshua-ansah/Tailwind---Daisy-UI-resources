## ADDED Requirements

### Requirement: All form input types are represented
The `components/forms.html` page SHALL display every common form input type with labels, helper text, and error states.

#### Scenario: Text inputs with states are shown
- **WHEN** the page renders
- **THEN** it SHALL show default, focused, disabled, and error-state text inputs

#### Scenario: Select, textarea, and speciality inputs are shown
- **WHEN** the page renders
- **THEN** it SHALL show a select dropdown, textarea, date picker, number input, and password input

#### Scenario: Checkboxes and radios are shown
- **WHEN** the page renders
- **THEN** it SHALL show checkbox groups and radio button groups in checked and unchecked states

#### Scenario: Toggle, range, and file input are shown
- **WHEN** the page renders
- **THEN** it SHALL show a DaisyUI toggle switch, range slider, and file upload input

#### Scenario: A complete form example is shown
- **WHEN** the page renders
- **THEN** it SHALL show a composed multi-field form card with submit and reset buttons
