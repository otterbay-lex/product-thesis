# Product Thesis · 产品立论

> 从问题结构出发，借用别的行业的机制，而不是复制它们的产品。
> Start from the problem structure; borrow mechanisms across domains, not products.

---

## About · 关于

### 先为一个产品立论

Product Thesis 是一个可安装给 AI Agent 使用的产品立论研究 Skill。它不替你批量产出创业点子，也不急着把一个念头扩写成产品功能。你先把背景完整讲出来，它再整理事实与假设、研究案例、核查迁移，再和你一起决定这个方向是否值得继续。

许多想法不是不新，而是太早变成了方案。人一旦开始讨论页面、模型或功能，原本的问题常常被盖住。Product Thesis 会先把方案放在一旁，要求把行业术语一点点拿掉，直到能用不依赖原行业的语言说出那种反复出现的困难。

然后，它才会向别的行业寻找线索。不是为了找一个“很像”的产品，而是为了看：另一个地方的人是否也被同一种结构困住；他们用什么机制让系统发生变化；这个机制挪回来之后，哪些部分仍然成立，哪些部分会失效。每个来源案例都应附可核查链接，不拿模型记忆里的公司故事充当研究。

有些推演最后会得到 `PARK`，甚至 `NO`。这不是流程失败。能在投入数周开发前发现一个想法站不住，本来就是这件事最有价值的结果之一。

### Make the case before making the product

Product Thesis is an installable product-research skill for AI agents. It does not mass-produce startup ideas or rush a first thought into a feature set. You first describe the context in full; it then separates facts from assumptions, researches source cases, checks the transfer, and helps decide whether the direction should continue.

Many ideas are not unoriginal; they simply become solutions too soon. Once the conversation turns to screens, models, or features, the original problem can disappear beneath them. Product Thesis parks the solution and removes industry language layer by layer, until the recurring difficulty can be described without relying on the source domain.

Only then does it look elsewhere for clues. The question is not whether another product looks similar. It is whether another field was constrained by the same structure, what mechanism changed that system, and which parts of that mechanism survive—or fail—when moved back. Every source case should carry a verifiable link; remembered company stories are not research.

Some explorations should end in `PARK`, or even `NO`. That is not a failure of the process. Discovering that an idea cannot carry its own weight before weeks of development is one of the reasons to use it.

> “好的类比不是让人觉得聪明，而是让人更早发现自己错在哪里。”
>
> “A good analogy does not make us sound clever; it helps us find out sooner where we may be wrong.”

*Problem before solution · Structure before analogy · Mechanism before feature*

---

## Features · 功能

### 1. Research intake｜先把背景讲完整

首次不需要逐关回答。你只要尽量完整地说出：具体问题、受影响的人、他们现在怎样处理、你的方案直觉、替代办法、见过的案例或数据，以及你的疑虑；不知道的地方可以直接写“不确定”。Skill 会先整理，而不是立刻追问。

You do not need to answer a gate-by-gate questionnaire. Describe the problem, affected people, current behaviour, solution intuition, alternatives, examples or data, and doubts in one pass; say “uncertain” where needed. The skill organises first rather than immediately interrogating you.

### 2. Abstraction｜把行业名字慢慢拿掉

同一个问题会被带过三层：正在完成的实际任务、让任务反复失败的系统、以及不依赖原行业的底层矛盾。到这一步，才会形成一组真正有因果作用的结构标签，例如信息不对称、协调成本、信任缺口或延迟回报。

The problem moves through three levels: the practical job, the system that makes the job fail repeatedly, and the underlying tension that does not depend on the original industry. Only then does it receive causal structure labels such as information asymmetry, coordination cost, trust deficit, or delayed reward.

### 3. Source-grounded Transfer Map｜有来源的跨行业迁移

这是这个 Skill 最在意的部分。Airbnb、Duolingo、GitHub 等在这里不是模板，而是被拆开的机制样本。Skill 会主动研究近、中、远三个层次的案例；每个案例附上可核查来源，并写成：

```text
目标问题的结构
→ 来源行业里的同构结构
→ 来源机制
→ 可以尝试的最小迁移
→ 会让迁移失效的边界
```

这会把“另一个产品也很像”变成更难、也更有用的问题：它们究竟在哪些变量上相同？来源行业的机制为什么在那边有用？放到这里以后，哪一个条件先不成立？

Airbnb, Duolingo, GitHub, and similar cases are not templates here. They are mechanism samples. The skill researches Near, Medium, and Far cases, cites each one, and turns each into a Transfer Map: target structure, equivalent source structure, source mechanism, smallest plausible adaptation, and the boundary where the transfer breaks.

### 4. Break the Analogy｜给类比找反例

每个候选迁移都必须回答：什么能映射，什么不能映射，哪些变量不同，为什么可能失败，以及什么证据可以尽快推翻它。Far Transfer 的表面差异越大，越不能因为它新鲜就默认它成立。

Every candidate transfer must say what maps, what does not, which variables differ, why it may fail, and what evidence could disprove it quickly. The more distant the surface resemblance, the less novelty alone should count as evidence.

### 5. Thesis Workspace｜最后留下可继续修正的立论工作台

最后生成的是一份 Product Thesis Workspace，而不是只给出一句结论。它会保留暂定立论、证据账本、尚未解决的问题和下一步研究路线。`PARK` 会明确指出缺什么证据，以及接下来是验证问题、深挖机制、比较机制还是做最低成本实验。`YES` 只代表值得做一个小实验，不代表应该立刻开发完整产品。

The final output is a Product Thesis Workspace, not a one-line verdict. It preserves a provisional thesis, evidence ledger, unresolved questions, and next research routes. A `PARK` names the missing evidence and whether to validate the problem, deepen a mechanism, compare mechanisms, or run the cheapest experiment. A `YES` only earns a small experiment, not a full build.

## Installation · 安装

### Codex

将整个 `product-thesis/` 文件夹复制到 Codex 的 skills 目录（通常为 `~/.codex/skills/`），重新打开或刷新 Codex 后即可使用。

Copy the entire `product-thesis/` folder into Codex’s skills directory (usually `~/.codex/skills/`), then reopen or refresh Codex.

### 其他 Agent

将本仓库中的 [`SKILL.md`](SKILL.md)、`references/` 和 `assets/` 一并提供给支持 Markdown Skill 或 Prompt 包的 Agent。只复制 `SKILL.md` 会少掉结构库、机制样本、评分规则和最终卡片模板。

For other agents, provide [`SKILL.md`](SKILL.md), `references/`, and `assets/` together to an agent that supports Markdown skills or prompt packages. Copying `SKILL.md` alone omits the structure library, mechanism examples, scoring rubric, and final-card template.

## Usage · 使用方式

默认使用 Research Mode。第一次只需要用自然语言把背景讲完整；Skill 会先整理“用户事实 / 用户判断 / 外部证据 / 待验证假设”，再主动研究有来源的近、中、远行业案例，最后给出可以继续修正的立论工作台。

Research Mode is the default. In one natural-language intake, you provide the context; the skill first creates an evidence ledger, then researches sourced Near, Medium, and Far cases, and returns a revisable thesis workspace.

如果你想刻意训练自己的抽象能力，可以明确说 Training Mode；它会在三处邀请你先作判断，但仍会完成研究。需要快速桌面研究时，明确说 Fast Mode。

Ask for Training Mode when you want to practise abstraction; it pauses for three of your own judgments but still completes the research. Ask for Fast Mode when you need a rapid desk-research pass.

```text
使用 product-thesis 的 Training Mode，为一个产品立论：
我想做一个面向独立律师的 AI 案件材料整理工具。
先不要讨论功能，带我完成前置分析。

Use product-thesis in Training Mode to develop a product thesis:
I want to build an AI case-material organisation tool for independent lawyers.
Do not discuss features yet. Guide me through the preflight analysis first.
```

```text
使用 product-thesis 的 Fast Mode，为这个方向形成 Product Thesis：
我想做一个帮助上班族减少每天衣橱决策疲劳的服务。

Use product-thesis in Fast Mode to form a Product Thesis:
I am considering a service that helps office workers spend less energy choosing what to wear each day.
```

## Principles & Boundaries · 原则与边界

- 方案可以先出现，但在问题结构分析完成前，不讨论产品功能、技术架构或 UI。
- 迁移的是机制，不是品牌、功能或界面。
- 没有访谈、行为数据或实际观察时，结论应当写成假设，而不是事实。
- `NO` 与 `PARK` 都是有价值的结果；不要为了完成流程强行生成产品。
- Training Mode 不替用户做判断，它训练的是结构识别、跨行业迁移与反证能力。

- A solution may appear early, but features, architecture, and UI wait until the problem structure is understood.
- Transfer mechanisms, not brands, features, or interfaces.
- Without interviews, behavioural evidence, or direct observation, conclusions remain hypotheses rather than facts.
- `NO` and `PARK` are useful results; do not invent a product just to finish the workflow.
- Training Mode does not make decisions for the user. It is intended to develop structural recognition, cross-domain transfer, and falsification.

## v0.1.0 Release Notes · 发布说明

第一个公开版本包含七个立论 Gate、Training Mode 与 Fast Mode、可扩展结构标签库、五个机制样本、Transfer Map、轻量评分规则、Product Thesis Card 以及法律科技、生活方式、AI 知识产品三组回归案例。

The first public version includes seven thesis-building gates, Training Mode and Fast Mode, an expandable structure library, five mechanism samples, Transfer Maps, a lightweight scoring rubric, the Product Thesis Card, and three regression cases for legal tech, lifestyle, and AI knowledge products.

## License · 许可证

本项目采用 [Apache License 2.0](LICENSE)，包含专利授权与专利诉讼终止条款。使用者仍需自行确认其输入材料、案例、商标和其他第三方内容的授权。

This project is licensed under the [Apache License 2.0](LICENSE), including its patent grant and patent-termination provision. Users remain responsible for rights in their own inputs, examples, trademarks, and other third-party content.
