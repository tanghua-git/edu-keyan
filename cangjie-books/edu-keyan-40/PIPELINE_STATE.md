# PIPELINE_STATE — edu-keyan-40

> 断点续跑用。每完成一个阶段更新本文件。

## 基本信息
- **书**: 《怎么做课题研究——给教师的40个教育科研建议》 费岭峰 著，华东师范大学出版社
- **slug**: edu-keyan-40
- **源文本**: `G:\wokbuddy案例\给教师的40个教育科研建议\给教师的40个教育科研建议.md` + `markdown/` 12 分章
- **开始时间**: 2026-09-18

## 用户决策（已确认）
- 输出模式: **pack**（1 路由入口 + 5 阶段技能，用户指定结构，晋级门按此映射）
- 安装位置: **用户级** `~/.workbuddy/skills/`
- 技能形态: **方法论 + 模板库**（references 含句式库/框架/清单/范文）
- 三个示例: 拆分归入 skill 2（方案示例）/ skill 4（文献综述示例）/ skill 5（研究报告示例）

## 技能树（目标产物）
| slug | 对应章节 | 状态 |
|---|---|---|
| edu-keyan | 全书路由入口 | 未开始 |
| edu-keyan-xuanti | 第一章 问题1-8（选题+命名） | 未开始 |
| edu-keyan-fangan | 第二章 问题9-16 + 方案示例 | 未开始 |
| edu-keyan-shishi | 第三章 问题17-24 | 未开始 |
| edu-keyan-fangfa | 第四章 问题25-32 + 文献综述示例 | 未开始 |
| edu-keyan-chengguo | 第五章 问题33-40 + 研究报告示例 | 未开始 |

## 优化决策（2026-09-18 用户确认三条批判后加入）
1. **当代适配层**：每个技能 references 固定含 `00-当代适配.md`，写入元知识补丁（2026 政策锚点：《"人工智能+教育"行动计划》《教育强国建设规划纲要(2024—2035)》、2022 版新课标；AI 辅助科研的工作流与学术诚信红线）。
2. **去地域化**：案例蒸馏为模式卡并标注来源标签；制度话语中性化（"以本地最新文件为准"）；学段学科中立。
3. **Boundary 三红线**（每技能 B 段必写）：① 作者经验是建议非定律；② 热点判断须以当下重新扫描；③ 申报格式以本地最新文件为准。
4. **评测时代陷阱负例**：如"现在有什么选题热点"不得照搬书中微课/电子书包案例，应先引导政策扫描。

## 阶段进度
| 阶段 | 状态 | 产出 | 备注 |
|---|---|---|---|
| 0 整书理解 | ✅ 已完成，待用户确认 | BOOK_OVERVIEW.md | 2026-09-18 |
| 1 并行提取 | ✅ 已完成 | candidates/ 5 文件，共 298 条 | 框架57/原则112/案例54/反例40/术语35；术语提取器首轮上下文超限，改检索式重跑成功 |
| 1.5 三重验证 | ✅ 已完成，待用户轻确认 | verified.md + 3 分区文件 + rejected/ | 298→去重73→通过45（含路由4）；router-flavor降级5；淘汰单元全部保留为references素材 |
| 1.6 晋级门 | ✅ 已完成 | 48 单元按 target_skill 映射到 6 技能（含捞回3条：实验五组成→fangfa、小题大做+微型课题三要求→xuanti） | 用户指定结构即去向，无需自动晋级评审 |
| 2+3 技能编写 | 🔵 进行中 | 直接编写 6 个技能目录（偏离仓颉 compile：用户要求"结合仓颉但不完全依赖"，成品手工精编为方法论+模板库形态） | 5 个作者代理并行 + 路由技能主代理自写 |
| 4 压力测试 | ✅ 已完成 | test-results.md | 6 盲测代理，58/59≈98%，全部技能过线无需回炉 |
| 5 编译交付 | ✅ 已完成 | 6 技能已装用户级 + DIGEST.md（3604字） | 直接编写式交付（偏离仓颉 compile，用户指定） |

## 最终交付清单（2026-09-18 完成）
- `~/.workbuddy/skills/edu-keyan/`（路由：SKILL.md + 00-当代适配 + 01-全书术语表35条 + evals 8条）
- `~/.workbuddy/skills/edu-keyan-xuanti/`（8单元，references 6件 + evals 10条）
- `~/.workbuddy/skills/edu-keyan-fangan/`（11单元，references 10件 + evals 10条）
- `~/.workbuddy/skills/edu-keyan-shishi/`（6单元+淘汰素材，references 7件 + evals 10条）
- `~/.workbuddy/skills/edu-keyan-fangfa/`（8单元含捞回f44，references 10件 + evals 10条）
- `~/.workbuddy/skills/edu-keyan-chengguo/`（11单元，references 9件 + evals 10条）
- 全书 DIGEST.md 3604 字
- 审计轨迹：candidates/(298条) + verified*.md(48通过) + rejected/ + test-results.md

## 断点恢复指引
当前停在：阶段 0 完成，等待用户对 BOOK_OVERVIEW.md 的确认。确认后进入阶段 1（5 个 extractor 并行提取，按 markdown/ 分章喂料）。
