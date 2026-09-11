---
name: product-thesis
description: >-
  Research and validate a defensible product thesis before designing or coding a
  product, AI tool, website, app, service, or feature. Use when a user brings a
  product idea or industry problem, asks whether or what to build, wants to learn
  from and lawfully translate an existing product's mechanism, or needs user
  interviews, a landing-page or pricing experiment, Wizard-of-Oz validation, or
  a narrow MVP decision. Default to source-grounded Research Mode, stress-test
  cross-domain transfer, and prefer decision-relevant evidence before coding.
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

## User-first output contract

The research may be detailed; the first answer should not feel like a research database. Keep the seven gates, evidence labels, transfer scores, and full tables in the reasoning layer unless the user asks to inspect them.

Before showing a dossier, ledger, scorecard, or workspace, answer in the user's language and in ordinary prose:

1. **Provisional judgment:** Say what you currently think and how confident that judgment is. Put `YES`, `PARK`, or `NO` after the explanation, not in place of it.
2. **Best reason to continue:** Explain the strongest evidence or structural reason in concrete language.
3. **Strongest reason against:** Give the competing explanation, non-mapping variable, or failure condition most likely to overturn the thesis.
4. **Recommended action:** Recommend one next action. Say who to involve, what to do, what to observe, and what result would change the judgment.

Read and adapt `assets/product-judgment-brief.md` for this default response. Treat it as a writing order, not a form to fill mechanically.

Use progressive disclosure:

- Do not open with L1/L2/L3 labels, a Structural Fingerprint, Gate names, scores, or a large table. Translate the important reasoning into plain language first.
- In the main answer, explain the one cross-domain mechanism that matters most. Mention rejected or weaker transfers only when they materially change the judgment.
- Keep citations next to the claims they support, but do not make a source list the main story.
- Match the user's language. Do not duplicate the answer bilingually unless the user asks.
- Offer the complete Product Thesis Workspace after the brief. Show it when the user asks for the evidence trail, wants to compare mechanisms, needs a durable research record, or requests a deep analysis.
- Prefer one recommended route over a menu. Offer alternatives only when two routes are genuinely close or the user asks to compare them.

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

After receiving it, do not serially interview the user unless a missing fact makes research impossible. First organise what is known and complete the necessary research, then return a readable Product Judgment Brief. Keep the full working analysis available for expansion rather than placing it all in the first answer.

### Training Mode — optional

Use only when the user explicitly asks to train abstraction or cross-domain thinking. Follow the same research standard, but pause at three moments for the user's attempt before adding your own:

- **Checkpoint A:** “你认为这个问题最底层的结构是什么？”
- **Checkpoint B:** “你能想到哪个表面无关但可能存在类似结构的领域？”
- **Checkpoint C:** “哪一个迁移最让你意外？为什么？”

Do not let these pauses replace external research or evidence checking.

### Fast Mode — optional

Use only when the user asks for a rapid desk-research pass. Complete the same analysis in one response, clearly marking evidence gaps. Fast Mode never licenses invented sources.

## Research workflow

Read `references/structure-library.md` before structural analysis, `references/transfer-patterns.md` before case search, and `references/scoring-rubric.md` before judging transfers. When an existing product is a study source, read both `references/lawful-translation-boundaries.md` and `references/product-study-method.md` before collecting or using evidence. Read `references/validation-playbook.md` when selecting, designing, interpreting, or continuing a pre-coding experiment. Use `assets/product-judgment-brief.md` for the default user-facing answer. Use `assets/product-thesis-template.md` only for the expanded workspace and adapt it to the user's language and the evidence actually available.

The user may begin with a target problem, a source product, or both. If only a source product is supplied, complete the product study before asking where to translate it; do not invent a target context. If only a target problem is supplied, clarify its structure before selecting source products. When both are supplied, investigate the source on its own terms before testing the proposed transfer.

### 1. Intake and evidence ledger

Quietly apply the old Gates 1–3:

1. Extract actor, desired outcome, current behaviour, friction, workaround, cost, constraints, and the candidate solution.
2. Create L1 functional, L2 system, and L3 principle abstractions.
3. Produce a 3–7 tag Structural Fingerprint in this form: `[structure A] + [structure B] + [structure C] → [recurring failure]`.

Maintain a compact **Evidence Ledger** with four categories: `User-supplied fact`, `User judgment`, `External evidence`, and `Assumption to verify`. Do not display the ledger by default. Surface only the facts and uncertainties that change the provisional judgment. If the user supplied too little, proceed with clearly labelled assumptions rather than asking a long chain of questions.

### 2. Source Product Dossier — when studying an existing product

Use the six lenses in `references/product-study-method.md`:

1. user and context;
2. value proposition;
3. key mechanism;
4. business model and incentives;
5. growth and retention;
6. constraints and failure boundary.

For each lens, cite a public source or label the statement `Inference`; keep unresolved claims as `Unverified lead`. Separate **Surface features** from the **Underlying mechanism**, then show the mechanism causally:

`starting structure → intervention → changed behaviour or system state → outcome`

Do not let one admired source product become the answer by default. Test at least one competing explanation—for example brand, distribution, timing, capital, regulation, or a different mechanism—when it could plausibly explain the observed result.

If a target context is known, create the **Target-Context Translation Map** from the reference. Map actors, triggers, information, trust, incentives, payer, workflow, regulation, feedback, and time to value. A transfer advances only when the critical non-mapping variable and its consequence are explicit.

### 3. Source-grounded cross-domain research

Research one candidate each for Near, Medium, and Far Transfer:

- **Near:** a similar workflow or adjacent operating context.
- **Medium:** a visibly different domain with a comparable mechanism.
- **Far:** a surface-dissimilar domain with a genuinely homologous underlying structure.

When web access exists, search before naming a source case. Prefer primary sources: company/product documentation, original research, official reports, filings, or direct case material. Use credible independent reporting only when a primary source cannot establish the relevant mechanism. Cite each source as a direct Markdown link next to the factual claim it supports.

For every source case, record internally or in the expanded workspace:

| Transfer type | Source case and source | Original problem | Mechanism | Structural variables that map | Variables that do not map | Failure boundary |
| --- | --- | --- | --- | --- | --- |

If web access is unavailable, say so plainly. You may offer a tentative, memory-based candidate only as `Unverified lead`, never as external evidence; the thesis cannot be stronger than `PARK` until its source and mechanism are checked.

Reject cases that are merely similar products, lack a source, or have no causal structural mapping. Do not force a Far Transfer when none survives this standard.

### 4. Mechanism and transfer stress test

For the one or two strongest sourced cases, show the causal change:

`starting structure → intervention mechanism → changed behaviour/system state → outcome`

Then score Structural Fit and Transfer Distance using the rubric. Explain:

- what maps and why;
- what does not map;
- the critical difference;
- the first failure condition;
- the observation or result that would falsify the transfer.

### 5. Provisional thesis and research routes

Develop enough of the **Product Thesis Workspace** to support the judgment, but do not display the full workspace by default. The thesis must identify the selected Transfer Map and explain why the borrowed mechanism may survive its critical difference. Present that reasoning first through the Product Judgment Brief.

Choose a decision state:

- **YES:** problem reality has sufficient support; the mechanism survives the stress test; and a critical assumption can be tested cheaply.
- **PARK:** the direction is plausible, but key evidence, a sourced mechanism, or a constraint is unresolved.
- **NO:** the problem, transferred mechanism, or constraints do not survive.

Every state needs a **Next Research Route**:

- `YES` → run one bounded experiment with a pass/fail signal, then define the next narrow workflow or requirements question after a pass.
- `PARK` → recommend the single route most likely to reduce the decisive uncertainty: validating problem reality, deepening one mechanism, comparing competing mechanisms, or designing the cheapest experiment. Mention up to two alternatives only when they are genuinely close, and state what each could change.
- `NO` → preserve the invalidated assumption and reusable learning; suggest at most one adjacent problem cut, without inventing features to rescue the rejected thesis.

In Research Mode and Training Mode, ask whether the user wants to take the recommended action or inspect the research trail after presenting the brief. Continue only along the chosen route. In Fast Mode, state the recommendation but do not begin the next action without permission.

### 6. Pre-coding validation — after the user chooses a route

Keep two decisions separate:

- `YES / PARK / NO` describes whether the thesis deserves further validation.
- `BUILD / PARK / KILL` describes what to do after a bounded experiment.

A `YES` thesis is not permission to build. It means the core reasoning is coherent enough to test. Until a real experiment has run, the action state is `NOT YET ELIGIBLE`; do not pre-fill `BUILD`, `PARK`, or `KILL`. Select the validation method by the uncertainty:

- recurring problem and real cost → problem interview plus behavioural evidence;
- comprehension and desirability → concept interview, then a landing-page test when qualified traffic is available;
- willingness to pay → pricing test or paid manual pilot;
- whether the transferred mechanism changes the outcome → Wizard-of-Oz or concierge experiment;
- scope too broad to interpret → first reduce it to one user, one moment, one outcome, one mechanism, and one success measure.

Every experiment needs a critical hypothesis, target sample, method, pass threshold declared in advance, disconfirming result, false-positive controls, ethical and legal considerations, time and cost cap, and the next decision. Never invent a result for an experiment that has not run.

After the user selects the route, produce the practical research artifact: interview questions, a concept-test script, landing-page copy and measurement plan, a pricing experiment, or a Wizard-of-Oz protocol. Do not write software unless the user separately requests implementation after the decision threshold is met.

Use the result to decide:

- **BUILD:** the pass threshold is met, the core mechanism has support, the scope is narrow, and no unresolved constraint makes implementation irresponsible. State the bounded workflow that may enter requirements or development.
- **PARK:** evidence is promising but inconclusive or a material constraint remains. State what is missing, the next test, and what could change the decision.
- **KILL:** the critical hypothesis, economics, mechanism, or acceptable-risk boundary fails. Preserve the learning; do not add features merely to avoid the conclusion.

## User-facing response shape

Default to a short decision narrative, even when the underlying research is extensive:

1. Start with the provisional judgment in plain language.
2. Explain the strongest reason for it and the strongest reason it may be wrong.
3. Describe the most useful transferred mechanism as a causal idea, not as a product feature.
4. End with one recommended action and the observation that would change the judgment.
5. Offer to expand the evidence ledger, Source Product Dossier, Near/Medium/Far research, scores, and full Product Thesis Workspace.

When the user asks for the full research record, use `assets/product-thesis-template.md`. Do not force empty sections, repeat the same conclusion under several headings, or translate every heading into two languages. Keep the prose concise, but never hide evidence gaps. Do not end at `YES`, `PARK`, or `NO` alone.
