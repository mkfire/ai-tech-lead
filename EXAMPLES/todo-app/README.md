# 示例：Todo App

这个示例展示 AI Tech Lead 应该如何引导一个简单项目。

## 用户输入

```text
我想做一个 todo app。
```

## 期望的 AI Tech Lead 行为

不要立刻创建代码。

先从 Discovery 开始：

```text
当前阶段：Discovery
状态：信息缺失
主要问题：项目范围仍然过于模糊
建议下一步：澄清第一版范围
```

提出聚焦问题：

1. 这个 Todo App 是个人使用、团队使用，还是公开 SaaS？
2. V1 是否需要登录？
3. 必须包含哪些操作：创建、编辑、完成、删除、搜索、标签、截止日期？
4. 数据是本地存储、服务端存储，还是跨设备同步？
5. 预期第一版交付物是什么：原型、生产应用，还是学习项目？

## 示例项目需求摘要

```md
# 项目需求摘要：Todo App

## 项目目标

构建一个简单的个人 Todo App，用于管理日常任务。

## 目标用户

- 个人用户

## V1 范围

### 必须包含

- 创建 Todo
- 编辑 Todo
- 标记 Todo 完成
- 删除 Todo
- 查看未完成/已完成 Todo

### 明确不做

- 团队协作
- 登录
- 重复任务
- 移动端 App

## 推荐结构

简单前端应用：

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

## 示例下一步

项目需求摘要确认后，初始化项目文档，并创建第一个模块需求：

```text
Use the AI Tech Lead skill.
请创建 Todo 列表模块的需求文档。暂时不要写代码。
```
