<p align="center">
  <img src="https://img.shields.io/badge/FreeRTOS-v11.1.0-26a269?style=flat-square&logo=freertos&logoColor=white" alt="FreeRTOS">
  <img src="https://img.shields.io/badge/Platform-ARM%20Cortex--M-00979d?style=flat-square" alt="Platform">
  <img src="https://img.shields.io/badge/Base-Freertos%20Kernel-26a269?style=flat-square&logo=freertos" alt="Kernel">
  <img src="https://img.shields.io/badge/License-MIT-ff6b6b?style=flat-square" alt="License">
</p>

<div align="center">

# FreeRTOS 学习笔记

*A14 Cortex · 源码驱动 · 实用主义*

<!-- Language Toggle — placed after title, not at top of file -->
<p align="right" style="margin-top:-40px">
  <a href="README_EN.md" style="
    display: inline-flex;
    align-items: center;
    gap: 6px;
    padding: 5px 14px;
    background: linear-gradient(135deg, #1a1a2e, #16213e);
    border: 1px solid #3a7bd5;
    border-radius: 20px;
    color: #3a7bd5;
    text-decoration: none;
    font-size: 12px;
    font-family: -apple-system, sans-serif;
    font-weight: 600;
    transition: all 0.2s ease;
  " onmouseover="this.style.background='#3a7bd5'; this.style.color='#fff'; this.style.boxShadow='0 0 12px rgba(58,123,213,0.5)'"
  onmouseout="this.style.background='linear-gradient(135deg, #1a1a2e, #16213e)'; this.style.color='#3a7bd5'; this.style.boxShadow='none'">
    🌐 English
  </a>
</p>

</div>

---

> 🔍 **基于 FreeRTOS 源码的深度学习笔记**，面向工作岗位上的嵌入式工程师。每一行关键代码都有分析，每一个概念都有实战支撑。

---

## ⚡ 核心特色

<div align="center">

|:--|:--|:--|
| **🔬 紧贴源码** | **🎨 图文并茂** | **🛠️ 实用主义** |
| 关键代码逐行 trace | 复杂流程配图（prompt 预留） | 概念 + 源码 + 调参 + 踩坑 |

</div>

- ✅ 源码 trace 基于 **FreeRTOS v11.1.0** 逐行验证
- ✅ 覆盖 10 大核心模块，**无 AI 幻觉**
- ✅ 调参指南 + 踩坑实录来自真实踩坑经验

---

## 📖 内容导览

| 章节 | 模块 | 描述 |
|:----:|------|------|
| 0 | [Basics](./0_Basics/) | 基础概念速览 |
| 1 | [Tasks](./1_Tasks/) | 任务管理 |
| 2 | [Scheduler](./2_Scheduler/) | 调度器原理 |
| 3 | [Queue](./3_Queue/) | 队列实现 |
| 4 | [Memory](./4_Memory/) | 内存管理 |
| 5 | [Sync](./5_Sync/) | 同步原语 |
| 6 | [Notifications](./6_Notifications/) | 事件标志组 & 任务通知 |
| 7 | [Time](./7_Time/) | 时间管理 |
| 8 | [Interrupt](./8_Interrupt/) | 中断管理 |
| 9 | [Port](./9_Port/) | 移植层 |

---

## ✍️ 写作原则

- **紧贴源码** — 关键代码逐行 trace
- **图文并茂** — 复杂流程配图（用 prompt 预留）
- **实用主义** — 概念 + 源码 + 调参 + 踩坑
- **无幻觉** — 所有解释经 FreeRTOS v11.1.0 源码验证

---

## 🗂️ 章节详情

详见 [docs/structure.md](./docs/structure.md)

---

## 📚 源码参考

所有源码 trace 均基于 **FreeRTOS Kernel v11.1.0**

<p align="center">
<a href="https://github.com/FreeRTOS/FreeRTOS-Kernel"><img src="https://img.shields.io/badge/GitHub-FreeRTOS%20Kernel-26a269?style=flat-square&logo=github" alt="GitHub"></a>
<a href="https://www.freertos.org/"><img src="https://img.shields.io/badge/Docs-FreeRTOS%20Official-26a269?style=flat-square&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9IiMyNmEyNjkiIHN0cm9rZS13aWR0aD0iMiI+PHBhdGggZD0iTTEyIDJDMCAyIDIgOCA2IDIgMTJjMCA1LjUgMyA4IDYgMTFhMTIgMTIgMCAwIDAgMTEuOTk5LTEyYy0zLjAwNS0wLjAwMi02LTYuNS02LTEyLjAwMiIgLz48L3N2Zz4=" alt=""></a>
</p>

---

<p align="center">
  <em>Made for embedded engineers, by embedded engineers.</em>
</p>
