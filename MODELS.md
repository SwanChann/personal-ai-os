# Models

> 本文件是当前模型信息与选择策略的动态 Registry。
> 选择或评估模型时应读取；具体模型状态、用途和验证日期只以本文件为 authoritative source。

## Model Registry

| Model | Provider | Main Role | Strength | Weakness | Default Use | Status | Last verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| GPT-5.6 Sol | To be maintained | To evaluate | To evaluate | To evaluate | To be maintained | To evaluate | Not verified |
| GPT-5.6 Astra | To be maintained | To evaluate | To evaluate | To evaluate | To be maintained | To evaluate | Not verified |
| Other / future models | To be maintained | To evaluate | To evaluate | To evaluate | To be maintained | To evaluate | Not verified |

## Current Defaults

- Default Coding Model: To be maintained
- Default Research Model: To be maintained

README 只展示这两个当前选择；评估依据与历史状态在本文件维护。

## Model Selection Principles

- 简单任务：prefer lower reasoning cost。
- 复杂 coding：prefer the strongest reliable coding model available。
- Architecture 或困难推理：先提高 reasoning depth，再考虑增加 Prompt 长度。
- Research：搜索能力和来源质量与 raw reasoning 同等重要。
- 选择前确认模型真实可用，不从命名推断能力。

## Model Evaluation

后续评估至少覆盖 reasoning、coding、instruction following、Agent capability、tool use、long-context reliability、research、latency、quota / cost 和 consistency。

详细条目可从 [Model Entry Template](./templates/model-entry.md) 开始；只有经过实际评估的信息才应进入 Registry。
