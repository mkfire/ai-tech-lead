# AI Tech Lead

AI Tech Lead is a lightweight Engineering Manager skill/playbook for AI-assisted software development.

It is designed to work with Codex first, while keeping the method generic enough to adapt to Cursor, Claude Code, or other AI coding tools later.

## Goal

Help users move from a vague idea to a development-ready plan, then guide AI coding tools through requirement, design, implementation, and review.

AI Tech Lead is not another code generator. It is a lightweight engineering layer that helps AI coding tools behave more like a careful technical lead:

- clarify requirements before coding
- recommend project structure based on actual needs
- produce design before implementation
- control scope and risk
- review outputs against requirements
- keep project documents simple and traditional

## Recommended Form

Use this repository as a Codex Skill plus a project `AGENTS.md` template.

- `SKILL.md` defines the core AI Tech Lead behavior.
- `CHECKLISTS/` defines stage-by-stage engineering checks.
- `TEMPLATES/` defines reusable document formats.
- `AGENTS.template.md` can be copied into a project root as `AGENTS.md`.

## V1 Scope

V1 focuses on a practical, low-friction workflow:

1. Discovery: clarify the project idea.
2. Project Brief: summarize the real requirement.
3. Project Init: recommend and initialize a traditional project structure.
4. Requirement: refine module-level requirements.
5. Design: produce a reviewable implementation plan.
6. Coding: guide AI implementation only after design is ready.
7. Review: check the result against requirement, design, risk, and tests.

V1 intentionally does not include a CLI, GitHub App, VS Code extension, multi-agent scheduler, or complex state engine. Those can come later after the method is validated.

## Suggested Repository Structure After Initialization

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

Keep the project familiar. Put the intelligence in the skill, not in a strange project structure.

## How to Use with Codex

### Option A: User-level Skill

Copy this repository or the skill folder into your Codex user skills directory, for example:

```text
~/.codex/skills/ai-tech-lead/
```

### Option B: Repository-level Skill

Copy the skill into a project repository:

```text
project/
└── .agents/
    └── skills/
        └── ai-tech-lead/
```

### Recommended First Prompt

```text
Use the AI Tech Lead skill.
I want to build a new project. First help me clarify the requirement, then recommend the project structure and technical plan. Do not write application code yet.
```

### Recommended Feature Prompt

```text
Use the AI Tech Lead skill.
I want to develop <feature/module name>. Do not write code first. Start with requirement clarification, then produce a design for review.
```

## Core Principle

Do not write code first. Drive the project first.
