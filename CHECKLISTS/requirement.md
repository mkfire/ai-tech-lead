# Requirement Checklist

Use this checklist before designing or coding a feature/module.

## Goal

Turn a feature idea into a requirement that is specific enough to design and test.

## Checkpoints

### Business Goal

- [ ] What problem does this feature solve?
- [ ] Who needs it?
- [ ] Why is it needed now?

### Scope

- [ ] What is included?
- [ ] What is excluded?
- [ ] What is the smallest useful version?

### Actors and Permissions

- [ ] Who can use this feature?
- [ ] Are there roles or permission differences?
- [ ] What data can each role see or modify?

### Functional Behavior

- [ ] What actions can the user perform?
- [ ] What data is required?
- [ ] What is the expected result of each action?
- [ ] Does the feature need search, filter, pagination, export, import, notification, or approval?

### Edge Cases

- [ ] What happens when data is missing?
- [ ] What happens with invalid input?
- [ ] What happens when the user lacks permission?
- [ ] What happens when external services fail?
- [ ] What happens with duplicate or stale data?

### Non-functional Requirements

- [ ] Are there performance requirements?
- [ ] Are there security requirements?
- [ ] Are there audit/logging requirements?
- [ ] Are there compatibility constraints?

### Acceptance Criteria

- [ ] How will the user know this is done?
- [ ] What test cases must pass?
- [ ] What should be manually verified?

## Output

Produce a requirement document using `TEMPLATES/requirement.md`.

If important information is missing, ask focused questions before writing the final requirement.
