# Changelog

## [0.2.0] — Unreleased

### Added

- Source-product study：既可以从目标问题出发，也可以从一个值得研究的产品出发；先建立 Product Dossier，再讨论迁移。
- 产品拆解框架：用户与使用时刻、替代方案、价值交付、关键工作流、信任、商业模式、增长与成本承担者。
- 合法迁移边界：只使用公开材料和经授权的信息；明确禁止复制代码、受保护素材、私有数据、商业秘密，以及用于发现非公开实现的逆向工程或技术探测。
- 开发前验证路线：问题访谈、概念访谈、Landing Page、定价实验、Wizard-of-Oz / concierge 实验。
- 两层决策：`YES / PARK / NO` 判断立论是否值得验证；实际实验后才使用 `BUILD / PARK / KILL`。
- 12 个跨领域评测场景，覆盖法律科技、生活方式、知识协作、B2B 采购、照护、定价、合规与市场信任等问题。
- 6 个实验结果判断场景：窄范围通过、证据不足、机制失败、约束失败、虚荣指标与事后改阈值。均为虚构测试输入，不是用户研究成果。
- 默认先给可读的 Product Judgment Brief；完整研究工作台按需展开。

### Changed

- 七个 Gate 继续作为内部研究骨架，对用户呈现为更自然的研究过程。
- Transfer Map 现在必须同时说明公开来源、事实与推断、结构变量、竞争解释、不映射变量和失效边界。
- `YES`、`PARK`、`NO` 不再是对话终点；每种结论都必须说明下一条可执行的研究路线。
- 评分增加 Evidence Quality 与 Validation Readiness；证据或实验设计不足时，不能越级给出 `BUILD`。
- 默认正文只展开一个核心机制，使用自然语言解释反方理由和一个推荐动作；尚无实验时明确暂不进入开发。
- 实验按原定阈值和实际观察期解释；小样本通过只支持被验证的窄工作流，不推断产品市场契合。

### English release summary

- Added public-source product study, lawful mechanism translation, competing explanations, and five pre-coding validation methods.
- The default answer now gives a readable judgment, its strongest objection, and one next action. The full research workspace is available on request.
- Added six fictional experiment-result scenarios alongside twelve intake scenarios. Reported outcomes are judged against the original threshold and observation window; a pass applies only to the tested workflow.
- This remains an instruction-only release candidate. Model-based checks do not replace real user testing.

### Still intentionally absent

- 不包含网页、数据库、抓取器或自动化竞品监控。
- 不以代码实现、私有指标或大规模案例库代替产品判断。

## [0.1.0] — 2026-08-12

### Added

- Research Mode：首次完整输入后，先整理证据账本，再进行产品立论研究。
- 近、中、远三类有来源的跨行业 Transfer Map。
- 机制迁移的压力测试：变量映射、关键差异、失效边界与可证伪证据。
- Product Thesis Workspace：暂定立论、证据、未解问题与下一步研究路线。
- 可选 Training Mode 与 Fast Mode。
- 结构标签库、机制样本、轻量评分规则，以及三组回归检查案例。

### Known limitations

- 当前为 instruction-only 版本；外部案例研究依赖 Agent 的联网与来源核查能力。
- 没有真实用户访谈、行为数据或直接观察时，结论仍应视为待验证假设。
