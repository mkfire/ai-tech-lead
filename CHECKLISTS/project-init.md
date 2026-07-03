# Project Init Checklist

Use this checklist after discovery, when the project brief is clear enough to choose a structure.

## Goal

Initialize a traditional, understandable project structure based on the actual requirement.

## Checkpoints

### Project Shape

- [ ] Is this a simple app, full-stack app, backend service, frontend app, library, CLI, extension, mobile app, or monorepo?
- [ ] Does it need separate backend and frontend directories?
- [ ] Does it need `apps/` and `packages/`?
- [ ] Does it need infrastructure or deployment configuration now?

### Documentation

- [ ] Create `AGENTS.md` from `AGENTS.template.md`.
- [ ] Create `docs/project-brief.md`.
- [ ] Create `docs/architecture.md`.
- [ ] Create `docs/requirements/`.
- [ ] Create `docs/design/`.
- [ ] Create `docs/decisions/`.

### Architecture Baseline

- [ ] Record project type.
- [ ] Record technology stack, if chosen.
- [ ] Record module boundaries.
- [ ] Record data/storage choice, if known.
- [ ] Record deployment assumptions, if known.

### Scope Control

- [ ] Do not generate complex structure before it is needed.
- [ ] Do not add microservices unless clearly justified.
- [ ] Do not add queues, cache, Kubernetes, or heavy infrastructure unless the requirement demands it.
- [ ] Prefer the simplest structure that can support the first version.

## Recommended Default Structure

```text
project/
├── AGENTS.md
├── docs/
│   ├── project-brief.md
│   ├── architecture.md
│   ├── requirements/
│   ├── design/
│   └── decisions/
└── src/
```

## More Complex Full-stack Structure

Use only when needed:

```text
project/
├── AGENTS.md
├── docs/
│   ├── project-brief.md
│   ├── architecture.md
│   ├── requirements/
│   ├── design/
│   └── decisions/
├── backend/
├── frontend/
└── infra/
```

## Output

After initialization, clearly report:

- created files/directories
- why this structure was selected
- what the next recommended step is
