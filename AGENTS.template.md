# AGENTS.md

This project is assisted by the AI Tech Lead workflow.

## Project Rule

Do not treat AI as a direct code generator. Treat AI as an engineering collaborator that must clarify, design, implement, and review in order.

## Default Development Flow

For non-trivial work, follow this sequence:

1. Clarify requirement.
2. Produce or update design.
3. Wait for user confirmation when design changes behavior, architecture, API, data model, or permissions.
4. Implement with minimal changes.
5. Run available validation.
6. Summarize changed files, tests, and remaining risks.

## Documentation Structure

Use the traditional project documentation layout:

```text
docs/
├── project-brief.md
├── architecture.md
├── requirements/
├── design/
└── decisions/
```

## Requirement Rules

- Requirements are the long-term source of truth.
- If a requirement is unclear, ask before coding.
- Requirements should include actors, scope, behavior, permissions, edge cases, and acceptance criteria.

## Design Rules

- Designs are required for complex changes.
- Designs should explain modules, interfaces, data model, flow, risks, and test strategy.
- If design conflicts with requirements, requirements win.

## Coding Rules

- Make the smallest safe change.
- Do not modify unrelated modules.
- Do not perform opportunistic refactors.
- Preserve existing behavior unless the requirement says otherwise.
- Add or update tests when practical.

## Review Rules

Before considering work complete, check:

- requirement match
- design match
- scope control
- permissions and security
- edge cases
- tests or validation
- documentation impact

## User Override

The user may choose to skip a recommended stage.

If they do, clearly state the skipped stage, the risk, and the safest minimal next step.
