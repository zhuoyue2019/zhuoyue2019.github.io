# 关键规范清单

> 版本：v1.2 ｜ 更新：2026-10-14 ｜ 数据基线：TSG#113（2026-09）；ISAC 家族版本号来自月度跟踪，每月 8/23 日检查更新

## 一、UAS 经典规范（R15–R17）

| 规范编号 | 标题 | 阶段 | 说明 |
|----------|------|------|------|
| TR 36.777 | Study on Enhanced LTE Support for Aerial Vehicles | R15 研究 | LTE 服务空中终端的空口研究报告 |
| TR 22.829 | Study on supporting UAS connectivity, Identification and tracking | R16 研究 | UAS 可行性研究，需求的源头 |
| TS 22.125 | Unmanned Aerial System (UAS) support in 3GPP | R17 业务需求 | Stage 1：UAS 业务与 KPI 需求 |
| TS 23.256 | Support of Uncrewed Aerial Systems (UAS) connectivity, identification and tracking | R17 系统架构 | Stage 2：5GS 如何支持 UAS，含 USS 对接 |

## 二、ISAC 规范家族（Rel-19–Rel-20）

| 规范编号 | 标题 | 版本（2026-10） | 说明 |
|----------|------|----------------|------|
| TR 38.765 | Study on ISAC for NR | v20.0.0 | RAN1/RAN3 Rel-20 研究：能不能测、测多准；2026-06 RAN#112 批准发布 |
| TR 23.700-14 | Study on architecture for ISAC（FS_Sensing_ARC） | v20.0.0 | SA2 架构研究；2026-03 完成 |
| TS 22.137 | Service requirements for ISAC | v21.0.0 | SA1 业务需求，Rel-19 已冻结 |
| TR 22.837 | Feasibility Study on ISAC | v19.4.0 | SA1 可行性研究 |
| TS 23.501 | System architecture for the 5G System | v20.3.0 | 5GS 架构；Sensing-ARC（SP-260297）修改目标 |
| TS 23.502 | Procedures for the 5G System | v20.2.0 | 5GS 流程；Sensing-ARC（SP-260297）修改目标 |
| RP-261566 | New WID on ISAC for NR | —（立项） | RAN 规范项，中国电信牵头，46 家公司支持；Stage 3 规范化进行中 |

## 三、R18/R19 UAS 增强速览

> 来源：TR 21.918《Release 18 Description》目录（8.1–8.4）、TS 38.300 §16.18、2024-09 TSG 全会纪要

| Release | 工作项 | 内容要点 |
|---------|--------|----------|
| R18 | Architecture for UAV and UAM Phase 2 | SA2 架构第二阶段：无人机与城市空中交通（UAM）架构增强 |
| R18 | Architecture for UAS Applications, Phase 2 | SA6 应用层架构第二阶段 |
| R18 | NR support for UAV（空口） | 把 R15 LTE 的 Aerial 特性搬到 NR：高度门限触发的测量上报、高度上报、按高度区分的配置、**多小区同时满足触发条件的干扰检测**、飞行路径信息上报（UE→NG-RAN、切换时源→目标 gNB）、含水平/垂直速度的位置上报、PC5 口传输 BRID/DAA 消息、Aerial UE 签约识别与授权（TS 23.502 §5.2.3.3.1） |
| R18 | Enhanced LTE Support for UAV | LTE 侧增强 |
| R19 | UAS Phase 3（SA2） | 探测与避让（detect and avoid）能力增强 + 通信增强（2024-09 TSG SA 全会立项方向） |
| R19 | UAV enhancements（RAN） | 公共安全场景的无人机增强（R19 规划议题） |

一句话演进：R15（LTE 空中终端）→ R17（5GS 架构+USS 对接）→ R18（NR 对齐 LTE + 高度/干扰/航径等空口增强）→ R19（探测避让 Phase 3）→ R20（ISAC for UAV，基站直接感知非合作目标）。

## 四、各规范核心章节摘录

- **TR 36.777（R15 研究）**：识别了 LTE 服务空中终端的三大问题——上下行干扰（高空视距传播导致）、移动性（频繁切换/无线链路失败）、空中 UE 识别；结论直接催生 R15 LTE Aerial 特性（高度测量上报、飞行路径上报、签约识别）。
- **TR 22.829（R16 研究）**：UAS 用例全集与需求可行性——C2 通信、Remote ID、USS 对接三大支柱在此定型，是 TS 22.125 的需求源头。
- **TS 22.125（R17 业务需求，Stage 1）**：C2 链路 QoS 分级（时延 10ms~5s、可靠 99%~99.99%、速率 50~300km/h，按控制模式区分）、Remote ID 业务需求、USS 互通需求、UAS 定位需求。
- **TS 23.256（R17 系统架构，Stage 2）**：UAS NF 网元、USS 发现与选择、C2 通信三种模式（直连/网络辅助/UTM 导航）、UAV-控制器配对、基于网络的 Remote ID 流程（无人机经 3GPP 网络向 USS 上报身份与位置）。

## 五、Remote ID：3GPP 与 ASTM F3411 的对应关系

ASTM F3411 定义了两类 Remote ID 实现，二者是**互补**而非替代关系：

| 实现方式 | 标准 | 机制 |
|----------|------|------|
| Broadcast RID（广播式） | ASTM F3411 | 无人机通过蓝牙/Wi-Fi 直接广播身份、位置、速度、方向；接收方可为普通智能手机；不依赖蜂窝网络 |
| Network RID（网络式） | ASTM F3411（Net-RID 服务提供方/展示提供方角色，USS 互操作） | 无人机经无线连接向 USS 上报，USS 聚合后向展示应用提供 |
| Network-based Remote ID | 3GPP TS 22.125（需求）/ TS 23.256（架构） | 无人机经 **3GPP 网络**向 USS 上报身份与位置——即 ASTM Network RID 中"无人机→网络→USS"这一段的蜂窝承载实现 |

对应关系：**3GPP 解决的是 Network RID 的"空口+核心网"段**（UAV→PLMN→USS），ASTM F3411 定义的是端到端框架（含广播式和 USS 间互操作）。做合规产品时，广播式按 F3411 做，网络式需同时满足 F3411 的 USS 接口与 3GPP 的网络流程。

!!! note "版本说明"
    ISAC 家族版本号与 [跟踪动态](tracking.md) 的 Watchlist 同步，具体章节以 [3GPP 官网](https://www.3gpp.org) 发布版本为准。

---

**本系列**：[总览](index.md) · [关键规范清单](specs.md) · [Rel-20 ISAC 深度报告](isac-for-uav.md) · [跟踪动态](tracking.md)
