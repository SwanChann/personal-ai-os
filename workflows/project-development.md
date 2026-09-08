# Project Development Workflow

> 本文件定义从零搭建项目或交付大型功能的端到端流程。
> 网站、Research OS、AI 系统、工具、App 或大型功能启动时应读取；项目阶段以本文件为 authoritative source。

## Process

```text
Problem
↓
Requirements
↓
Architecture
↓
Milestones
↓
Implementation
↓
Verification
↓
Iteration
↓
Maintenance
```

## Operating Principle

先定义问题、使用者、成功条件与约束，再设计 Architecture。采用：

> simplest architecture that supports expected evolution

不要在证据不足时追求完美架构，也不要用临时拼接阻断可预见的近期演进。

## Milestones and Implementation

Milestone 应产生可检查的 outcome。按依赖顺序增量实现，每个主要阶段完成后验证，再进入下一阶段。计划是可调整的工作假设，不是不能改变的承诺。

## Maintenance

交付时保留足够的 Architecture、Data Flow、依赖、运行方式和技术债信息，使项目可以由未来的人类或 Agent 继续维护。具体 coding 执行使用 [AI Coding Workflow](./ai-coding.md)。
