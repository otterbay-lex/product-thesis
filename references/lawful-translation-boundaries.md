# Lawful Product Study and Mechanism Translation

Use this reference when an existing product, company, workflow, interface, dataset, or proprietary system is offered as a source of learning.

The purpose is to understand why a product may work, extract a general mechanism, and test whether that mechanism can survive in a new context. The source product is evidence, not a blueprint.

This is a practical research boundary, not jurisdiction-specific legal advice. When ownership, licence terms, confidentiality, privacy, or access authority is genuinely uncertain, label the issue and recommend qualified review before relying on the material.

## Evidence labels

Keep these labels visible in notes and outputs:

| Label | Meaning | Minimum support |
| --- | --- | --- |
| **Observed public fact** | Something directly visible through ordinary lawful use or in public material | Identify the product surface, document, page, or user-provided observation |
| **Publicly sourced claim** | Something asserted by an identifiable public source | Provide a direct citation and identify who is making the claim |
| **Inference** | An explanation or causal interpretation produced by the analyst | Show the facts it rests on, the reasoning, and what could make it wrong |
| **Unverified lead** | A potentially relevant claim that has not yet been checked | Do not use it as evidence or let it support a `BUILD` conclusion |

Marketing statements, founder interviews, and public reviews may be useful sources, but they establish that someone made or experienced a claim—not automatically that the proposed causal mechanism is true.

## Research boundary

| Research activity | Allowed public evidence | Not allowed | Safe alternative |
| --- | --- | --- | --- |
| Experience a public product | Ordinary user flows accessed under applicable terms; public demos; public help documentation; the user's own authorised experience | Bypassing authentication, payment, rate limits, role restrictions, or other access controls; using another person's credentials | Use the public demo, documentation, screenshots published by the owner, reviews, or ask the user to describe their authorised experience |
| Study the user problem and value proposition | Product pages, pricing, help centres, public reviews, research, filings, public interviews | Non-public customer lists, leaked research, confidential metrics, unlawfully obtained personal data | Triangulate public claims, independent reviews, public datasets, and fresh user interviews |
| Analyse observable workflow | Publicly visible steps, terminology, feedback loops, permissions, and outcomes | Technical probing designed to reveal hidden implementation; intercepting private traffic; enumerating hidden endpoints | Describe the observable input → action → feedback → outcome sequence and keep implementation unknown |
| Infer a mechanism | Multiple public observations and sources, with the causal explanation labelled `Inference` | Presenting speculation as proprietary knowledge or claiming access to internal algorithms | State competing explanations and name an observation that would falsify the preferred mechanism |
| Learn from public visual or UI material | General layout principles, interaction patterns, information hierarchy, accessibility choices, owner-published screenshots | Copying protected text, illustrations, icons, brand assets, distinctive trade dress, or recreating a screen closely enough to substitute for the original | Abstract the design principle and create an independently expressed interface for the new user's task |
| Understand business and growth logic | Public pricing, terms, filings, published interviews, referral rules, public marketplace policies | Private unit economics, confidential contracts, unpublished experiments, trade secrets | Model plausible economics from public inputs, label assumptions, and validate them independently |
| Translate a mechanism | General ideas such as standardisation, reputation, commitment, progressive disclosure, aggregation, or reinforcement, re-designed for the target constraints | Copying source code, proprietary datasets, protected content, non-public processes, or a source product's feature set wholesale | Restate the mechanism without brand or industry language, then design a target-specific experiment from first principles |
| Compare APIs or integrations | Public developer documentation and authorised test environments | Private APIs, credential extraction, unauthorised access tokens, hidden endpoint discovery, or access-control bypasses | Use documented APIs, request authorised sandbox access, or model the workflow manually for validation |
| Review user-provided material | Material the user is authorised to share, with sensitive details minimised | Leaked, confidential, privileged, stolen, or personal data shared without authority | Ask for a redacted summary, public equivalent, synthetic example, or confirmation of authority |

## Safe translation sequence

Use this sequence so that lawful distance from the source product also improves the product judgment:

1. **Record public evidence.** Separate observed facts, sourced claims, inferences, and unverified leads.
2. **Remove the product identity.** Rewrite the source problem and mechanism without its brand, industry nouns, interface labels, or feature names.
3. **Name the causal mechanism.** Express it as `starting structure → intervention → changed behaviour or system state → outcome`.
4. **Map target variables.** Explain which actors, incentives, information conditions, timing, trust, and constraints correspond.
5. **Break the analogy.** Identify the important variable that does not correspond and the earliest condition under which the transfer fails.
6. **Design independently.** Turn the mechanism into a target-specific hypothesis and experiment. Do not use the source interface or implementation as the specification.

## Redirecting an unsafe request

When only part of the request is unsafe, do not abandon the legitimate objective. Briefly name the boundary and continue with a lawful alternative.

Example response pattern:

> 我不能帮助获取或还原该产品的非公开实现、私有接口、受保护素材或商业秘密。我们仍然可以基于公开产品体验、官方文档、公开定价、用户评价和已发表材料，研究它解决了什么结构性问题、采用了什么机制、该机制迁移到你的场景时会在哪里失效，并设计一个独立的低成本验证。

Escalate to legal or specialist review rather than guessing when the proposed work depends on ambiguous licence rights, contractual restrictions, confidential information, personal-data authority, or a close reproduction of protected expression.
