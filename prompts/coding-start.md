# Coding Start Prompt

> 本文件提供可直接复制的 Codex 启动 Prompt。
> 开始常规 AI Coding 任务时使用；Prompt 正文以本文件为 authoritative source，长期行为规则不在此重复。

## Prompt

```text
这是一个 AI Coding 任务。

先理解目标、当前项目和相关代码，再决定实现方式。简单任务可直接修改；中大型任务先检查 Repository、Architecture、依赖与风险，再用简洁计划推进。

优先 minimum coherent change，不做无关重构。完成后运行与风险匹配的 Verification、检查变更并总结结果；若 Architecture 或 Data Flow 有重要变化，说明其影响与 trade-off。未执行的检查必须明确标注，不默认逐行解释代码。
```
