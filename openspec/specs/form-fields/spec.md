## ADDED Requirements

### Requirement: Per-step form fields
Each wizard step SHALL render a distinct set of form fields appropriate to that step's data requirements, using DaisyUI form components.

#### Scenario: Step 1 renders personal info fields
- **WHEN** Step 1 is active
- **THEN** the form SHALL display fields for First Name, Last Name, Email, Phone, Date of Birth, and Nationality

#### Scenario: Step 2 renders travel and insurance fields
- **WHEN** Step 2 is active
- **THEN** the form SHALL display fields for Departure Date, Return Date, Destination Country, Trip Purpose, Insurance Plan, and Number of Travellers

#### Scenario: Step 3 renders documents and agreements fields
- **WHEN** Step 3 is active
- **THEN** the form SHALL display a passport photo file upload, an ID document file upload, and checkboxes for Terms & Conditions and Privacy Policy

#### Scenario: Step 4 renders confirmation summary
- **WHEN** Step 4 is active
- **THEN** the form SHALL display a read-only summary of all previously entered data grouped by section

#### Scenario: Every input has a label
- **WHEN** any form field renders
- **THEN** it SHALL have a visible label and an optional helper text below it

#### Scenario: Error placeholder is available per field
- **WHEN** a field has a validation error
- **THEN** a red error message placeholder SHALL appear below the field
