# Discovery Checklist

Use this checklist when the user has a vague project idea or asks to start a new project.

## Goal

Turn a vague idea into a concise project brief that can guide project initialization and technical planning.

## Checkpoints

### Problem and Goal

- [ ] What problem does this project solve?
- [ ] Who has this problem?
- [ ] What outcome should the first version achieve?
- [ ] What would make this project successful?

### Users and Roles

- [ ] Who will use the system?
- [ ] Are there different user roles?
- [ ] Does the project need login?
- [ ] Does the project need permissions or access control?

### First Version Scope

- [ ] What are the top 3 must-have features?
- [ ] What is explicitly out of scope for V1?
- [ ] Which feature should be built first?
- [ ] Are there features that can be delayed?

### Core Workflows

- [ ] What are the main user workflows?
- [ ] What data is created, imported, edited, or viewed?
- [ ] Are there approval, review, or audit steps?
- [ ] Are there recurring jobs or background tasks?

### Data and Integration

- [ ] Where does the data come from?
- [ ] Does the project integrate with third-party services?
- [ ] Does it need file upload, payment, email, messaging, scraping, browser extension, mobile app, or admin panel?
- [ ] Are there reporting or export requirements?

### Non-functional Requirements

- [ ] Are there performance expectations?
- [ ] Are there security or privacy requirements?
- [ ] Are there deployment constraints?
- [ ] Is this a prototype, internal tool, SaaS, production system, or enterprise system?

### Risks and Unknowns

- [ ] What is currently unclear?
- [ ] What decisions could cause major rework later?
- [ ] What should be validated before coding?

## Output

After completing discovery, produce `docs/project-brief.md` using `TEMPLATES/project-brief.md`.

Do not initialize a project skeleton until the project brief is clear enough to justify the structure.
