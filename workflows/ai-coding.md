# AI Coding Workflow

> 本文件定义长期使用的 AI Coding 执行流程。
> 进行软件开发或 Repository 修改时应读取；流程步骤以本文件为 authoritative source，Codex 的行为边界以 [CODEX.md](../CODEX.md) 为准。

## Purpose

让 AI 端到端承担大量实现工作，同时让人类继续拥有项目所需的系统级理解与最终验收权。

## Process

```text
Goal definition
↓
Context acquisition
↓
Repository understanding
↓
Solution design
↓
AI implementation
↓
Automated verification
↓
Human outcome validation
↓
Architecture sync
```

### Goal definition

明确交付物、成功条件、范围和风险边界。简单任务不需要额外仪式；大任务应先消除会改变 Architecture 的歧义。

### Context acquisition and Repository understanding

检查相关文件、现有约定、依赖、测试与工作区状态。先理解已有系统，再决定修改方式。

### Solution design and implementation

选择支持当前目标的 minimum coherent change。AI 可以自主编码、重构局部实现与补充必要文档，但不扩大授权范围。

### Verification and validation

AI 根据风险执行自动化检查并如实报告结果；Human 从需求与实际体验角度验收 outcome。高风险变更需要更深入的回归与边界检查。

### Architecture sync

重要变更后，更新人类对系统结构的认知。同步内容应聚焦 system purpose、modules、APIs、Data Flow、important dependencies 与 major design decisions。

## Ownership Principle

> Human does not need to understand every line of AI-generated code. Human should understand the system at the level required to continue owning the project.

这意味着解释应覆盖影响后续决策的结构，而不是默认逐行复述实现。

## Outputs

- 可验证的代码或配置变更
- 与风险匹配的 Verification 结果
- 简洁的影响说明
- 必要时更新的长期知识
