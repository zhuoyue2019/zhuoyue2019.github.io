# 需求规格说明书：6G 追踪专题页

## 1. 范围与目标
在 MkDocs Material 知识库中新增“6G 追踪”专题，包含三个页面：总览、三条路线之争、跟踪动态。导航栏需更新以包含新栏目。

## 2. 功能性需求 (Functional Requirements)

### 2.1 导航结构 (Navigation)
*   **REQ-NAV-01**: WHEN 用户访问站点导航，THEN 系统 SHALL 在“MCX”栏目之后、“应急政策”栏目之前显示顶级栏目“6G 追踪”。
*   **REQ-NAV-02**: WHEN 用户点击“6G 追踪”栏目，THEN 系统 SHALL 展示三个子页面链接：
    1.  总览 (指向 `6g/index.md`)
    2.  三条路线之争 (指向 `6g/core-routes.md`)
    3.  跟踪动态 (指向 `6g/tracking.md`)
*   **REQ-NAV-03**: IF 现有导航中的其他栏目（首页、3GPP UAS、跟踪平台、MCX、应急政策、免费 API、关于）存在，THEN 系统 SHALL 保持其顺序和内容不变。

### 2.2 页面内容：总览 (6g/index.md)
*   **REQ-INDEX-01**: WHEN 渲染 `6g/index.md`，THEN 页面顶部 SHALL 包含一个引用块，内容为：“版本 v1.0｜更新 2026-11-19｜数据基线：6G 核心网研究报告 2026-11-12”。
*   **REQ-INDEX-02**: WHEN 渲染 `6g/index.md`，THEN 页面 SHALL 包含“阅读路径”章节，以带链接的编号列表形式呈现。
*   **REQ-INDEX-03**: WHEN 渲染 `6g/index.md`，THEN 页面 SHALL 包含“6G 核心网是什么”章节，准确描述三条路线：
    *   方向一：独立 AI 域（AI 在分组交换网之外，传统 NAS 仍由 AMF 路由）。
    *   方向二：AI 进入网络功能（AI 纳入 NF 体系，可设专用 NF 或嵌入 AMF/SMF/PCF，NAS 组织方式有柔性）。
    *   方向三：智能体直接管理连接（AI Agent 参与 NF 协调和连接管理，涉及独立于 AMF 的 SRF）。
*   **REQ-INDEX-04**: WHEN 渲染 `6g/index.md`，THEN 页面 SHALL 包含“演进脉络/决策时间线”表格，包含以下精确行：
    *   Rel-20：5G-A 与 6G 双轨研究
    *   Rel-21：首个规范性 6G 版本
    *   FS_6G_ARC 研究计划：2027-03-03 结束
    *   SA2#178：2026-11-16 至 2026-11-20，卡尔加里，架构总体决策最迟在此作出
    *   SA#114：2026-12-08 至 2026-12-11
    *   Rel-21 Stage-1 冻结：2027-03
    *   Stage-2 80% 检查点：2028-03
    *   Stage-2 冻结：2028-06
    *   Stage-3 功能冻结：2028-12
    *   ASN.1 和 OpenAPI 冻结：2029-03
*   **REQ-INDEX-05**: WHEN 渲染 `6g/index.md`，THEN 页面 SHALL 包含“本系列”表格，列出本篇及后续篇目、一句话导读、状态。
*   **REQ-INDEX-06**: WHEN 渲染 `6g/index.md`，THEN 页面 SHALL 包含“关键词”章节，术语使用行内代码格式。
*   **REQ-INDEX-07**: WHEN 渲染 `6g/index.md`，THEN 页面 SHALL 包含“更新日志”，首条为“2026-11-19 建页”。

### 2.3 页面内容：三条路线之争 (6g/core-routes.md)
*   **REQ-CORE-01**: WHEN 渲染 `6g/core-routes.md`，THEN 页面 SHALL 包含六个主要章节及结语：一、三条路线；二、NAS；三、迁移问题；四、产业账本；五、互通；六、标准进展；结语。
*   **REQ-CORE-02**: IF 源内容中包含 CSDN 专用结尾文字（如“zhuoyue2019.github.io 直达链接暂不公开，私信获取”），THEN 系统 SHALL 移除这些文字。
*   **REQ-CORE-03**: WHEN 渲染 `6g/core-routes.md`，THEN 页面 SHALL 保留以下谨慎限定表述：
    *   “46 比 7”和“16 比 32”为非正式意向征询，不是正式表决。
    *   Omdia 的判断是分析判断，不是部署结果。
    *   方向一 2031 年量产是条件性推论，须三个假设同时成立。
    *   语音和紧急呼叫是 6G Day 1 需求，倾向复用 4G/5G IMS。
*   **REQ-CORE-04**: WHEN 渲染 `6g/core-routes.md` 的第六节“标准进展”，THEN 页面 SHALL 保留占位符 `[待填：SA2#178 决策结果]`，且 SHALL NOT 编造任何具体的会议决策结果。

### 2.4 页面内容：跟踪动态 (6g/tracking.md)
*   **REQ-TRACK-01**: WHEN 渲染 `6g/tracking.md`，THEN 页面 SHALL 包含“三个决策点”表格：
    *   SA2#178 (2026-11-16 至 20)：状态为“会议进行中、结果待公布”。
    *   SA#114 (2026-12-08 至 11)：状态为“待开”。
    *   Rel-21 Stage-1 冻结 (2027-03)：状态为“待定”。
*   **REQ-TRACK-02**: WHEN 渲染 `6g/tracking.md`，THEN 页面 SHALL 包含“待核清单”表格，包含 I1 至 I10 项，内容严格对应：
    *   I1: 基带迭代周期 18—24 个月原始出处
    *   I2: 爱立信 Ekholm 中国市场份额约 10% 估计年份
    *   I3: SA2#178 实际决策结果
    *   I4: FS_6G_ARC 研究结束日期与架构总体决策节点关系
    *   I5: 提案文号重复及编号形式异常
    *   I6: SA2#173 的 R20 架构全景报告及 AIMF
    *   I7: 中国在 3GPP R19 提案中占比 38%
    *   I8: IRJET 的 TCO 测算方法
    *   I9: 17 家联署运营商完整名单
    *   I10: 方向一 UE AI 域客户端量产最快 2031 年前后的条件性推论
*   **REQ-TRACK-03**: WHEN 渲染 `6g/tracking.md`，THEN 页面 SHALL 包含“更新节奏说明”，指出按“会前预告→会后定论”更新，并接每月 8/23 日跟踪。
*   **REQ-TRACK-04**: WHEN 渲染 `6g/tracking.md`，THEN 页面 SHALL 包含“更新日志”。

## 3. 非功能性需求 (Non-Functional Requirements)

### 3.1 数据准确性与合规
*   **NFR-ACC-01**: IF 内容涉及 SA2#178 决策结果，THEN 系统 SHALL 使用占位符，SHALL NOT 编造任何未提供的具体结果。
*   **NFR-ACC-02**: WHEN 渲染所有新页面，THEN 所有数字、日期、人名、会议名 SHALL 严格以本需求文档提供的数据为准，SHALL NOT 自行补充或修改。
*   **NFR-LANG-01**: WHEN 渲染所有新页面，THEN 内容 SHALL 为中文，SHALL NOT 包含英文段落（术语缩写 NAS/NF/AMF/SMF/PCF/SRF/IMS 除外）。

### 3.2 构建与链接
*   **NFR-BUILD-01**: WHEN 执行 `mkdocs build`，THEN 构建过程 SHALL 零警告通过。
*   **NFR-LINK-01**: WHEN 在新页面之间进行链接，THEN 系统 SHALL 使用相对路径。
*   **NFR-SCOPE-01**: IF 修改涉及现有页面或 nav 其他栏目，THEN 系统 SHALL 报错或拒绝修改，本次任务 SHALL NOT 改动现有页面和 nav 其他栏目。

## 4. 验收标准 (Acceptance Criteria - EARS Style)

1.  **WHEN** 用户打开站点导航，**THEN** "6G 追踪" 应出现在 "MCX" 之后且 "应急政策" 之前。
2.  **WHEN** 用户点击 "6G 追踪" 下的 "总览"，**THEN** 页面应显示引用块 "版本 v1.0｜更新 2026-11-19｜数据基线：6G 核心网研究报告 2026-11-12"。
3.  **WHEN** 用户查看 "总览" 页面的决策时间线，**THEN** SA2#178 的地点应显示为 "卡尔加里"，时间应为 "2026-11-16 至 20"。
4.  **WHEN** 用户查看 "三条路线之争" 页面的第六节，**THEN** 应看到 `[待填：SA2#178 决策结果]`，且周围不应有关于该会议具体决议的非占位文本。
5.  **WHEN** 用户查看 "跟踪动态" 页面，**THEN** 待核清单 I3 应明确标注为 "SA2#178 实际决策结果"。
6.  **IF** 构建命令 `mkdocs build` 执行完毕，**THEN** 退出码应为 0 且无 warning 输出。
7.  **WHEN** 检查 `docs/6g/` 下的文件链接，**THEN** 所有内部链接应指向 `./core-routes.md`, `./tracking.md`, `./index.md` 等相对路径。
8.  **IF** 对比修改前后的 `mkdocs.yml`，**THEN** 仅 `nav` 部分增加了 "6G 追踪" 及其子项，其他键值对未变。
