# FreeRTOS Study Notes
# FreeRTOS 学习笔记

> In-depth study notes based on FreeRTOS source code, built for embedded engineers in production roles.
> 基于 FreeRTOS 源码的深度学习笔记，面向工作岗位上的嵌入式工程师。

---

## Features | 特点

- **Source-First** — Every critical code path is traced line by line
- **Visual** — Complex flows are illustrated with diagrams (prompts included)
- **Practical** — Concepts + Source + Tuning Guide + Pitfalls & Solutions

---

## Content | 内容

| Chapter | Module | Description |
|---------|--------|-------------|
| 0 | [Basics](./0_Basics/) | 基础概念速览 |
| 1 | [Tasks](./1_Tasks/) | 任务管理 · Task Management |
| 2 | [Scheduler](./2_Scheduler/) | 调度器原理 · Scheduler Internals |
| 3 | [Queue](./3_Queue/) | 队列实现 · Queue Implementation |
| 4 | [Memory](./4_Memory/) | 内存管理 · Memory Management |
| 5 | [Sync](./5_Sync/) | 同步原语 · Synchronization Primitives |
| 6 | [Notifications](./6_Notifications/) | 事件标志组 & 任务通知 · Event Groups & Task Notifications |
| 7 | [Time](./7_Time/) | 时间管理 · Time Management |
| 8 | [Interrupt](./8_Interrupt/) | 中断管理 · Interrupt Management |
| 9 | [Port](./9_Port/) | 移植层 · Porting Layer |

---

## Writing Principles | 写作原则

- **紧贴源码** — 关键代码逐行 trace
- **图文并茂** — 复杂流程配图（用 prompt 预留）
- **实用主义** — 概念 + 源码 + 调参 + 踩坑
- **无幻觉** — 所有解释经 FreeRTOS v11.1.0 源码验证

---

## Chapter Details | 章节详情

See [docs/structure.md](./docs/structure.md) for the full outline.

---

## Source Reference | 源码参考

All source traces are based on **FreeRTOS v11.1.0**.
FreeRTOS Kernel: https://github.com/FreeRTOS/FreeRTOS-Kernel
