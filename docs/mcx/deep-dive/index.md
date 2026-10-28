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
| **TS 24.379** | [Mission Critical Push To Talk (MCPTT) call control protocol，MCPTT 呼叫控制协议](24379.md) | Rel-20 v20.1.0 | ✅ 已发布（2026-10-28） |
| **TS 24.281** | [Mission Critical Video (MCVideo) call control protocol，MCVideo 呼叫控制协议](24281.md) | Rel-20 v20.1.0 | ✅ 已发布（2026-10-28） |
| **TS 24.282** | [Mission Critical Data (MCData) signalling control protocol，MCData 信令控制协议](24282.md) | Rel-20 v20.1.0 | ✅ 已发布（2026-10-28） |
| **TS 24.483** | [Mission Critical Services (MCS) configuration management，MC 配置管理对象](24483.md) | Rel-20 v20.1.0 | ✅ 已发布（2026-10-28） |
| **TS 24.484** | [Mission Critical Services (MCS) configuration management procedures，MC 配置管理流程](24484.md) | Rel-20 v20.1.0 | ✅ 已发布（2026-10-28） |
| **TS 33.180** | [Security of the Mission Critical (MC) service，关键任务通信安全](33180.md) | Rel-20 v20.1.0 | ✅ 已发布（2026-10-28） |
| **TS 22.289** | [Mobile Communication System for Railways，铁路通信业务需求](22289.md) | Rel-19 v19.0.1 | ✅ 已发布（2026-10-28） |
| **TS 23.283** | [Mission Critical Communication Interworking with Land Mobile Radio Systems，MCX 与 LMR 互通架构](23283.md) | Rel-20 v20.1.0 | ✅ 已发布（2026-10-28） |
| **TS 23.289** | [Mission Critical services over 5G System，MCX over 5GS 架构](23289.md) | Rel-20 v20.3.0 | ✅ 已发布（2026-10-28） |
| **TS 24.380** | [Mission Critical Push To Talk (MCPTT) media plane control，MCPTT 媒体面控制](24380.md) | Rel-19 v19.1.0 | ✅ 已发布（2026-10-28） |
| **TS 24.481** | [Mission Critical Services (MCS) group management，MC 组管理](24481.md) | Rel-19 v19.1.0 | ✅ 已发布（2026-10-28） |
| **TS 24.482** | [Mission Critical Services (MCS) identity management，MC 身份管理](24482.md) | Rel-19 v19.1.0 | ✅ 已发布（2026-10-28） |
| **TS 24.581** | [Mission Critical Video (MCVideo) media plane control，MCVideo 媒体面控制](24581.md) | Rel-19 v19.2.0 | ✅ 已发布（2026-10-28） |
| **TS 24.582** | [Mission Critical Data (MCData) media plane control，MCData 媒体面控制](24582.md) | Rel-19 v19.0.0 | ✅ 已发布（2026-10-28） |
| **TR 22.819** | [Study on Maritime Communication Services over 3GPP system，海事通信服务可行性研究](22819.md) | Rel-16 v16.2.0 | ✅ 已发布（2026-10-28） |
| **TR 23.790** | [Study on application architecture for the Future Railway Mobile Communication System (FRMCS); Stage 2，FRMCS 应用架构研究](23790.md) | Rel-15 v15.0.0 | ✅ 已发布（2026-10-28） |
| **TR 24.980** | [Minimum requirements for support of MCPTT Service over the Gm reference point，Gm 参考点 MCPTT 最低要求](24980.md) | Rel-16 v16.0.0 | ✅ 已发布（2026-10-28） |

## 后续计划
- MCX 基线清单 25 条（规范类 TS 22 条 + 研究报告类 TR 3 条）已全部覆盖；下一步候选：ISAC for UAV 系列 ELI5 深读。
