# Review Checklist

Use this checklist after implementation, for a patch, pull request, or completed module.

## Goal

Verify that the work is correct, scoped, safe, and ready for the next step.

## Checkpoints

### Requirement Match

- [ ] Does the implementation satisfy the requirement?
- [ ] Are all acceptance criteria covered?
- [ ] Are any requested behaviors missing?
- [ ] Did the implementation add unrequested behavior?

### Design Match

- [ ] Does the implementation follow the approved design?
- [ ] If it diverges, is the reason explained?
- [ ] Are interfaces and data structures consistent with the design?

### Scope and Maintainability

- [ ] Are changes limited to relevant files?
- [ ] Is there unnecessary refactoring?
- [ ] Is there duplicated logic?
- [ ] Is naming clear?
- [ ] Is the code maintainable?

### Security and Permissions

- [ ] Are permission checks correct?
- [ ] Is sensitive data protected?
- [ ] Are inputs validated?
- [ ] Are errors handled safely?

### Edge Cases

- [ ] Empty data
- [ ] Invalid input
- [ ] Unauthorized access
- [ ] External service failure
- [ ] Duplicate data
- [ ] Boundary values

### Tests and Validation

- [ ] Were tests added or updated?
- [ ] Were relevant tests run?
- [ ] Was build/typecheck/lint run if available?
- [ ] If not, is the reason explained?

### Documentation

- [ ] Does requirement/design need updating?
- [ ] Does architecture need updating?
- [ ] Is an ADR needed for a significant decision?

## Output

Review result should include:

- verdict: pass / needs changes / high risk
- issues found
- required fixes
- optional improvements
- validation status
