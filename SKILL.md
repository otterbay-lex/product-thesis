---
name: product-thesis
description: >-
  Research and develop a defensible product thesis before proposing, designing,
  or building a product, AI tool, website, app, service, or feature. Use whenever
  a user brings a product idea, industry pain point, solution intuition, asks
  whether something is worth building, or wants to study a successful existing
  product and translate what makes it work into another user, context, or
  industry. Default to Research Mode: organise the user's context, study lawful
  public evidence, separate product features from mechanisms, research sourced
  near/medium/far transfers, stress-test where each transfer fails, and produce
  an iterative thesis workspace with a concrete validation route before coding.
---

# Product Thesis Research Assistant

This skill helps a user make a product case that can be revised with evidence. It is not a seven-question exercise, a feature generator, or a catalogue of clever analogies.

Its central claim is:

`problem structure → cross-domain mechanism → qualified transfer → testable product thesis`

The seven gates below are an internal research spine. In the default mode, do not make the user experience them one by one.

## Operating rules

- Work **problem before solution**. Park any early product concept as `Candidate Solution`; do not design features, architecture, UI, or an MVP before the thesis has survived transfer stress testing.
- Separate **user-supplied facts**, **user judgments**, **external evidence**, and **inferences**. Do not turn a plausible inference into a fact.
- Remove industry language progressively. A good principle-level abstraction is understandable without knowing the original industry.
- Transfer mechanisms, not brands, features, or interfaces.
- A source case is usable only with a verifiable source and a causal mapping. Do not present remembered company stories as research.
- Every analogy needs a failure boundary and a way to be disproved.
- `YES`, `PARK`, and `NO` are decision states, not conversation endings. Always show the next research route.

## Lawful product study boundary

Read `references/lawful-translation-boundaries.md` whenever the user names an existing product, company, interface, workflow, dataset, or proprietary system as something to learn from, reproduce, translate, or improve.

Product study here means learning from lawfully accessible evidence and forming an independent product judgment. It does not mean reconstructing protected implementation details. Keep a visible boundary between what the evidence shows and what the analysis infers by labelling material claims as:

- **Observed public fact:** directly visible through ordinary lawful use of a publicly available product or public material. State what was observed and where.
- **Publicly sourced claim:** stated by an identifiable public source. Cite the source next to the claim and do not silently upgrade marketing language into verified causation.
- **Inference:** an analytical explanation derived from facts or sources. State the reasoning and the uncertainty; do not present it as inside knowledge.

Use public product pages, public pricing, help centres, published interviews, filings, public reviews, research, and the user's own lawful experience. It is acceptable to describe observable flows, compare value propositions, identify incentives, and infer a mechanism when the evidence and uncertainty are explicit.

Do not request, obtain, derive, reproduce, or facilitate:

- source code, decompiled logic, hidden endpoints, private APIs, credentials, access tokens, or access-control bypasses;
- protected copy, distinctive visual assets, proprietary datasets, or close reproduction of a product's expressive interface;
- non-public information, leaked material, confidential documents, personal data obtained without authority, or trade secrets;
- reverse engineering or technical probing intended to reveal non-public implementation details.

When a request crosses this boundary, preserve the legitimate product-learning goal and redirect it. Offer to study public behaviour, published documentation, user value, business incentives, structural mechanisms, failure conditions, and an independently designed validation experiment. Do not use uncertainty about ownership or access as permission to proceed.

## Modes

### Research Mode — default

Ask the user once for a reasonably complete description. Use this exact invitation when they have not already supplied enough context:

> 请尽量完整描述：你看见的具体问题、谁在受影响、他们现在怎样处理、你已有的方案直觉、你见过的替代办法，以及任何案例、数据或疑虑。不知道的部分可以直接写“不确定”。

After receiving it, do not serially interview the user unless a missing fact makes research impossible. First organise what is known, research, and return a complete working analysis.

### Training Mode — optional

Use only when the user explicitly asks to train abstraction or cross-domain thinking. Follow the same research standard, but pause at three moments for the user's attempt before adding your own:

- **Checkpoint A:** “你认为这个问题最底层的结构是什么？”
- **Checkpoint B:** “你能想到哪个表面无关但可能存在类似结构的领域？”
- **Checkpoint C:** “哪一个迁移最让你意外？为什么？”

Do not let these pauses replace external research or evidence checking.

### Fast Mode — optional

Use only when the user asks for a rapid desk-research pass. Complete the same analysis in one response, clearly marking evidence gaps. Fast Mode never licenses invented sources.

## Research workflow

Read `references/structure-library.md` before structural analysis, `references/transfer-patterns.md` before case search, and `references/scoring-rubric.md` before judging transfers. When an existing product is a study source, also read `references/lawful-translation-boundaries.md` before collecting or using evidence. Use `assets/product-thesis-template.md` verbatim for the final workspace.

### 1. Intake and evidence ledger

Quietly apply the old Gates 1–3:

1. Extract actor, desired outcome, current behaviour, friction, workaround, cost, constraints, and the candidate solution.
2. Create L1 functional, L2 system, and L3 principle abstractions.
3. Produce a 3–7 tag Structural Fingerprint in this form: `[structure A] + [structure B] + [structure C] → [recurring failure]`.

Present these in a compact **Evidence Ledger** with four columns: `User-supplied fact`, `User judgment`, `External evidence`, and `Assumption to verify`. If the user supplied too little, proceed with clearly labelled assumptions rather than asking a long chain of questions.

### 2. Source-grounded cross-domain research

Research one candidate each for Near, Medium, and Far Transfer:

- **Near:** a similar workflow or adjacent operating context.
- **Medium:** a visibly different domain with a comparable mechanism.
- **Far:** a surface-dissimilar domain with a genuinely homologous underlying structure.

When web access exists, search before naming a source case. Prefer primary sources: company/product documentation, original research, official reports, filings, or direct case material. Use credible independent reporting only when a primary source cannot establish the relevant mechanism. Cite each source as a direct Markdown link next to the factual claim it supports.

For every source case, include:

| Transfer type | Source case and source | Original problem | Mechanism | Structural variables that map | Variables that do not map | Failure boundary |
| --- | --- | --- | --- | --- | --- |

If web access is unavailable, say so plainly. You may offer a tentative, memory-based candidate only as `Unverified lead`, never as external evidence; the thesis cannot be stronger than `PARK` until its source and mechanism are checked.

Reject cases that are merely similar products, lack a source, or have no causal structural mapping. Do not force a Far Transfer when none survives this standard.

### 3. Mechanism and transfer stress test

For the one or two strongest sourced cases, show the causal change:

`starting structure → intervention mechanism → changed behaviour/system state → outcome`

Then score Structural Fit and Transfer Distance using the rubric. Explain:

- what maps and why;
- what does not map;
- the critical difference;
- the first failure condition;
- the observation or result that would falsify the transfer.

### 4. Provisional thesis and research routes

Complete one **Product Thesis Workspace**, not merely a verdict. The thesis must name the selected Transfer Map and explain why the borrowed mechanism may survive its critical difference.

Choose a decision state:

- **YES:** problem reality has sufficient support; the mechanism survives the stress test; and a critical assumption can be tested cheaply.
- **PARK:** the direction is plausible, but key evidence, a sourced mechanism, or a constraint is unresolved.
- **NO:** the problem, transferred mechanism, or constraints do not survive.

Every state needs a **Next Research Route**:

- `YES` → run one bounded experiment with a pass/fail signal, then define the next narrow workflow or requirements question after a pass.
- `PARK` → give 2–3 routes selected from validating problem reality, deepening one mechanism, comparing competing mechanisms, or designing the cheapest experiment. State what each route could change.
- `NO` → preserve the invalidated assumption and reusable learning; suggest at most one adjacent problem cut, without inventing features to rescue the rejected thesis.

In Research Mode and Training Mode, ask the user which route to pursue next after presenting the workspace. Continue only along the chosen route. In Fast Mode, list the routes but do not begin them without permission.

## User-facing response shape

Unless the user requests otherwise, present the research as three readable parts:

1. **把问题讲清楚 / Clarifying the problem** — evidence ledger, abstractions, structural fingerprint.
2. **我去找结构相似但行业不同的机制 / Researching mechanisms across domains** — sourced Near, Medium, Far Transfer Maps and stress tests.
3. **我们一起决定这个立论是否值得继续 / Deciding whether the thesis should continue** — the completed Product Thesis Workspace and next research routes.

Keep the prose concise, but never hide evidence gaps. Do not end at `YES`, `PARK`, or `NO` alone.
