# Personal AI OS

> 本文件是 Personal AI OS 的总览和入口。
> 开始协作时先读本页；具体配置以本页链接的文件为唯一维护源。

My personal operating system for working with AI.

Status: Active

Version: 0.1

## Current Setup（当前配置）

| Category | Current Default |
| --- | --- |
| Primary Coding Agent | Codex |
| Primary General AI | ChatGPT |
| Default Coding Model | To be maintained |
| Default Research Model | To be maintained |
| Primary Knowledge Format | Markdown |
| Version Control | Git |

具体模型以 [MODELS.md](./MODELS.md) 为准。

`To be maintained` 表示尚未确定，需要以后根据实际使用结果填写。

## Default Operating Loop（默认工作循环）

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

AI 可以自主完成大量实现工作，但人类仍应掌握目标、系统边界、主要数据流和重要决策。

## Core Principles（核心原则）

- 人类决定目标、方向和最终验收标准。
- AI 可以负责具体实现，但不能擅自改变目标。
- 重要前提必须先核验，不能为了迎合用户而默认接受。
- 人类不必理解每一行代码，但应掌握关键系统结构。
- 任务风险越高，验证越深入。
- 优先复用稳定的 Workflow，不为每次任务重新发明做法。
- 研究任务优先检索一手资料和官方来源。
- Personal AI OS 会随着实际使用持续更新。

## Information Layers（信息分层）

| Layer | Changes | Authoritative sources |
| --- | --- | --- |
| Stable（稳定层） | 很少变化：协作哲学、职责、原则与边界 | [AI_PROFILE.md](./AI_PROFILE.md)、[CODEX.md](./CODEX.md)、[CHATGPT.md](./CHATGPT.md)、[RULES.md](./RULES.md) |
| Dynamic（动态层） | 经常变化：模型、Skill、工具状态与当前选择 | [MODELS.md](./MODELS.md)、[SKILLS.md](./SKILLS.md) |

Workflow 和 Prompt 只引用这些原则与配置，不在多个文件重复维护同一事实。

## How to Use（怎么使用）

- 快速了解当前工作方式：读本页。
- 让新的 AI 开始工作：读本页、[AI_PROFILE.md](./AI_PROFILE.md) 和本次任务对应的 Workflow。
- 更新模型或 Skill：只修改对应的动态 Registry，再按维护规则更新 Dashboard 或 Changelog。

## Key Terms（关键术语）

- Single Source of Truth：同一项信息只在一个指定文件中维护，避免多个版本互相冲突。
- Registry：当前可用项目的清单，例如模型清单和 Skill 清单。
- Workflow：一类任务可以重复使用的执行流程。
- Prompt：发给 AI 的任务启动说明。
- Agent：能够读取上下文、使用工具并执行多步任务的 AI。

## Quick Navigation（快速导航）

- [AI Profile](./AI_PROFILE.md)
- [Codex](./CODEX.md)
- [ChatGPT](./CHATGPT.md)
- [Models](./MODELS.md)
- [Skills](./SKILLS.md)
- [Workflows](./WORKFLOWS.md)
- [Prompts](./PROMPTS.md)
- [Rules](./RULES.md)
- [Changelog](./CHANGELOG.md)

## Current Workflow（默认任务分工）

| Task | Default route |
| --- | --- |
| Discussion | 通常使用 ChatGPT |
| Research | 通常使用 ChatGPT，并采用 Research Workflow |
| Implementation | 通常使用 Codex |
| Project development | 通常使用 Codex |
| 代码仓库工作 | 通常使用 Codex |
| Long-term knowledge | Personal AI OS 或 Research OS |

这些只是默认选择。当前明确指令和实际任务条件始终可以覆盖它们。

## How to Maintain（怎么维护）

### 新模型成为默认模型

更新 [MODELS.md](./MODELS.md)、本页的 Current Setup，以及 [CHANGELOG.md](./CHANGELOG.md)。模型事实只在 MODELS.md 维护，本页仅显示当前选择。

### 新 Skill

只更新 [SKILLS.md](./SKILLS.md)；确认真实可用后再登记。

### AI Coding 工作方式改变

更新 [CODEX.md](./CODEX.md)、[workflows/ai-coding.md](./workflows/ai-coding.md) 和 [CHANGELOG.md](./CHANGELOG.md)，并保持协议与执行流程职责分离。

### 新 Prompt

先确认它确实是新的 reusable pattern，而不是已有 Prompt 的变体或一次性任务。优先修改已有 Prompt，避免 Prompt Library 无限膨胀。

## Roadmap（未来可做）

未来可按实际需要增加 `scripts/`，用于同步 Agent 配置、生成 `AGENTS.md`、验证链接、检查模型条目时效或生成 Dashboard。当前版本不实现自动化。
