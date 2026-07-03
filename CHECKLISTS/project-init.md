# Project Init Checklist

在 Discovery 完成、项目需求摘要已经足够清楚、可以选择项目结构时，使用这个 Checklist。

## 目标

根据真实需求初始化一个传统、清晰、容易理解的项目结构。

## 检查项

### 项目形态

- [ ] 这是简单应用、全栈应用、后端服务、前端应用、库、CLI、浏览器插件、移动端应用还是 Monorepo？
- [ ] 是否需要拆分 `backend/` 和 `frontend/`？
- [ ] 是否需要 `apps/` 和 `packages/`？
- [ ] 现在是否需要基础设施或部署配置？

### 文档

- [ ] 根据 `AGENTS.template.md` 创建 `AGENTS.md`。
- [ ] 创建 `docs/project-brief.md`。
- [ ] 创建 `docs/architecture.md`。
- [ ] 创建 `docs/requirements/`。
- [ ] 创建 `docs/design/`。
- [ ] 创建 `docs/decisions/`。

### 架构基线

- [ ] 记录项目类型。
- [ ] 记录技术栈，如果已经选择。
- [ ] 记录模块边界。
- [ ] 记录数据/存储方案，如果已知。
- [ ] 记录部署假设，如果已知。

### 范围控制

- [ ] 不要在需求不足时生成复杂结构。
- [ ] 除非明确必要，不要引入微服务。
- [ ] 除非需求明确要求，不要引入队列、缓存、Kubernetes 或重型基础设施。
- [ ] 优先选择能支撑第一版的最简单结构。

## 推荐默认结构

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

## 更复杂的全栈结构

仅在确实需要时使用：

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

## 输出

初始化完成后，清楚报告：

- 创建了哪些文件和目录
- 为什么选择这个结构
- 下一步建议做什么
