# Coding Checklist

Use this checklist when the requirement and design are ready and the user has approved implementation.

## Goal

Implement the requested change with minimal, safe, reviewable modifications.

## Checkpoints

### Before Coding

- [ ] Requirement exists or is explicitly waived.
- [ ] Design exists for non-trivial changes or is explicitly waived.
- [ ] Affected files/modules are identified.
- [ ] Test or validation plan is known.

### Scope Control

- [ ] Modify only files needed for the task.
- [ ] Do not perform unrelated refactors.
- [ ] Do not rename or restructure modules unless required by design.
- [ ] Do not change public interfaces unless design says so.

### Implementation

- [ ] Follow existing project style.
- [ ] Keep business logic in the appropriate layer.
- [ ] Validate inputs and handle errors.
- [ ] Respect permission/security rules.
- [ ] Keep code readable and maintainable.

### Tests and Validation

- [ ] Add or update tests when practical.
- [ ] Run relevant tests, lint, typecheck, or build commands when available.
- [ ] If tests cannot be run, explain why and provide manual validation steps.

### Completion Summary

Report:

- files changed
- behavior changed
- tests/validation run
- risks or follow-up work

## Output

Implement code only after this checklist is satisfied or the user explicitly chooses to proceed with recorded risk.
