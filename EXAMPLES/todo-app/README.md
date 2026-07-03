# Example: Todo App

This example shows how AI Tech Lead should guide a simple project.

## User Input

```text
I want to build a todo app.
```

## Expected AI Tech Lead Behavior

Do not immediately create code.

Start with discovery:

```text
Current stage: Discovery
Status: missing information
Main issue: project scope is still too vague
Recommended next step: clarify the first version
```

Ask focused questions:

1. Is this todo app for personal use, a team, or a public SaaS?
2. Does V1 need login?
3. What are the must-have actions: create, edit, complete, delete, search, tags, due dates?
4. Is data local, server-side, or synced across devices?
5. What is the expected first deliverable: prototype, production app, or learning project?

## Example Project Brief

```md
# Project Brief: Todo App

## Project Goal

Build a simple personal todo app for managing daily tasks.

## Target Users

- Individual user

## V1 Scope

### Must Have

- Create todo
- Edit todo
- Mark todo complete
- Delete todo
- View active/completed todos

### Out of Scope

- Team collaboration
- Login
- Recurring tasks
- Mobile app

## Recommended Structure

Simple frontend app:

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

## Example Next Step

After the project brief is accepted, initialize the project docs and create the first module requirement:

```text
Use the AI Tech Lead skill.
Create the requirement for the todo list module. Do not write code yet.
```
