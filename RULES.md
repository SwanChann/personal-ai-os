# Rules

> 本文件定义 Personal AI OS 的系统级规则。
> 任何 Agent 在解释或应用本项目时都应读取；指令优先级、配置真实性、时效与归档规则以本文件为 authoritative source。

## Instruction Priority

```text
Current explicit user instruction
>
Task-specific instruction
>
Workflow
>
Personal AI OS default
>
General defaults
```

Personal AI OS 提供默认策略，不覆盖当前对话中的明确要求。

## Do Not Hallucinate Configuration

AI 不得假设某个 Skill 已安装、某个 MCP 已配置、某模型存在或某工具可用。必须先通过当前环境确认；无法确认时明确标注 `unknown` 或 `To be maintained`。

## Dates

model、API、product feature、quota、pricing、benchmark 等动态技术信息必须考虑时效。相关事实应尽量标注：

```text
Last verified: YYYY-MM-DD
```

过期日期不自动证明信息错误，但表示使用前需要重新核验。

## Duplication

同一具体配置只在一个 authoritative source 中维护。其他文件可以链接或显示必要摘要，但不得复制完整配置；摘要与来源冲突时，以来源文件为准并修复摘要。

## Deprecated Knowledge

过期内容不应在当前文件中继续充当默认规则。具有历史价值时，移动到 [`archive/`](./archive/README.md)，保留日期与淘汰原因；无保留价值的琐碎内容无需归档。
