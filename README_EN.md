<!--language: en-US-->

<p align="center">
  <a href="README.md" style="
    display: inline-flex;
    align-items: center;
    gap: 6px;
    padding: 6px 16px;
    background: linear-gradient(135deg, #1a1a2e, #16213e);
    border: 1px solid #3a7bd5;
    border-radius: 20px;
    color: #3a7bd5;
    text-decoration: none;
    font-size: 13px;
    font-family: -apple-system, sans-serif;
    font-weight: 600;
    transition: all 0.2s ease;
  " onmouseover="this.style.background='#3a7bd5'; this.style.color='#fff'; this.style.boxShadow='0 0 12px rgba(58,123,213,0.5)'"
  onmouseout="this.style.background='linear-gradient(135deg, #1a1a2e, #16213e)'; this.style.color='#3a7bd5'; this.style.boxShadow='none'">
    🌐 中文
  </a>
</p>

---

<p align="center">
  <img src="https://img.shields.io/badge/FreeRTOS-v11.1.0-26a269?style=flat-square&logo=freertos&logoColor=white" alt="FreeRTOS">
  <img src="https://img.shields.io/badge/Platform-ARM%20Cortex--M-00979d?style=flat-square" alt="Platform">
  <img src="https://img.shields.io/badge/Base-Freertos%20Kernel-26a269?style=flat-square&logo=freertos" alt="Kernel">
  <img src="https://img.shields.io/badge/License-MIT-ff6b6b?style=flat-square" alt="License">
</p>

<div align="center">

# FreeRTOS Study Notes

*A14 Cortex · Source-Driven · Practical First*

</div>

---

> 🔍 **In-depth study notes based on FreeRTOS source code**, built for embedded engineers in production roles. Every critical code path is traced, every concept is backed by real-world experience.

---

## ⚡ Key Features

<div align="center">

| | | |
|:--|:--|:--|
| **🔬 Source-First** | **🎨 Visual** | **🛠️ Practical** |
| Line-by-line code trace | Diagrams for complex flows | Concepts + Source + Tuning + Pitfalls |

</div>

- ✅ All source traces verified against **FreeRTOS v11.1.0** line by line
- ✅ 10 core modules covered, **zero AI hallucinations**
- ✅ Tuning guides & pitfall stories from real production experience

---

## 📖 Content Overview

| Ch. | Module | Description |
|:---:|--------|-------------|
| 0 | [Basics](./0_Basics/) | Foundation Concepts |
| 1 | [Tasks](./1_Tasks/) | Task Management |
| 2 | [Scheduler](./2_Scheduler/) | Scheduler Internals |
| 3 | [Queue](./3_Queue/) | Queue Implementation |
| 4 | [Memory](./4_Memory/) | Memory Management |
| 5 | [Sync](./5_Sync/) | Synchronization Primitives |
| 6 | [Notifications](./6_Notifications/) | Event Groups & Task Notifications |
| 7 | [Time](./7_Time/) | Time Management |
| 8 | [Interrupt](./8_Interrupt/) | Interrupt Management |
| 9 | [Port](./9_Port/) | Porting Layer |

---

## ✍️ Writing Principles

- **Source-First** — Every critical code path is traced line by line
- **Visual** — Complex flows are illustrated with diagrams (prompts included)
- **Practical** — Concepts + Source + Tuning Guide + Pitfalls & Solutions
- **No Hallucinations** — All explanations verified against FreeRTOS v11.1.0 source

---

## 🗂️ Chapter Details

See [docs/structure.md](./docs/structure.md) for the full outline.

---

## 📚 Source Reference

All source traces are based on **FreeRTOS Kernel v11.1.0**

<p align="center">
<a href="https://github.com/FreeRTOS/FreeRTOS-Kernel"><img src="https://img.shields.io/badge/GitHub-FreeRTOS%20Kernel-26a269?style=flat-square&logo=github" alt="GitHub"></a>
<a href="https://www.freertos.org/"><img src="https://img.shields.io/badge/Docs-FreeRTOS%20Official-26a269?style=flat-square" alt="Official Docs"></a>
</p>

---

<p align="center">
  <em>Made for embedded engineers, by embedded engineers.</em>
</p>
