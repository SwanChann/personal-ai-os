# Skills

> 本文件记录本地已确认、日常较常用的 Skill，属于动态 Registry。
> 选择 Skill 时应读取；是否登记、默认级别和使用场景只在本文件维护。

## 常用 Skill 清单

| Skill | Category | Used By | Trigger | Purpose | Status |
| --- | --- | --- | --- | --- | --- |
| `make-agent-work-visible` | 协作表达 | Codex / Agent | 非简单任务需要清楚报告进度与结果 | 说明结果、依据、验证、未知项和下一步 | default |
| `project-state-navigator` | 项目状态 | Codex / Agent | 长期、多阶段、跨会话或计划可能变化 | 判断当前任务在整体项目中的位置，并维护项目状态 | default |
| `personal-writing-style` | 中文写作 | Codex / ChatGPT | 撰写或修改中文内容 | 使用简洁、直接、结果优先的表达方式 | active |
| `context-handoff` | 上下文交接 | Codex / Agent | 将长对话或多条工作流迁移到新会话 | 创建或读取完整的交接包 | active |
| `context-refresh` | 上下文整理 | Codex / Agent | 只需压缩当前上下文，不需要完整交接包 | 生成轻量的会话续接信息 | active |
| `plus-short-loop` | 执行控制 | Codex | 用户要求节省额度、缩小范围或完成即停 | 用短循环完成最小必要工作和验证 | active |
| `research-note-writer` | 研究写作 | Codex / ChatGPT | 编写中文研究笔记、教程或实验总结 | 形成聚焦、可复用的 Markdown 研究文档 | active |
| `research-frontier-scan` | 研究检索 | Codex / ChatGPT | 扫描近期论文、技术进展或研究方向 | 整理前沿证据和候选方向 | active |
| `research-question-framer` | 研究设计 | Codex / ChatGPT | 研究方向过于宽泛 | 收敛研究问题、目标和贡献表述 | active |
| `research-gap-idea` | 研究设计 | Codex / ChatGPT | 需要从资料中提出研究点或实验方向 | 把已有证据转化为可检验的研究候选 | active |
| `paper-deep-read` | 论文阅读 | Codex / ChatGPT | 深读一至三篇论文 | 提取论文主张、证据、限制和比较结果 | active |
| `literature-triage-matrix` | 文献整理 | Codex / ChatGPT | 比较一组已知论文 | 生成跨论文对照矩阵，而不是逐篇泛泛总结 | active |
| `weekly-research-review` | 研究管理 | Codex / ChatGPT | 周度研究回顾和下周规划 | 汇总进展、未闭环问题和下一步 | active |
| `slides-from-research` | 研究汇报 | Codex / ChatGPT | 把研究资料转成演示内容 | 生成幻灯片大纲或演示文稿草稿 | active |
| `pptx-builder` | 演示文稿 | Codex | 程序化创建、编辑或检查 PPTX | 处理 PowerPoint 文件并进行必要验证 | active |

本表于 2026-09-08 对照本地 Skill 目录核验。`active` 只表示本地可用且适合按需调用，不表示每次任务都会自动使用，也不证明依赖的外部服务一定可用。

## 怎样选择 Skill

任务与某个 Skill 明确匹配时，优先复用该 Skill，不重新设计一套相同流程。但 Skill 不是强制规则：质量不足、与任务不匹配或任务本身很简单时，可以不使用。

## 状态含义

- `experimental`：正在试用，还没有形成稳定用法。
- `active`：当前可用，按任务需要调用。
- `default`：满足触发条件时的默认选择。
- `deprecated`：不再推荐，等待替代或归档。
- `archived`：只保留历史价值，不属于当前配置。

新增条目可使用 [Skill Entry Template](./templates/skill-entry.md)。
