> 版本：v1.3 ｜ 更新：2026-10-28 ｜ 数据基线：MCX 基线 v0.2（2026-10-16，2026-10-28 补同步）；基线口径已升至 Rel-20（2026-10-23 用户拍板）：已发布 Rel-20 的 14 条采用 Rel-20 版本，其余保留 Rel-19 最新；TS 22.280 Rel-21 v21.0.0 仅跟踪、不纳入基线

# 关键规范清单

## 一、3GPP MCX 关键规范清单

| 编号 | 标题 | Stage | Release | 版本 | 状态备注 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **TS 22.280** | Mission Critical Services Common Requirements (MCCoRe)（任务关键型服务通用业务需求） | Stage 1 | Rel-20 | v20.2.0 | MCX 三大业务（MCPTT/MCVideo/MCData）的通用需求总纲；Rel-21 v21.0.0 已出现（2026-10-02），仅跟踪 |
| **TS 22.179** | Mission Critical Push To Talk (MCPTT)（MCPTT业务需求） | Stage 1 | Rel-20 | v20.0.0 | MCPTT业务需求；Rel-21 v21.0.0 已出现，仅跟踪 |
| **TS 22.281** | Mission Critical Video over LTE（关键视频业务需求） | Stage 1 | Rel-19 | v19.0.0 | 关键视频业务需求 |
| **TS 22.282** | Mission Critical Data over LTE（关键数据业务需求） | Stage 1 | Rel-19 | v19.0.0 | 关键数据业务需求 |
| **TS 22.289** | Mobile Communication System for Railways（铁路移动通信系统） | Stage 1 | Rel-19 | v19.0.1 | 铁路通信 Stage 1 需求（FRMCS），干线与城市轨道交通在 5G 系统上的业务能力；MBS 承载内容归 TS 23.289 |
| **TR 22.819** | Study on Maritime Communication Services over 3GPP system（海事通信服务研究） | Stage 1 | Rel-16 | v16.2.0 | 海事通信服务可行性研究 FS MARCOM（2018-12-21发布，已结项，无后续更新；标题于2026-10-28订正，旧标题“与非3GPP系统互通研究”为误） |
| **TS 23.280** | Common functional architecture to support mission critical services（MCX通用功能架构） | Stage 2 | Rel-20 | v20.5.1 | MCX通用功能架构 |
| **TS 23.379** | Functional architecture and information flows to support mission critical push to talk (MCPTT)（MCPTT功能架构与信息流） | Stage 2 | Rel-20 | v20.4.0 | MCPTT功能架构与信息流 |
| **TS 23.281** | Functional architecture and information flows to support mission critical video（关键视频功能架构与信息流） | Stage 2 | Rel-20 | v20.5.1 | 关键视频功能架构与信息流 |
| **TS 23.282** | Functional architecture and information flows to support mission critical data（关键数据功能架构与信息流） | Stage 2 | Rel-20 | v20.3.1 | 关键数据功能架构与信息流；2026-10-28 同步（10-23 检查漏了 Rel-20 版） |
| **TS 23.283** | Mission Critical Communication Interworking with Land Mobile Radio Systems（与LMR互通的架构） | Stage 2 | Rel-20 | v20.1.0 | 与LMR互通的架构；2026-10-28 同步（10-23 检查漏了 Rel-20 版） |
| **TS 23.289** | Mission Critical Services over the 5G System (5GS)（MCX over 5GS架构） | Stage 2 | Rel-20 | v20.3.0 | MCX over 5GS，5G-R/FRMCS场景的关键架构；2026-10-28 同步（10-23 检查漏了 Rel-20 版） |
| **TR 23.790** | Study on application architecture for the Future Railway Mobile Communication System (FRMCS); Stage 2（未来铁路移动通信系统应用架构研究） | Stage 2 | Rel-15 | v15.0.0 | 未来铁路移动通信系统应用架构研究（2018-01-06发布，无后续更新，为最终版；2026-10-23待核关闭；标题于2026-10-28补全 application architecture） |
| **TS 24.379** | Mission Critical Push To Talk (MCPTT) call control; Protocol specification（MCPTT呼叫控制协议） | Stage 3 | Rel-20 | v20.1.0 | MCPTT呼叫控制协议 |
| **TS 24.380** | Mission Critical Push To Talk (MCPTT) media plane control; Protocol specification（MCPTT媒体面控制协议） | Stage 3 | Rel-19 | v19.1.0 | MCPTT媒体面控制协议 |
| **TS 24.481** | Mission Critical Services (MCS) group management; Protocol specification（组管理协议） | Stage 3 | Rel-19 | v19.1.0 | 组管理协议 |
| **TS 24.482** | Mission Critical Services (MCS) identity management; Protocol specification（身份管理协议） | Stage 3 | Rel-19 | v19.1.0 | 身份管理协议 |
| **TS 24.483** | Mission Critical Services (MCS) Management Object (MO); Protocol specification（管理对象协议） | Stage 3 | Rel-20 | v20.1.0 | 管理对象协议 |
| **TS 24.484** | Mission Critical Services (MCS) configuration management; Protocol specification（配置管理协议） | Stage 3 | Rel-20 | v20.1.0 | 配置管理协议 |
| **TS 24.281** | Mission Critical Video (MCVideo) signalling control; Protocol specification（MCVideo信令控制协议） | Stage 3 | Rel-20 | v20.1.0 | MCVideo信令控制协议 |
| **TS 24.581** | Mission Critical Video (MCVideo) media plane control; Protocol specification（MCVideo媒体面控制协议） | Stage 3 | Rel-19 | v19.2.0 | MCVideo媒体面控制协议 |
| **TS 24.282** | Mission Critical Data (MCData) signalling control; Protocol specification（MCData信令控制协议） | Stage 3 | Rel-20 | v20.1.0 | MCData信令控制协议 |
| **TS 24.582** | Mission Critical Data (MCData) media plane control; Protocol specification（MCData媒体面控制协议） | Stage 3 | Rel-19 | v19.0.0 | MCData媒体面控制协议 |
| **TR 24.980** | Minimum requirements for support of Mission Critical Push To Talk (MCPTT) over the Gm reference point（Gm参考点上支持MCPTT的最低要求） | Stage 3 | Rel-16 | v16.0.0 | Gm 参考点 MCPTT 最低要求 profile（唯一版本，2026-10-23确认为最终版；标题于2026-10-28订正，旧标题“MCX使能器与增强研究”为误） |
| **TS 33.180** | Security of the Mission Critical (MC) service（关键业务安全） | 安全 | Rel-20 | v20.1.0 | 关键业务安全 |

## 二、中国 CCSA/行标 MCX与5G-R 规范清单

| 标准号 | 名称 | 类别 | 状态 | 备注 |
| :--- | :--- | :--- | :--- | :--- |
| **YD/T 2689-2014** | 《基于LTE技术的宽带集群通信(B-TrunC)系统总体技术要求(第一阶段)》 | 通信行业标准 | 现行 | 归口CCSA；B-TrunC宽带集群总体技术要求 |
| **T/VSTR 031—2025** | 《公网铁路应用总体技术要求》 | 团体标准 | 2025-12-25发布 | 规范性引用TS 23.280/23.379/33.180（中国团标直接引用3GPP MCX的实证） |
| **TJ/DW 239-2021** | 《铁路5G专网业务和功能需求暂行规范》 | 铁路行业暂行规范 | 现行（暂行） | 5G-R专网业务与功能需求 |
| **TJ/DW 246-2022** | 《铁路5G专用移动通信（5G-R）系统总体技术要求（暂行）》 | 铁路行业暂行规范 | 现行（暂行） | 5G-R系统总体技术要求 |
| **Q/CR 883-2022** | （国铁集团企业标准） | 企业标准 | 现行 | 铁路5G相关企业标准 |
| **YJ/T 42.1—2026** | 《应急指挥无线宽带自组网系统技术规范 第1部分：总体要求》 | 应急行业标准 | 2026-05-14发布、2026-08-01实施 | 应急指挥自组网系列第1部分；42.2—42.4已发布，第5部分（测试方法）拟制 |
| **B-TrunC联盟标准具体编号** | 待核 | 联盟标准 | 待核 | 具体编号待核实 |
| **应急部2026年第6号公告同批其余6项名单** | 待核（非YJ/T 42系列） | 应急行业标准 | 待核 | 同批其余6项（非YJ/T 42系列）名单待核实 |

## 三、防错备注

> **警告：**
> **TS 24.280** 和 **TS 24.289** 不存在——曾误传为 MCX 协议规范，经核对 3GPP 官方编号体系中并无这两条，本清单不收录。严禁在后续文档中误引。

## 四、待核事项汇总

1. ~~**TR 22.819** 的公开版本号~~ → 已决：Rel-16 v16.2.0（2026-10-23 纠正基线记录错误）
2. ~~**TR 23.790** 的公开版本号~~ → 已决：Rel-15 v15.0.0 为最终版，无更新（2026-10-23 待核关闭）
3. **B-TrunC联盟标准** 具体编号（仍待核）
4. **应急部2026年第6号公告** 同批其余6项（非YJ/T 42系列）名单（仍待核）
5. ~~Rel-20 口径升级待决策~~ → 已决（2026-10-23 用户拍板）：基线口径升至 Rel-20，10 条已发布 Rel-20 的规范采用 Rel-20 版本（见上表）；**TS 22.280** Rel-21 v21.0.0（2026-10-02）仅跟踪、不纳入基线

---

!!! note 版本说明
    版本号以 3GPP 官网公布为准，本清单定期跟踪更新；"待核"表示暂无公开可查的权威版本，持续核查中。

### 更新日志
- **v1.3（2026-10-28）**：补同步 4 条漏检的 Rel-20 升级——22.179→v20.0.0、23.282→v20.3.1、23.283→v20.1.0、23.289→v20.3.0（10-23 检查漏检，Stage 2 批 ELI5 取数时发现）；Rel-20 口径由 10 条扩至 14 条；其余 Rel-19 规格经全量复核无 Rel-20 版（22.289、24.581、24.582）。
- **v1.2（2026-10-23）**：基线口径升至 Rel-20（用户拍板）——10 条采用 Rel-20：22.280→v20.2.0、23.280→v20.5.1、23.281→v20.5.1、23.379→v20.4.0、24.379/24.281/24.282/24.483/24.484/33.180→v20.1.0；其余保留 Rel-19 最新；TS 22.280 Rel-21 v21.0.0 仅跟踪。本版含 v1.1 全部内容，一并发布上线。
- **v1.1（2026-10-23，未单独发布）**：首次定期检查更新——Rel-19 6 条升级（23.379→v19.11.0、24.379→v19.8.0、24.281→v19.7.0、24.282→v19.8.0、24.484→v19.6.0、33.180→v19.5.0）+ 23.280 编辑性 v19.10.1；TR 22.819 纠正为 Rel-16 v16.2.0、TR 23.790 确认为 Rel-15 v15.0.0（最终版）。
- **v1.0（2026-10-17）**：首版，基于 MCX 基线 v0.2（2026-10-16）；3GPP MCX 25条（23条版本已核对）+中国8条；标出2项防错、待核项见正文。
