# 标准深入理解

> ELI5 图解版：把 3GPP UAS（无人机系统）系列标准逐条读薄，用大白话讲明白，关键流程配流程图。每一篇都基于指定版本的原文逐条核实，条款编号可回查原文。

## 怎么读

- 每篇先讲“一句话是什么”，再讲“它要解决什么问题”，然后是核心概念大白话、关键流程、边界（它不管什么）、往下读的路径。
- 文中 `[§x.y]` 指向对应标准原文的条款号；版本号以每篇页首标明的基线为准。
- Stage 1 只规定“要什么”，不管“怎么做”：架构在 Stage 2（TS 23 系列），安全在 TS 33 系列；TR 是研究报告，结论不是强制要求。

## 篇目

| 标准 | 标题 | 基线版本 | 状态 |
| :--- | :--- | :--- | :--- |
| **TS 22.125** | [Uncrewed Aerial System (UAS) support in 3GPP，UAS 业务需求](22125.md) | Rel-19 v19.2.0 | ✅ 已发布（2026-10-28） |
| **TS 23.256** | [Support of Uncrewed Aerial Systems (UAS) connectivity, identification and tracking，UAS 架构](23256.md) | Rel-19 v19.5.0 | ✅ 已发布（2026-10-28） |
| **TS 33.256** | [Security aspects of Uncrewed Aerial Systems (UAS)，UAS 安全](33256.md) | Rel-19 v19.2.0 | ✅ 已发布（2026-10-28） |
| **TR 36.777** | [Study on Enhanced Support for Aerial Vehicles，无人机增强支持研究](36777.md) | Rel-15 v15.0.0 | ✅ 已发布（2026-10-28） |

## 后续计划
- ISAC for UAV 系列（TS 22.137、TR 38.765、TR 23.700-14 等）按同款版式继续做。
- TR 38.821（无人机通信信道模型）最新版待核，核实后补入。
