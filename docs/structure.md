# FreeRTOS 学习笔记 - 内容结构规划

> 本仓库记录基于 FreeRTOS 源码的深度学习笔记，面向工作岗位上的嵌入式工程师。

---

## 目标读者

- 有一定 RTOS 使用经验
- 想深入理解内核原理
- 需要实战调参和排坑指南

---

## 核心原则

- **紧贴源码**：每一行关键代码都有分析
- **图文并茂**：复杂流程配图（图片位置用 prompt 代替）
- **实用主义**：概念 + 源码 + 调参 + 踩坑

---

## 内容结构

### 0_Basics/ — 基础概念
- 0.1 什么是 RTOS / 为什么需要
- 0.2 裸机与多线程的对比
- 0.3 FreeRTOS 架构总览
- 0.4 核心术语速查表

### 1_Tasks/ — 任务管理
- 1.1 概念：任务状态机、优先级、栈
- 1.2 API 速查：xTaskCreate / vTaskDelete / vTaskSuspend
- 1.3 源码解析：task.c 核心逻辑 trace
- 1.4 调参指南：栈大小怎么算、configMAX_PRIORITIES 设多少
- 1.5 踩坑实录：栈溢出怎么排查

### 2_Scheduler/ — 调度器
- 2.1 概念：抢占式 / 协作式 / 时间片
- 2.2 源码解析：vTaskSwitchContext trace
- 2.3 概念：PendSV 中断如何触发上下文切换
- 2.4 源码解析：Cortex-M 上下文切换原理
- 2.5 踩坑实录：调度器不启动 / 优先级反转

### 3_Queue/ — 队列
- 3.1 概念：FIFO / 消息传递 / 阻塞机制
- 3.2 API 速查：xQueueCreate / xQueueSend / xQueueReceive
- 3.3 源码解析：xQueueSend trace
- 3.4 中断安全队列：FromISR 版本
- 3.5 踩坑实录：队列死锁 / 阻塞超时设置

### 4_Memory/ — 内存管理
- 4.1 概念：五种 heap 策略对比表
- 4.2 对比详解：碎片 / 确定性 / 开销
- 4.3 调参指南：heap 大小怎么定
- 4.4 源码解析：pvPortMalloc / vPortFree trace
- 4.5 踩坑实录：内存碎片 / 对齐 / 泄漏

### 5_Sync/ — 同步原语
- 5.1 信号量、互斥量、计数信号量
- 5.2 API 速查：xSemaphoreCreate / xSemaphoreTake / xSemaphoreGive
- 5.3 源码解析：xSemaphoreTake trace
- 5.4 优先级继承：解决优先级反转
- 5.5 踩坑实录：死锁 / 忘记 Give / 递归互斥

### 6_Notifications/ — 事件标志组与任务通知
- 6.1 事件标志组概念（Event Groups）
- 6.2 事件标志组 API 速查
- 6.3 事件标志组踩坑实录
- 6.4 任务通知概念（Task Notifications）
- 6.5 任务通知 API 速查
- 6.6 任务通知踩坑实录

### 7_Time/ — 时间管理
- 7.1 vTaskDelay vs vTaskDelayUntil
- 7.2 Tick 中断机制
- 7.3 软件定时器 daemon（timer.c）
- 7.4 踩坑实录：延时精度 / 空转功耗

### 8_Interrupt/ — 中断管理
- 8.1 临界段：taskENTER_CRITICAL / taskEXIT_CRITICAL
- 8.2 FromISR 的意义：中断安全函数
- 8.3 中断嵌套规则（Cortex-M）
- 8.4 踩坑实录：中断里不能 delay / 过长临界段

### 9_Port/ — 移植层
- 9.1 移植层结构：portmacro.h
- 9.2 ARM Cortex-M 移植要点
- 9.3 Keil / IAR / GCC 差异
- 9.4 换芯片怎么改

---

## 每章写作模板

```markdown
## X.Y 章节名

### 概念（配图 prompt）
[IMAGE_PROMPT: 描述需要生成的图片内容]

### API 速查
```c
// 函数签名和说明
```

### 源码解析
```c
// 关键代码 trace
```

### 调参指南
| 参数 | 建议值 | 原因 |
|------|--------|------|

### 踩坑实录
**现象**：
**原因**：
**解决**：
```

---

## 图片 prompt 规范

需要配图时，使用以下格式：

```
[IMAGE_PROMPT: 描述生成图片的内容，包括元素、布局、文字说明]
```

生成时可将 `[IMAGE_PROMPT: ...]` 内容直接复制给图片生成 AI（如 DALL-E、Midjourney）获取对应图片。

### 常用图片类型

| 位置 | prompt 类型 |
|------|-------------|
| 状态机 | `[IMAGE_PROMPT: FreeRTOS task state machine diagram with states: Ready, Running, Blocked, Suspended, arrows showing transitions with conditions]` |
| 调度流程 | `[IMAGE_PROMPT: FreeRTOS scheduler flowchart showing task switching between Running and Ready states, with PendSV interrupt trigger]` |
| 内存布局 | `[IMAGE_PROMPT: FreeRTOS heap memory layout diagram showing allocated blocks, free blocks, header structures]` |
| 队列结构 | `[IMAGE_PROMPT: FreeRTOS queue data structure diagram showing head, tail, items, and read/write pointers]` |
| 中断嵌套 | `[IMAGE_PROMPT: ARM Cortex-M interrupt nesting diagram showing nested interrupts with priority levels]` |

---

## 更新记录

| 日期 | 更新内容 |
|------|----------|
| 2026-04-08 | 初始化结构规划文档 |
| 2026-04-08 | 新增第 9 章：事件标志组 + 任务通知（6 节） |
| 2026-04-08 | 源码 trace 全面基于 FreeRTOS v11.1.0 校正 |
