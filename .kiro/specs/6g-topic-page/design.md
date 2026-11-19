# 设计文档：6G 追踪专题页

## 1. 文件清单 (File Manifest)

| 路径 | 状态 | 说明 |
| :--- | :--- | :--- |
| `docs/6g/index.md` | 新建 | 6G 追踪总览页 |
| `docs/6g/core-routes.md` | 新建 | 三条路线之争详解 |
| `docs/6g/tracking.md` | 新建 | 跟踪动态与待核清单 |
| `mkdocs.yml` | 修改 | 更新 `nav` 配置 |
| `.kiro/specs/6g-topic-page/source-csdn-first-article.md` | 参考（已提供） | CSDN 首篇定稿原文，core-routes.md 的改编底本 |

## 2. 导航结构设计 (Navigation Design)

在 `mkdocs.yml` 的 `nav` 列表中，定位到 `MCX` 相关项之后，`应急政策` 之前，插入以下结构：

```yaml
- 6G 追踪:
  - 总览: 6g/index.md
  - 三条路线之争: 6g/core-routes.md
  - 跟踪动态: 6g/tracking.md
```

## 3. 页面结构设计 (Page Structure Design)

### 3.1 6g/index.md (总览)
*   **Header**: 
    *   Title: `# 6G 核心网追踪：总览`
    *   Meta Block (Quote): `> 版本 v1.0｜更新 2026-11-19｜数据基线：6G 核心网研究报告 2026-11-12`
*   **Section 1: 阅读路径**
    *   Ordered List with links to `./core-routes.md` and `./tracking.md`.
*   **Section 2: 6G 核心网是什么**
    *   Subsection: 方向一 (独立 AI 域)
    *   Subsection: 方向二 (AI 进入网络功能)
    *   Subsection: 方向三 (智能体直接管理连接)
*   **Section 3: 演进脉络与决策时间线**
    *   Markdown Table: Columns [阶段/事件, 时间/状态, 备注]
*   **Section 4: 本系列**
    *   Markdown Table: Columns [篇目, 一句话导读, 状态]
*   **Section 5: 关键词**
    *   Inline Code list: `NAS`, `NF`, `AMF`, `SMF`, `PCF`, `SRF`, `IMS`
*   **Section 6: 更新日志**
    *   List: `2026-11-19 建页`

### 3.2 6g/core-routes.md (三条路线之争)
*   **Header**: `# 6G 核心网：三条路线之争`
*   **Section 1: 一、三条路线**
    *   Detailed comparison of Route 1, 2, 3.
*   **Section 2: 二、NAS**
    *   Analysis of NAS handling in each route.
    *   *Constraint*: Keep "46 比 7" / "16 比 32" as informal polling context.
*   **Section 3: 三、迁移问题**
    *   Discussion on migration challenges.
*   **Section 4: 四、产业账本**
    *   *Constraint*: Omdia analysis is analytical, not deployment result.
    *   *Constraint*: 2031 mass production for Route 1 is conditional (3 assumptions).
*   **Section 5: 五、互通**
    *   *Constraint*: Voice/Emergency calls are Day 1, favoring 4G/5G IMS reuse.
*   **Section 6: 六、标准进展**
    *   *Critical Constraint*: Must contain literal text `[待填：SA2#178 决策结果]`. Do not invent results.
*   **Section 7: 结语**
    *   Summary without CSDN-specific footer.

### 3.3 6g/tracking.md (跟踪动态)
*   **Header**: `# 6G 核心网：跟踪动态`
*   **Section 1: 三个决策点**
    *   Table: [会议/事件, 时间, 状态]
    *   Row 1: SA2#178, 2026-11-16 至 20, 会议进行中、结果待公布
    *   Row 2: SA#114, 2026-12-08 至 11, 待开
    *   Row 3: Rel-21 Stage-1 冻结, 2027-03, 待定
*   **Section 2: 待核清单 (I1-I10)**
    *   Table: [编号, 待核项]
    *   Rows I1 to I10 as specified in requirements.
*   **Section 3: 更新节奏说明**
    *   Text explaining "Pre-meeting preview -> Post-meeting conclusion" workflow and monthly 8/23 tracking.
*   **Section 4: 更新日志**
    *   List of updates.

## 4. 链接规则 (Linking Rules)

*   **Internal Links**: All links between the three new pages must use relative paths.
    *   In `index.md`: `[三条路线之争](./core-routes.md)`, `[跟踪动态](./tracking.md)`
    *   In `core-routes.md`: `[返回总览](./index.md)`, `[跟踪动态](./tracking.md)`
    *   In `tracking.md`: `[返回总览](./index.md)`, `[三条路线之争](./core-routes.md)`
*   **External Links**: Use full URLs if referencing external sources (though minimal in this scope, ensure they are absolute or properly configured in Material theme if applicable, but primarily focus on internal relative links for build stability).

## 5. 技术约束 (Technical Constraints)

*   **MkDocs Material Theme**: Ensure front matter is present if required by the theme for navigation sorting or page attributes, though standard Markdown headers are sufficient for basic structure.
*   **Language**: Strictly Chinese content. English only for acronyms (NAS, NF, AMF, SMF, PCF, SRF, IMS) and specific proper nouns if unavoidable, but preference is for Chinese terms where defined.
*   **Build Integrity**: No broken links. `mkdocs build` must pass without warnings. This implies checking for misspelled relative paths.
