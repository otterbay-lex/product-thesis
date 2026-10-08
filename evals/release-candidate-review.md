# v0.2.0 candidate review · 发布候选检查

Date: 2026-10-08. Instruction-only package; no scripts or dependencies added.

## What was tested · 测试范围

Used Codex CLI v0.160.0 with its configured default model, gpt-5.6-sol, medium reasoning. Each run read the working copy of SKILL.md and its routed references. Reviewed the actual final responses for readability, mechanism mapping, failure boundaries, next actions, and decision restraint. No automated grading score is claimed.

本次输入均为虚构场景。六个实验判断测试把上一轮假设、原定门槛和用户报告的结果放在同一条续轮输入里，不是六次真实用户实验，也没有覆盖长期多轮对话。十二个原有输入场景保留在 evals.json，本轮没有全部重跑。

## Readability results · 可读性结果

| Final case | Result | Main insight and objection | Final response size |
| --- | --- | --- | --- |
| 带猫酒店核验 | PASS with length caveat | 借充电设施的近期使用记录机制，区分永久标签与有时效的观察；低频贡献可能让记录迅速失效。PARK，先验证痛点与实际贡献。 | 1,617 characters, 3 headings |
| AI 公司知识 | PASS after correction | 借医疗质量体系的受控版本机制，先确认当前有效内容；咨询资料可能没有单一最终真相。PARK，记录真实检索事件。 | 1,368 characters, 3 headings |
| Costco → 小企业采购 | PASS | 借买方筛选责任及激励，检验有限选择；软件退出和集成成本不能按零售退货类比。PARK，先做人工采购试验。 | 1,281 characters, 3 headings |

字符数包含 Markdown 和完整链接，不是纯中文正文长度。PASS 表示本次人工检查通过，不代表不同模型或重复运行一定相同。

首次带猫场景只有一句想法，Skill 合理地邀请补充背景；补齐经历后才评估完整研究回答。首次知识回答虽然易读，却主要展示同类 AI 产品，未充分体现跨行业迁移。随后补强 SKILL.md：同类竞品不能代替跨行业研究，正文须解释来源领域、映射变量和关键差异。补充目标背景后重跑得到医疗文档控制案例。规则和输入均有变化，因此不能把改善完全归因于规则调整。

宠物案例选择了中距离迁移，不应包装成高质量 Far Transfer。知识案例的医疗质量管理与咨询工作表面不同，受控有效版本的映射有解释，但迁移有效性仍待目标实验。没有证据说明所有问题都能找到合格的远迁移。

## Experiment decisions · 实验结果判断

| Fixture | Expected / observed | Review |
| --- | --- | --- |
| bounded-build | BUILD / conditional BUILD | 保留用户报告及小样本限制，只放行被测采购流程，先复核记录。 |
| inconclusive-park | PARK / PARK | 6人使用未达8人门槛；没有用喜欢替代行为证据，建议重新招募临近订房的用户。 |
| mechanism-kill | KILL / KILL | 查证时间仅改善3%，错误增加，停止当前机制，保留知识时效教训。 |
| constraint-overrides-demand | KILL / KILL | 付款通过不能覆盖核心资料授权失败，不提出绕过授权。 |
| vanity-signal-park | PARK / PARK | 注册只能支持兴趣，不能证明查证机制，建议人工真实任务对比。 |
| posthoc-window-park | PARK / PARK | 两周活跃不能证明90天留存，不允许事后改原门槛。 |

六项判断与预期一致。该结果只验证这些输入下的行为，不能证明真实商业判断的准确率。

## Source spot checks · 来源抽查

Verified three central source claims against primary material: recent rather than lifetime charging observations in [PlugShare documentation](https://help.plugshare.com/hc/en-us/articles/6327300783507-Station-PlugScores); approved controlled copies and retained obsolete documents in [MDSAP document control](https://www.fda.gov/media/146756/download?attachment=); limited warehouse selection in [Costco's 2025 filing](https://www.sec.gov/Archives/edgar/data/909832/000090983225000101/cost-20250831.htm). These establish source practices, not causal effectiveness in the target contexts. Other links in the generated answers were not exhaustively independently checked in this review.

## Release preparation · 发布准备

- SKILL metadata, 18 fixture definitions, eight routed files and local Markdown links checked.
- Package scan found no secret values, private home paths, contact data or stale TODO/TBD markers in the checked patterns. Fixtures contain no real customer data.
- Apache-2.0 full license and patent grant retained. Added package-level .gitignore for export to the public repository.
- Chinese/English README describes the short answer and optional full workspace; CHANGELOG records the candidate changes and limitations.
- Local installed skill updated with a recoverable backup. Global reminder now includes product study, mechanism translation and pre-coding validation.
- At candidate review, v0.2.0 was Unreleased. Release preparation subsequently dated the changelog 2026-10-08. Publishing exports this package, not the surrounding monorepo; unrelated plan edits are excluded.

## Remaining limitation · 仍需观察

Ready for a public instruction-only candidate, with the evidence limits above. The next useful check is a small number of real users reading the answer and describing, in their own words, the judgment, the strongest objection and what they will do next. Also test longer continuations and repeated runs for cross-domain selection stability. The present checks do not establish that every answer is easy for every user to act on.

可读性已改善，但仍有公式式箭头、短列表和专业词。宠物答案略长；Costco 答案中“正确的产品”措辞偏肯定。后续优先观察这些表达是否影响理解，而不是继续增加模板。
