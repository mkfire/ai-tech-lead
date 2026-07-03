# Design Checklist

Use this checklist after the requirement is clear and before coding non-trivial work.

## Goal

Produce a reviewable design that explains how the requirement will be implemented safely.

## Checkpoints

### Requirement Alignment

- [ ] Does the design directly satisfy the requirement?
- [ ] Are all acceptance criteria covered?
- [ ] Are excluded items still excluded?

### Module Boundary

- [ ] Which module owns this feature?
- [ ] Which files/directories are likely affected?
- [ ] Are module boundaries clear?
- [ ] Are cross-module calls necessary and justified?

### Interfaces

- [ ] Are API endpoints, commands, functions, or UI events defined?
- [ ] Are inputs and outputs clear?
- [ ] Are error responses clear?
- [ ] Are DTOs/types/contracts needed?

### Data Model

- [ ] What data is created, read, updated, or deleted?
- [ ] Are schema changes needed?
- [ ] Is migration needed?
- [ ] Are indexes or constraints needed?

### Flow

- [ ] What is the main success path?
- [ ] What are the failure paths?
- [ ] What permission checks happen and where?
- [ ] Are external service calls involved?

### Risk

- [ ] What can break existing behavior?
- [ ] What might cause security or permission issues?
- [ ] What parts are uncertain?
- [ ] What should be validated before or during implementation?

### Test Strategy

- [ ] What unit tests are needed?
- [ ] What integration tests are needed?
- [ ] What manual verification is needed?
- [ ] What existing tests should be run?

### Task Split

- [ ] Can the implementation be split into small tasks?
- [ ] Are any tasks safely parallelizable?
- [ ] Which task should be done first?

## Output

Produce a design document using `TEMPLATES/design.md`.

Do not start coding until the user confirms the design, unless the user explicitly asks to skip design.
