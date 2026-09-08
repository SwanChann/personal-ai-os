# Models

> 本文件记录当前模型及其选择规则，属于经常更新的动态 Registry。
> 选择或评估模型时应读取；模型状态、用途和核验日期只在本文件维护。

## 模型清单

| Model | Provider | Main Role | Strength | Weakness | Default Use | Status | Last verified |
| --- | --- | --- | --- | --- | --- | --- | --- |
| GPT-5.6 Sol | To be maintained | To evaluate | To evaluate | To evaluate | To be maintained | To evaluate | Not verified |
| GPT-5.6 Astra | To be maintained | To evaluate | To evaluate | To evaluate | To be maintained | To evaluate | Not verified |
| Other / future models | To be maintained | To evaluate | To evaluate | To evaluate | To be maintained | To evaluate | Not verified |

状态说明：`To be maintained` 表示需要用户维护；`To evaluate` 表示尚未完成能力评估；`Not verified` 表示本项目尚未核验该信息。

## 当前默认模型

- Default Coding Model: To be maintained
- Default Research Model: To be maintained

README 只展示当前选择；模型评估和状态统一在本文件维护。

## 怎样选择模型

- 简单任务：优先选择推理成本较低、能够稳定完成任务的模型。
- 复杂编码：优先选择当前可用且可靠性最高的编码模型。
- 架构或困难推理：先提高推理深度，再考虑增加 Prompt 长度。
- 研究：搜索能力和来源质量与模型本身的推理能力同样重要。
- 选择前确认模型真实可用，不从命名推断能力。

## 怎样评估模型

后续评估至少覆盖推理、编码、指令遵循、Agent 能力、工具使用、长上下文可靠性、研究能力、响应速度、额度或成本，以及结果稳定性。

详细条目可从 [Model Entry Template](./templates/model-entry.md) 开始；只有经过实际评估的信息才应进入 Registry。
