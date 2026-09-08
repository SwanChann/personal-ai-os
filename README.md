# Personal AI OS

> 本文件是 Personal AI OS 的总览与导航页。
> 人类或 Agent 应在开始协作时先读取；具体配置以链接到的注册表和协议文件为 authoritative source。

My personal operating system for working with AI.

Status: Active

Version: 0.1

## Current Setup

| Category | Current Default |
| --- | --- |
| Primary Coding Agent | Codex |
| Primary General AI | ChatGPT |
| Default Coding Model | To be maintained |
| Default Research Model | To be maintained |
| Primary Knowledge Format | Markdown |
| Version Control | Git |

具体模型以 [MODELS.md](./MODELS.md) 为准。

## Default Operating Loop

```text
Goal
↓
Context
↓
Plan
↓
Execute
↓
Verify
↓
Explain
↓
Update Knowledge
```

AI 可以高度自主地执行实现工作，但关键系统认知不能完全丢失。人类应始终能理解目标、系统边界、主要数据流和重要决策。

## Core Principles

- Human owns goals.
- AI may own implementation.
- Important assumptions must be challenged.
- Architecture understanding should not be outsourced completely.
- Verification depth depends on task risk.
- Prefer reusable workflows over one-off prompting.
- Research should prefer search and primary sources when appropriate.
- Personal AI OS is continuously evolving.

## Information Layers

| Layer | Changes | Authoritative sources |
| --- | --- | --- |
| Stable | 慢：协作哲学、职责、原则与边界 | [AI_PROFILE.md](./AI_PROFILE.md)、[CODEX.md](./CODEX.md)、[CHATGPT.md](./CHATGPT.md)、[RULES.md](./RULES.md) |
| Dynamic | 快：模型、Skill、工具状态与当前选择 | [MODELS.md](./MODELS.md)、[SKILLS.md](./SKILLS.md) |

Workflow 和 Prompt 引用这些原则与配置，不复制维护同一事实。

## Quick Navigation

- [AI Profile](./AI_PROFILE.md)
- [Codex](./CODEX.md)
- [ChatGPT](./CHATGPT.md)
- [Models](./MODELS.md)
- [Skills](./SKILLS.md)
- [Workflows](./WORKFLOWS.md)
- [Prompts](./PROMPTS.md)
- [Rules](./RULES.md)
- [Changelog](./CHANGELOG.md)

## Current Workflow

| Task | Default route |
| --- | --- |
| Discussion | Normally ChatGPT |
| Research | Prefer ChatGPT with the Research workflow |
| Implementation | Normally Codex |
| Project development | Normally Codex |
| Repository work | Normally Codex |
| Long-term knowledge | Personal AI OS or Research OS |

这些是默认路由，不是绝对规则。当前明确指令和任务条件可以改变选择。

## How to Maintain

### 新模型成为默认模型

更新 [MODELS.md](./MODELS.md)、本页的 Current Setup，以及 [CHANGELOG.md](./CHANGELOG.md)。模型事实只在 MODELS.md 维护，本页仅显示当前选择。

### 新 Skill

只更新 [SKILLS.md](./SKILLS.md)；确认真实可用后再登记。

### AI Coding 工作方式改变

更新 [CODEX.md](./CODEX.md)、[workflows/ai-coding.md](./workflows/ai-coding.md) 和 [CHANGELOG.md](./CHANGELOG.md)，并保持协议与执行流程职责分离。

### 新 Prompt

先确认它确实是新的 reusable pattern，而不是已有 Prompt 的变体或一次性任务。优先修改已有 Prompt，避免 Prompt Library 无限膨胀。

## Roadmap

未来可按实际需要增加 `scripts/`，用于同步 Agent 配置、生成 `AGENTS.md`、验证链接、检查模型条目时效或生成 Dashboard。当前版本不实现自动化。
