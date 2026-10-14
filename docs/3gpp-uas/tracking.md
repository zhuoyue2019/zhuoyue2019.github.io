# 3GPP UAS 跟踪动态

> 长期跟踪 3GPP UAS（含 Rel-20 ISAC for UAV）标准进展。**基线**：《3GPP Release 20 ISAC for UAV 深度研究报告》v1.0（2026-09-09，数据截至 TSG#113）。本页每月检查更新一次。
>
> 版本：v1.1 ｜ 更新：2026-10-14

## 里程碑时间表

| 时间 | 会议 | 关键事项 | 状态 |
|------|------|----------|------|
| 2026-09 | TSG#113 | Stage 2 冻结 | ✅ 已完成（基线） |
| 2026-12 | TSG#114 | Stage 3 进展检查点 | ⏳ 待跟踪 |
| 2027-03 | TSG#115 | **Stage 3 冻结**（RAN 规范） | ⏳ 待跟踪 |
| 2027-06 | TSG#116 | **ASN.1 / OpenAPI 冻结** | ⏳ 待跟踪 |

## 规范版本 Watchlist

| 文档 | 标题 | 基线版本（2026-09） | 最新检查（2026-10-08） |
|------|------|---------------------|------------------------|
| TR 38.765 | Study on ISAC for NR | v20.0.0（2026-06 发布） | v20.0.0，无变化 |
| TR 23.700-14 | Study on architecture for ISAC（FS_Sensing_ARC） | 研究完成（2026-03） | v20.0.0 |
| TS 22.137 | Service requirements for ISAC | 已冻结（Rel-19） | v21.0.0（已出 Rel-21 版本） |
| TR 22.837 | Feasibility Study on ISAC | v19.4.0 | v19.4.0，无变化 |
| TS 23.501 | 5GS 架构（Sensing-ARC 修改目标） | SP-260297 进行中 80% | v20.3.0 |
| TS 23.502 | 5GS 流程（Sensing-ARC 修改目标） | SP-260297 进行中 80% | v20.2.0 |
| RP-261566 | New WID on ISAC for NR（中国电信牵头） | RAN#112 批准 | 通过会议新闻跟踪 |

## 关键待解问题

- [ ] **Level D 目标级上报**：待 SA3 隐私安全裁定（最大不确定性）
- [ ] **Sensing-ARC 规范完成度**：2026-06 为 80%，预期 2026-09 完成——待确认
- [ ] **配套规范**：FS_Sensing_SEC（安全）、FS_Sensing_CH（计费）、FS_Sensing_OAM、Sensing-CT 进展
- [ ] **多站协同**：Rel-20 明确不做 inter-gNB 协调，6G/厂商私有方案动态

## 跟踪日志

### 2026-10-13 —— R19 冻结，R20 全面转向（短评）
- R19 冻结：2025 年 12 月 TSG 全会（巴尔的摩，RAN/SA/CT）宣布 R19 规范冻结，此后只接受实现/测试中发现的问题修正（来源：urgentcomm《3GPP completes Release 19, while progress begins on 6G work》）
- R20 全面启动：各工作组转向 R20，重点为 6G 研究活动；R20 分 5G-Advanced 特性增强 + 6G 研究两条线并行
- 对本跟踪线：ISAC 业务需求侧（TS 22.137 等 R19 部分）已定型；无人机感知载体为 R20 ISAC for NR（TR 38.765、RP-261566 中国电信牵头 WID），按既有里程碑推进（2026-12 Stage 3 检查点 → 2027-03 Stage 3 冻结 → 2027-06 ASN.1/OpenAPI 冻结）
- 影响：基线（深度报告 v1.0）中引用 R19 冻结版本规范的内容视为稳定；月度检查重点不变；Level D 目标级上报待 SA3 裁定继续跟踪
- 完整短评审阅稿：本地 workspace（`3gpp-uas-tracking/短评_R19冻结与R20动向_20261013.md`），2026-10-13 已获审阅通过

### 2026-10-08 —— 建立跟踪
- 以附件报告 v1.0 为基线入库（[深度报告](isac-for-uav.md)）
- 建立本跟踪页与月度检查机制
- 基线核对：TR 38.765 当前仍为 v20.0.0，与报告一致

---

**本系列**：[总览](index.md) · [关键规范清单](specs.md) · [Rel-20 ISAC 深度报告](isac-for-uav.md) · [跟踪动态](tracking.md)
