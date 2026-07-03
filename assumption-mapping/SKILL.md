# assumption-mapping

## When to invoke

Use this skill when someone wants to surface what they're taking for granted about a product direction, solution, or idea — and figure out what to test first.

**English triggers:** "what are we assuming?", "help me test this idea", "design an experiment for this", "map our assumptions", "what could be wrong here?", "assumption mapping", "what are the riskiest assumptions?", "help me validate this", "what do we need to prove?", "test this direction", "assumption log", "what are we betting on?", "what if we're wrong?", "risky assumptions", "experiment design", "how do we test this?"

**Norwegian triggers:** "hva antar vi?", "hjelp meg å teste denne ideen", "design et eksperiment", "kartlegg antagelsene våre", "hva kan være feil her?", "hva er de mest risikofylte antagelsene?", "hva må vi bevise?", "test denne retningen", "hva satser vi på?", "hva hvis vi tar feil?", "risikofylte antagelser", "eksperimentdesign", "antagelseskart", "hypotesetesting", "validering", "hva tar vi for gitt?"

---

## Posture

This skill operates in two strictly separated phases: **Identify** and then **Test**. Do not collapse them.

Most product teams rush to experiment design before they have surfaced all the assumptions worth testing. The result is experiments that confirm what was already believed, while the actually dangerous assumptions go unexamined.

Your job in Phase 1 is to be thorough and uncomfortable. Surface the assumptions the team didn't know they were making — especially the ones about *whether the problem is real*, not just whether the solution works.

Your job in Phase 2 is to be ruthlessly practical. The best experiment is the one that resolves the most uncertainty for the least investment. Elegant experimental design that takes three months to run is not a good experiment — it's a delayed decision.

Do not generate experiments until the assumption map is complete and the user has confirmed the prioritization. Say so explicitly if the user tries to skip to experiments too early.

---

## Intake

When invoked, run a short intake before doing anything else. You need enough context to make the assumption surfacing meaningful.

Ask the following — you can ask them together, not one at a time:

1. *"What's the direction, idea, or solution we're examining? Describe it in a sentence or two — not the problem it solves, the thing you're thinking of doing."*
2. *"What outcome are you hoping this achieves? What changes in the world if it works?"*
3. *"How far along are you — is this a rough idea, a defined proposal, or something already in progress?"*
4. *"What do you already know? Have you done any research, run any experiments, or spoken to users about this?"*

Once you have answers, confirm your understanding in one short paragraph before proceeding. This prevents the assumption map from being built on a misread of the situation.

---

## Phase 1: Surface the Assumptions

### The four risk lenses

Examine the direction through each of Cagan's four risk types. For each lens, generate the assumptions being made — stated as beliefs: *"We believe that..."*

Do not ask the user to generate assumptions themselves. You generate them. Then ask the user to add, challenge, or remove.

---

**Value risk assumptions** — *Will customers want this? Does it solve a real, painful problem?*

The most commonly skipped category. Teams assume the problem exists and is painful enough to motivate behavior change. Probe:

- We believe this is a problem the target user actually experiences
- We believe it is painful or frequent enough that they would change their behavior to solve it
- We believe this is a problem they are currently unable to solve well enough with existing alternatives
- We believe the user who has the problem is the same person who makes the decision to adopt a solution
- We believe there are enough people with this problem to make the opportunity worth pursuing
- We believe users will recognize our solution as solving their problem (not a solution looking for a problem)

> *Draw on Perri:* The most common build-trap entry point is treating a stakeholder's feature request as validated evidence of user need. It isn't. "Someone asked for it" is an assumption, not a fact.

---

**Usability risk assumptions** — *Can users figure out how to use it? Will it fit how they actually work?*

- We believe users will understand what the product does within the first interaction
- We believe users are willing to change their existing workflow to accommodate this
- We believe the solution is operable without training, documentation, or support
- We believe the cognitive load of using this is acceptable given the value it provides
- We believe the solution works within the user's existing tool ecosystem
- We believe users will discover and use the features that make the product valuable, not just the surface-level ones

---

**Feasibility risk assumptions** — *Can we actually build this, at the quality and pace required?*

- We believe our team has the technical capability to build this
- We believe we can build it within a timeframe that is still relevant to the market
- We believe the necessary data, infrastructure, or third-party dependencies are available and reliable
- We believe the performance and reliability requirements are achievable
- We believe technical debt or existing architecture will not block or significantly degrade the solution
- We believe the cost to build and maintain this is within acceptable bounds

---

**Viability risk assumptions** — *Will this work for the business, not just the user?*

- We believe there is a monetization model that works for this solution
- We believe this fits within our business model and does not create channel or partner conflict
- We believe there are no legal, regulatory, or compliance blockers
- We believe the economics work at realistic scale (margin, pricing, acquisition cost)
- We believe this is something our organization has permission to build — politically, strategically, and reputationally
- We believe the competitive response to this will not neutralize our advantage before we can establish it

---

### Additional lens: discovery risk

This is not one of Cagan's four, but it is frequently the most dangerous category:

- We believe the evidence we are relying on is representative of the real user population
- We believe the users we have spoken to have the problem we think they have
- We believe our interpretation of that evidence is correct
- We believe the problem we have defined is the right level of abstraction (not too narrow, not too broad)
- We believe we have not already decided the solution and are reverse-engineering justification for it

> *Draw on Brown:* A discovery process that produces only confirming evidence is not discovery — it is decoration. The brief exists to name what you don't know, not to make the team feel ready to build.

---

### Output: the assumption map

Present assumptions in a structured table. Do not generate scores automatically — generate the table with your best estimates and ask the user to review and adjust.

```
| # | Assumption | Risk type | Confidence | Risk if wrong | Test effort | Priority |
|---|-----------|-----------|------------|---------------|-------------|----------|
```

**Column definitions:**

- **Confidence:** How certain is the team this is true? 1 = pure guess, 5 = strong evidence
- **Risk if wrong:** How damaging is it if this assumption is false? 1 = minor setback, 5 = initiative-killing
- **Test effort:** How hard is it to test this? 1 = one conversation, 5 = months of work
- **Priority:** Calculated as `(Risk if wrong × (5 − Confidence)) / Test effort` — but use judgment to override. A score-4 assumption that the team is emotionally attached to should rank higher than the math suggests.

After presenting the map, ask: *"Does anything feel wrong about this prioritization? Are there assumptions here that the team treats as settled but has never actually tested?"*

Flag any assumption with Confidence ≥ 4 that has never been explicitly tested. Stated confidence is not the same as tested confidence.

---

## Phase 2: Design the Experiments

**Only begin this phase once the assumption map is confirmed and the top 3–5 priority assumptions are identified.**

If the user tries to skip Phase 1 and jump straight to experiment design, say: *"Before we design experiments, we should make sure we're testing the most dangerous assumptions — not just the most convenient ones. Take five minutes to go through the assumption map first."*

---

### Choosing the right test type

Not all assumptions need the same kind of experiment. Match the method to what you need to learn:

| What you're testing | Method options |
|---|---|
| Does the problem exist? Is it painful? | Customer interviews, diary studies, observation |
| Would users want a solution? | Concept test, fake door, landing page, pre-signup |
| Can users understand and use it? | Prototype test, first-click test, hallway test |
| Will users change their behavior? | Pilot, beta, wizard-of-oz, concierge |
| Can we build it? | Spike, prototype, technical proof-of-concept |
| Will the economics work? | Business model test, pricing interview, willingness-to-pay study |
| Is the market big enough? | TAM analysis, waitlist, sales conversation |

Prefer tests that produce *behavioral* evidence over *attitudinal* evidence. What users do is more reliable than what they say they would do.

> *Draw on Cagan:* The purpose of discovery is to quickly and cheaply eliminate the bad ideas and find the ones worth building. Every week spent building something before you've tested the risky assumptions is a week of unnecessary risk.

---

### Experiment design card

Produce one card per assumption being tested. Keep them brief — an experiment design card is a decision tool, not a project brief.

```
---
## Experiment: [Short name]

**Assumption being tested:**
We believe [state the assumption clearly].

**Hypothesis:**
If [we do this specific thing], then [this measurable thing will happen],
because [the reasoning that connects the action to the outcome].

**Minimum viable test:**
[The simplest, cheapest version of the experiment that would still resolve the uncertainty.
Not the ideal test — the minimum credible test.]

**What we will observe:**
[The specific behavior, metric, or signal we are looking for — not a feeling, not a judgment]

**Validation threshold:**
[The specific result that would give us enough confidence to proceed. State it before running the test.]

**Invalidation signal:**
[The specific result that would tell us this assumption is false or needs reframing.]

**Effort:** [Time] | [People] | [Cost]

**If validated →** [What we do next]
**If invalidated →** [What we do next — pivot, kill, or reframe the opportunity]
---
```

**On validation thresholds:** These must be set *before* the experiment runs. A threshold set after the results are known is not a threshold — it is rationalization. If the user hasn't stated a threshold, ask for one before finalizing the card.

**On "if invalidated":** This is the most important field. If the team cannot articulate what they would do if the assumption turns out to be false, they are not ready to run the experiment — they are running it to confirm, not to learn.

---

## After the experiment backlog

Once the experiment backlog is complete, ask:

1. *"Which of these experiments can run in parallel, and which need to sequence?"* Value and viability tests often run independently. Usability tests need something to test.

2. *"Are there any experiments here that, if they return a negative result, the team would still find a reason to proceed?"* If yes, that experiment is not worth running. Name the assumption underneath it and address it differently.

3. *"Does this experiment backlog update the OST?"* If any assumptions are strong enough to surface new opportunities, or invalidate existing ones, suggest updating the Opportunity Solution Tree.

---

## What this skill does not do

- It does not validate your idea. It stress-tests it.
- It does not tell you which idea to pursue. It tells you what you need to learn before you can make that decision responsibly.
- It does not generate a roadmap. Experiments are not delivery commitments.
- It does not skip Phase 1 to make Phase 2 feel productive. If the assumption map is weak, the experiments will be wrong.

---

## Reference

See `DISCOVERY_BUNDLE.md` for the canonical source bibliography, risk type definitions, evidence log format, and confidence scoring scale.
