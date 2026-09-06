# Pre-Coding Validation Playbook

Use this playbook after the problem structure and transferred mechanism have been made explicit. Its purpose is to buy decision-relevant evidence before committing to software development.

A polished artifact is not evidence by itself. Choose the smallest test that exposes the most important uncertainty, define the signal in advance, and record results without rescuing the hypothesis after the fact.

## Keep two decisions separate

- **Thesis state — `YES / PARK / NO`:** Does the current product thesis deserve further validation?
- **Action decision — `BUILD / PARK / KILL`:** After a bounded experiment, is there enough evidence to enter a narrow build phase?

`YES` does not automatically mean `BUILD`. It means the thesis is coherent enough to spend the next small unit of effort on a test. `BUILD` requires an experiment result that meets a pre-declared threshold and a scope narrow enough to implement responsibly.

## Choose the uncertainty before the method

| Primary uncertainty | Preferred validation route | Avoid treating as proof |
| --- | --- | --- |
| Does the problem recur and matter? | Problem interviews plus behavioural or workflow evidence | General opinions, compliments, or “I would use it” |
| Is the proposed outcome understandable and desirable? | Concept interview, then a focused landing-page test when traffic can be interpreted | Feedback on polished visuals or friends' encouragement |
| Will the intended buyer pay at a viable level? | Pricing test, paid manual pilot, or a clearly disclosed refundable commitment | A willingness-to-pay survey without consequence |
| Can the transferred mechanism change the target behaviour or outcome? | Wizard-of-Oz or concierge experiment | Engagement with a mock-up that never delivers the mechanism |
| Is the idea too broad to test? | Apply the MVP scope rule before choosing a method | Testing several users, moments, mechanisms, and outcomes at once |

When two uncertainties are equally critical, test the one that would kill or materially reshape the thesis sooner.

## Five validation routes

### 1. Problem interview

- **Question answered:** Does a specific user repeatedly experience the proposed problem strongly enough to change behaviour, spend resources, or accept risk?
- **Concrete setup:** Recruit people who recently encountered the target moment. Ask for the last specific occurrence, what triggered it, what they did step by step, what it cost, what they tried, and what happened. Ask for artefacts or observable workflow evidence when appropriate and authorised.
- **Evidence produced:** Recency, frequency, severity, workaround, switching trigger, decision authority, and actual costs in time, money, risk, or coordination.
- **Pass signal:** A pre-declared proportion of qualified participants independently describes the same costly pattern and has taken observable action to address it.
- **Fail signal:** The event is rare, low-cost, tolerated, solved well enough, or reported only after prompting.
- **Common false positive:** Leading questions make users agree with the researcher's framing; enthusiasm about a future solution is mistaken for evidence of past pain.

Prefer questions about past behaviour. Do not pitch the product during a problem interview.

### 2. Concept interview

- **Question answered:** Does the proposed outcome and mechanism make sense in the user's real workflow, and what objection blocks adoption?
- **Concrete setup:** After establishing recent problem behaviour, show a neutral concept statement or low-fidelity flow. Ask the participant to explain it back, place it into their actual process, compare it with their current alternative, and identify the point where they would stop.
- **Evidence produced:** Comprehension, perceived relevance, workflow fit, trust concerns, switching barriers, and the next action the participant is willing to take.
- **Pass signal:** Qualified participants understand the intended outcome without coaching and take a costly next step such as sharing data under appropriate safeguards, scheduling a pilot, involving a decision-maker, or accepting a follow-up.
- **Fail signal:** The concept needs repeated explanation, solves a low-priority part of the workflow, or creates a larger trust or switching cost than it removes.
- **Common false positive:** Courtesy feedback, design preference, and feature requests are mistaken for adoption intent.

### 3. Landing-page test

- **Question answered:** Will a defined audience take a measurable next step when the value proposition is presented in a realistic acquisition context?
- **Concrete setup:** Create one page for one audience, problem moment, promised outcome, mechanism-level explanation, and call to action. Use a traffic source whose audience and cost can be measured. Clearly disclose waitlist, pilot, preorder, or availability status; do not imply a functioning product when none exists.
- **Evidence produced:** Qualified visits, message comprehension, call-to-action conversion, acquisition cost, follow-through quality, and objections.
- **Pass signal:** A pre-declared number or rate of qualified visitors completes the meaningful call to action at an acceptable acquisition cost, and follow-up confirms they match the target problem.
- **Fail signal:** Relevant traffic does not convert, converters are outside the target segment, or follow-up reveals curiosity without the problem.
- **Common false positive:** Untargeted traffic, novelty clicks, vanity sign-ups, or an unusually strong incentive inflate conversion without demonstrating demand.

### 4. Pricing test

- **Question answered:** Will the intended payer exchange money or another meaningful commitment at a level compatible with the proposed delivery model?
- **Concrete setup:** Present a clearly defined outcome, delivery boundary, price, timing, cancellation/refund terms, and genuine next step. Prefer a paid manual pilot, signed letter of intent with concrete conditions, preorder where lawful and fulfilment is credible, or a disclosed refundable deposit. Test one pricing hypothesis at a time or use a comparison design with interpretable samples.
- **Evidence produced:** Payment, deposit, procurement progression, signed commitment, price objection, decision authority, sales-cycle friction, and gross delivery assumptions.
- **Pass signal:** A pre-declared number or rate of qualified buyers makes the required commitment at or above the tested price, with delivery economics that are not obviously untenable.
- **Fail signal:** Interest disappears at the price, the wrong party controls budget, the buying process overwhelms the value, or delivery cost exceeds plausible revenue.
- **Common false positive:** Hypothetical willingness to pay, discounts that erase viability, non-binding praise from non-buyers, or one exceptional customer is treated as a market.

Never charge for something that cannot be responsibly delivered. State refund, privacy, consumer, and sector-specific obligations before collecting payment or data.

### 5. Wizard-of-Oz or concierge experiment

- **Question answered:** If the proposed mechanism is delivered manually or with limited automation, does it create the expected user or system outcome?
- **Concrete setup:** Deliver one core mechanism to a small, qualified sample using manual operations behind a simple interface or service process. Define service limits, human involvement, response time, data handling, escalation, and stopping conditions. Disclose human involvement when non-disclosure would mislead users or create safety, privacy, professional-reliance, or regulatory risk.
- **Evidence produced:** Outcome change, completion, repeat use, time to value, failure modes, operational load, trust response, and willingness to continue or pay.
- **Pass signal:** The mechanism produces the pre-declared outcome for the target users within acceptable manual effort and without unacceptable legal, ethical, safety, or trust costs.
- **Fail signal:** Outcomes do not improve, users require a different mechanism, manual effort cannot plausibly be reduced, or the test creates unacceptable risk.
- **Common false positive:** Exceptional founder labour, hidden coaching, cherry-picked users, or an outcome measure that rewards activity rather than value.

## MVP scope rule

Before proposing an MVP, constrain it to:

- **one user** — the actor whose behaviour or outcome matters;
- **one moment** — the trigger and bounded workflow being tested;
- **one outcome** — the change the user should experience;
- **one mechanism** — manual or automated, responsible for that change;
- **one success measure** — the pre-declared signal used to decide what happens next.

If the proposal cannot fit this sentence, narrow it before building:

> For `[one user]` at `[one moment]`, deliver `[one mechanism]` to produce `[one outcome]`, measured by `[one success measure]`.

An MVP is not the smallest version of every planned feature. It is the smallest credible test of the core causal claim.

## Experiment Card

Every recommended or completed experiment must state:

1. **Decision to inform:** What decision will this evidence change?
2. **Critical hypothesis:** One falsifiable statement, not a general ambition.
3. **Method and rationale:** Why this route exposes the uncertainty better than a cheaper alternative.
4. **Target sample and recruitment:** Who qualifies, who does not, sample size or stopping rule, and how participants will be reached.
5. **Test asset and procedure:** Interview guide, concept, landing page, price offer, or manual service protocol.
6. **Pass threshold:** The result required before seeing the data.
7. **Disconfirming result:** What result supports `PARK` or `KILL`, including evidence that a different problem or mechanism is present.
8. **False-positive controls:** How leading questions, biased traffic, discounts, founder effort, novelty, or selection bias will be limited.
9. **Ethical and legal considerations:** Consent, privacy, payment/refund, professional reliance, safety, accessibility, sector rules, and truthful representation as applicable.
10. **Time and cost cap:** The maximum effort justified before reviewing the decision.
11. **Result:** Observed evidence only; do not fill this field before the experiment.
12. **Next action:** `BUILD`, `PARK`, or `KILL`, with a reason tied to the threshold.

## Decision rules after the experiment

### BUILD

Choose `BUILD` only when the critical result meets the declared pass threshold, the mechanism—not merely the presentation—has meaningful support, the narrow scope is clear, and no unresolved constraint makes implementation irresponsible. State exactly what bounded workflow may now enter requirements or development.

### PARK

Choose `PARK` when evidence is promising but inconclusive, the sample or acquisition context is unreliable, a constraint remains unresolved, or competing mechanisms cannot yet be distinguished. Name the missing evidence, one next test, and the evidence that would move the decision.

### KILL

Choose `KILL` when the critical hypothesis is disconfirmed, the economics or operating burden cannot plausibly work, the mechanism fails in the target context, or the legal, ethical, safety, or trust cost is unacceptable. Preserve the reusable learning and identify at most one adjacent problem worth reframing; do not add features merely to avoid the conclusion.

## Producing the validation artifact

Once the user selects a route, produce the practical artifact they need: an interview guide, concept-test script, landing-page copy and measurement plan, pricing experiment, or Wizard-of-Oz protocol. Do not write software unless the user separately asks for implementation after the relevant decision threshold is met.
