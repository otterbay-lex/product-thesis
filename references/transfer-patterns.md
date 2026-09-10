# Transfer Patterns

These are source-backed mechanism exemplars, not product templates. Use them to learn how to separate public facts from causal inference and how to state a transfer's failure boundary. Do not reuse an exemplar merely because its company name is familiar.

For a live product thesis, research current sources again. Product behaviour and operating conditions can change after this library is published.

## Airbnb — making heterogeneous supply more transactable

### Public sources

- [Airbnb Terms of Service](https://www.airbnb.com/help/article/2908) describes a marketplace in which hosts publish listings and guests communicate and transact.
- [Reviews for homes](https://www.airbnb.com/help/article/13) explains that reviews follow eligible stays and can inform future guests.
- [Identity verification](https://www.airbnb.com/help/article/450) says verification is intended to promote trust and reduce fraud, while warning that no process is perfect.
- [Location-verification limitations](https://www.airbnb.com/help/article/3542) says verification does not guarantee all listing details, safety, or quality.

### What is observed or publicly claimed

- **Publicly sourced claim:** Airbnb combines listings, communication, booking, reviews, identity checks, and selected protections around transactions between hosts and guests.
- **Observed limitation:** Airbnb expressly limits what identity and location verification establish; a badge is not a guarantee of quality, safety, or truthfulness.

### What is inferred

- **Underlying problem:** Valuable but non-standard private capacity is difficult for strangers to compare, trust, and transact over.
- **Structural fingerprint:** `fragmented supply + standardisation problem + information asymmetry + trust deficit + matching cost`.
- **Mechanism:** `heterogeneous private supply → structured representation + transaction-linked reputation + bounded verification/risk controls → lower uncertainty and transaction friction → more supply can be considered and booked`.
- **Business and incentive logic:** The marketplace benefits when more credible supply and demand can transact; reviews and verification may improve confidence, but also create moderation, privacy, fairness, and false-assurance costs.

### Transferable principle and boundary

- **Transferable principle:** When dispersed capacity exists but is hard to use, make it legible, attach credible evidence to completed interactions, and provide only the transaction infrastructure and risk controls the context needs.
- **What maps:** Fragmented supply, repeated matching, pre-transaction uncertainty, and the ability to standardise a minimum set of attributes.
- **What does not automatically map:** Legal permission to supply, quality comparability, transaction frequency, harm severity, insurance economics, and the target users' willingness to trust peer evidence.
- **Failure boundary:** The mechanism weakens when supply cannot be meaningfully standardised, transactions are too rare to generate reputation, errors cause irreversible or high-stakes harm, or verification creates more privacy and operational cost than trust.
- **Do not copy:** Listing layouts, badges, review screens, brand language, or platform rules. Re-test which evidence and risk allocation the target actually needs.

## Duolingo — converting distant value into repeated action

### Public sources

- [Duolingo 2025 Form 10-K](https://investors.duolingo.com/static-files/f19d76fb-dee4-4f13-96ae-138ebfd0f2d3) describes bite-sized lessons, points, streaks, collaboration, and competition as ways to encourage return to learning.
- [Duolingo's article on streaks and habit research](https://blog.duolingo.com/how-duolingo-streak-builds-habit/) explains the intended role of streaks in supporting repeated study.

### What is observed or publicly claimed

- **Publicly sourced claim:** Lessons can be completed in short sessions, and completion can award points and extend streaks.
- **Publicly sourced claim:** Duolingo says these elements are designed to support motivation and repeated learning. This establishes product intent, not independent proof that streaks alone cause learning outcomes.

### What is inferred

- **Underlying problem:** A long-term benefit loses against immediate effort, distraction, and the cost of restarting.
- **Structural fingerprint:** `delayed reward + intention-action gap + weak immediate feedback + habit inertia`.
- **Mechanism:** `distant benefit + effortful repetition → small action unit + immediate feedback + visible continuity → lower restart cost and stronger short-term reinforcement → more opportunities for repeated practice`.
- **Business and incentive logic:** Repeat use can support both learning exposure and product retention, so engagement and user benefit may align—but can diverge when maintaining a streak becomes the goal rather than meaningful practice.

### Transferable principle and boundary

- **Transferable principle:** For beneficial behaviour with delayed rewards, reduce the activation energy of one useful repetition and make progress quickly visible.
- **What maps:** Frequent repeatable behaviour, low-cost feedback, a meaningful minimum action, and a user who already values the distant outcome.
- **What does not automatically map:** Whether daily cadence is appropriate, whether the action produces real progress, and whether external reinforcement crowds out intrinsic or professional motivation.
- **Failure boundary:** The mechanism fails when tasks cannot be safely divided, quality requires long uninterrupted work, the reward encourages gaming or anxiety, or continuity measures activity without the intended outcome.
- **Do not copy:** Streak icons, points, mascots, leagues, or lesson screens. Test the smallest valuable repetition and the right feedback cadence for the target behaviour.

## GitHub pull requests — coordinating work through reviewable change objects

### Public sources

- [About pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests) describes pull requests as a place to propose changes and track their discussion and progress.
- [Resolving reviews](https://docs.github.com/en/pull-requests/concepts/resolving-reviews) explains that reviews, comments, commits, and automated checks remain connected to the proposed change.

### What is observed or publicly claimed

- **Observed public fact:** A pull request binds a proposed change, its evolving commits, review comments, status, and merge decision into a traceable workflow.
- **Observed public fact:** New commits update the proposal and can rerun automated checks while unresolved review comments remain visible.

### What is inferred

- **Underlying problem:** Distributed contributors need to change a shared artifact without losing context, accountability, or a reviewable decision boundary.
- **Structural fingerprint:** `coordination cost + handoff loss + change ambiguity + verification gap + accountability gap`.
- **Mechanism:** `shared artifact with distributed changes → bounded change proposal + visible diff + threaded review + checks + explicit acceptance → inspectable commitments and lower handoff ambiguity`.
- **Business and incentive logic:** Contributors can work asynchronously while maintainers retain decision authority; the value depends on participants accepting the common artifact and review process.

### Transferable principle and boundary

- **Transferable principle:** When collaboration breaks at handoffs, make the proposed change—not general conversation—the unit of review, evidence, and decision.
- **What maps:** Versionable artifacts, bounded changes, identifiable reviewers, reversible revisions, and an explicit acceptance point.
- **What does not automatically map:** Tacit work, physical operations, negotiations that cannot be exposed, urgent decisions, or contexts in which a diff omits the real-world consequence.
- **Failure boundary:** The mechanism degrades when the artifact cannot represent the work, review latency exceeds the decision window, authority is unclear, or visibility creates confidentiality or participation harms.
- **Do not copy:** Repository metaphors, pull-request screens, or software terminology. Translate the change-object and review logic into the target workflow's own language.

## Wikipedia — combining open contribution with visible revision and source rules

### Public sources

- [Wikipedia's verifiability policy](https://en.wikipedia.org/wiki/Wikipedia:Verifiability) requires published material to be attributable to reliable sources under the policy's conditions.
- [Wikipedia's consensus policy](https://en.wikipedia.org/wiki/Wikipedia:Consensus) describes consensus as the normal basis for editorial decisions.
- [Page history](https://en.wikipedia.org/wiki/Help:Page_history) explains how article revisions and contributors can be inspected and compared.

### What is observed or publicly claimed

- **Observed public fact:** Contributions can be revised; article histories expose prior versions; content rules require sourcing; disputes can be handled through discussion and consensus processes.
- **Observed limitation:** Open participation does not guarantee correctness, balanced coverage, contributor diversity, or fast resolution of disputes.

### What is inferred

- **Underlying problem:** Broad knowledge is too large and distributed for one central editor, but open contribution creates verification, vandalism, conflict, and governance problems.
- **Structural fingerprint:** `fragmented expertise + collective-action problem + contribution friction + verification gap + governance cost`.
- **Mechanism:** `dispersed knowledge → low-friction contribution + source requirements + public revision history + community review/governance → errors and disputes become inspectable and correctable → knowledge can accumulate beyond a central team`.
- **Business and incentive logic:** The model depends on voluntary contribution, reusable public knowledge, and governance labour; contributor motivations and maintenance capacity replace ordinary transaction incentives.

### Transferable principle and boundary

- **Transferable principle:** Lower contribution friction only together with provenance, reversible revision, quality rules, and a workable governance path.
- **What maps:** Dispersed contributors, decomposable knowledge, inspectable revisions, shared norms, and enough reviewers to maintain the commons.
- **What does not automatically map:** Scarce expert judgment, confidential knowledge, legal responsibility, contributor incentives, representation gaps, and situations requiring correctness before publication.
- **Failure boundary:** The mechanism fails when review capacity is thinner than contribution volume, reliable sources do not exist, disputes cannot reach legitimate resolution, or post-publication correction is too late for the harm involved.
- **Do not copy:** Wiki page conventions or “anyone can edit” as a standalone feature. Transfer the coupled contribution-and-governance system, if the target can sustain it.

## Costco — coupling constrained assortment with committed demand

### Public sources

- [Costco corporate overview](https://investor.costco.com/overview/default.aspx) says its model combines membership, low prices, a limited selection, high sales volume, rapid inventory turnover, volume purchasing, efficient distribution, and reduced handling.
- [Costco company profile](https://investor.costco.com/company-profile/default.aspx) describes membership categories and the retailer's value positioning.

### What is observed or publicly claimed

- **Publicly sourced claim:** Costco intentionally offers a limited selection and uses a membership model.
- **Publicly sourced claim:** Costco links high volume and rapid turnover, together with operating efficiencies, to its ability to operate at lower gross margins.

### What is inferred

- **Underlying problem:** Buyers face noisy recurring choices, while a retailer seeking low prices needs concentrated, predictable purchasing power and operational discipline.
- **Structural fingerprint:** `choice overload + search cost + demand fragmentation + purchasing-power gap + incentive alignment`.
- **Mechanism:** `noisy assortment + fragmented demand → curated selection + paid membership + concentrated purchasing + operational simplicity → higher throughput and credible value discipline → repeat demand`.
- **Business and incentive logic:** Membership can create committed demand and a direct reason to preserve member value; limited assortment and volume purchasing may lower handling and procurement complexity. The fee can also exclude low-frequency users.

### Transferable principle and boundary

- **Transferable principle:** In a repeated, high-noise decision, constrained choice can create value when it is coupled to credible curation and enough committed demand to improve economics.
- **What maps:** Repeated purchasing, substitutable options, measurable quality/value, aggregation leverage, and users willing to trade variety for confidence and savings.
- **What does not automatically map:** Long-tail preferences, low purchase frequency, small addressable demand, weak procurement leverage, or categories in which curation errors are costly.
- **Failure boundary:** The mechanism fails when users need high variety, savings do not exceed the commitment cost, demand cannot be concentrated, or the curator lacks a trusted and economically sustainable selection process.
- **Do not copy:** Membership tiers, warehouse presentation, private-label strategy, or assortment rules. Test whether constraint plus commitment improves the target system's decision quality and economics.

## How to use this library

1. Start from the target Structural Fingerprint, not from a company name.
2. Treat every mechanism above as an `Inference` supported—but not proven—by the linked public facts.
3. Re-research the source case and add a competing explanation before using it in a live thesis.
4. State the target variables that map, do not map, and determine failure.
5. Use `scoring-rubric.md`; high novelty or distance never compensates for weak structure or evidence.
