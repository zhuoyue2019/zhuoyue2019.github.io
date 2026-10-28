# 标准深入理解

> ELI5 图解版：把 3GPP MCX 系列标准逐条读薄，用大白话讲明白，关键流程配流程图。每一篇都基于指定版本的原文逐条核实，条款编号可回查原文。

## 怎么读

- 每篇先讲“一句话是什么”，再讲“它要解决什么问题”，然后是核心概念大白话、关键流程、边界（它不管什么）、往下读的路径。
- 文中 `[§x.y]` 指向对应标准原文的条款号；版本号以每篇页首标明的基线为准。
- Stage 1 只规定“要什么”，不管“怎么做”：架构在 Stage 2（TS 23 系列），协议在 Stage 3（TS 24 系列）。

## 篇目

| 标准 | 标题 | 基线版本 | 状态 |
| :--- | :--- | :--- | :--- |
| **TS 22.280** | [Mission Critical Services Common Requirements (MCCoRe)，任务关键型服务通用业务需求](22280.md) | Rel-20 v20.2.0 | ✅ 已发布（2026-10-28） |
| **TS 22.179** | [Mission Critical Push To Talk (MCPTT)，关键型按讲对讲](22179.md) | Rel-20 v20.0.0 | ✅ 已发布（2026-10-28） |
| **TS 22.281** | [Mission Critical Video (MCVideo)，关键型视频](22281.md) | Rel-19 v19.0.0 | ✅ 已发布（2026-10-28） |
| **TS 22.282** | [Mission Critical Data (MCData)，关键型数据](22282.md) | Rel-19 v19.0.0 | ✅ 已发布（2026-10-28） |
| **TS 23.280** | [Mission Critical Services Common Functional Architecture，MCX 通用功能架构](23280.md) | Rel-20 v20.5.1 | ✅ 已发布（2026-10-28） |
| **TS 23.379** | [Mission Critical Push To Talk (MCPTT) functional architecture and information flows，MCPTT 功能架构](23379.md) | Rel-20 v20.4.0 | ✅ 已发布（2026-10-28） |
| **TS 23.281** | [Functional architecture and information flows to support Mission Critical Video，MCVideo 功能架构](23281.md) | Rel-20 v20.5.1 | ✅ 已发布（2026-10-28） |
| **TS 23.282** | [Functional architecture and information flows to support mission critical data，MCData 功能架构](23282.md) | Rel-20 v20.3.1 | ✅ 已发布（2026-10-28） |

## 后续计划
- 第三批：Stage 3 协议与安全篇——TS 24.379 / 24.281 / 24.282、TS 24.483 / 24.484、TS 33.180（安全）。
- 另：TS 22.289（5G MBS 承载）、TS 22.283 / 23.283（LMR 互通）待补入清单。
