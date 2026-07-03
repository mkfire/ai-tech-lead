# AI Tech Lead

AI Tech Lead 是一个轻量级的 AI 工程负责人 Skill / Playbook，用于辅助 AI 参与软件工程开发。

它优先适配 Codex，同时保持方法足够通用，后续也可以迁移到 Cursor、Claude Code 或其他 AI Coding 工具。

## 目标

帮助用户从一个模糊想法出发，逐步形成可开发的需求与技术方案，然后再引导 AI Coding 工具按“需求 → 设计 → 任务拆分 → 开发 → Review”的方式推进。

AI Tech Lead 不是另一个代码生成器，而是一层轻量的工程化约束，让 AI Coding 工具更像一个谨慎的技术负责人：

- 写代码前先澄清需求
- 根据真实需求推荐项目结构
- 实现前先输出设计方案
- 设计确认后拆分可执行任务
- 控制开发范围和风险
- 按需求检查开发结果
- 保持项目文档简单、传统、易理解

## 推荐形态

这个仓库推荐作为 Codex Skill 使用，同时提供项目级 `AGENTS.md` 模板。

- `SKILL.md` 定义 AI Tech Lead 的核心行为。
- `CHECKLISTS/` 定义各阶段的工程检查清单。
- `TEMPLATES/` 定义可复用的文档模板。
- `AGENTS.template.md` 可以复制到项目根目录并改名为 `AGENTS.md`。

## V1 范围

V1 聚焦一个实用、低成本的开发流程：

1. Discovery：澄清项目想法。
2. Project Brief：整理项目需求摘要。
3. Project Init：根据需求推荐并初始化传统项目结构。
4. Requirement：细化模块级需求。
5. Design：输出可 Review 的实现方案。
6. Task Planning：设计确认后拆分可执行任务。
7. Coding：按任务引导 AI 实现。
8. Review：按需求、设计、任务、风险和测试检查结果。

V1 暂时不包含 CLI、GitHub App、VS Code 插件、多 Agent 调度器或复杂状态引擎。这些可以在方法验证后再做。

## 初始化后的推荐项目结构

```text
project/
├── AGENTS.md
├── docs/
│   ├── project-brief.md
│   ├── architecture.md
│   ├── requirements/
│   ├── design/
│   ├── tasks/
│   └── decisions/
└── src/
```

让项目结构保持熟悉。把复杂逻辑放在 Skill 里，而不是暴露成奇怪的项目目录。

## 最快使用方式

1. 安装到用户级 Skills 目录：

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/mkfire/ai-tech-lead.git ~/.codex/skills/ai-tech-lead
```

2. 在 Codex 里输入：

```text
Use the AI Tech Lead skill.
我想做一个新项目。请先帮我澄清需求，再推荐项目结构和技术方案。暂时不要写业务代码。
```

3. 如果是在已有项目里使用，可以把 `AGENTS.template.md` 复制到项目根目录，并改名为 `AGENTS.md`。

## 验证是否生效

安装后可以在 Codex 里输入：

```text
Use the AI Tech Lead skill.
请说明你会如何处理一个新项目需求。不要写代码。
```

如果生效，AI 应该先说明会进入 Discovery / 需求澄清阶段，而不是直接生成项目代码。

## 适合使用

- 新项目启动
- 模块需求澄清
- 复杂功能设计
- 权限、数据模型、API 或架构变更
- Codex 开发前评审
- AI 生成代码后的 Review
- 需要控制范围和减少返工的任务

## 不适合使用

- typo、错别字、标点修正
- 简单文案修改
- 一行配置修改
- 明确的小范围样式调整
- 用户已经完全明确要求直接做的小改动

这些场景可以按轻量模式处理，不需要完整走需求/设计流程。

## 在 Codex 中使用

### 方式 A：用户级 Skill

把这个仓库或 Skill 目录复制到你的用户级 Skills 目录：

```text
~/.codex/skills/ai-tech-lead/
```

### 方式 B：仓库级 Skill

把 Skill 复制到某个项目仓库中：

```text
project/
└── .codex/
    └── skills/
        └── ai-tech-lead/
```

### 推荐的首次使用 Prompt

```text
Use the AI Tech Lead skill.
我想做一个新项目。请先帮我澄清需求，再推荐项目结构和技术方案。暂时不要写业务代码。
```

### 推荐的功能开发 Prompt

```text
Use the AI Tech Lead skill.
我想开发 <功能/模块名称>。请先不要写代码，先帮我澄清需求，然后输出设计方案供我确认。
```

## 核心原则

不要先写代码。先推进项目。
