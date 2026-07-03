# solution-exploration

Generates a range of distinct solution directions attached to a specific OST opportunity — not a single answer, not a brainstorm dump. Forces divergence before convergence, structures ideation by strategic angle, and produces a reasoned prototype recommendation.

Use this skill when someone wants to generate solution ideas for a known opportunity, explore what they could build, or ensure they aren't converging prematurely on a single direction.

**English triggers:** "generate solution ideas", "help me ideate on this", "what could we build for this opportunity?", "brainstorm solutions", "explore solutions", "solution generation", "what are our options here?", "help me think through solutions", "I need ideas for this", "what directions could we go?", "solution exploration", "ideate on this opportunity", "what could we build?", "think through options", "what are the possible approaches?"

**Norwegian triggers:** "generer løsningsideer", "hjelp meg å idémyldre om dette", "hva kan vi bygge for denne muligheten?", "utforsk løsninger", "løsningsgenerering", "hva er alternativene våre?", "hjelp meg å tenke gjennom løsninger", "jeg trenger ideer til dette", "hvilke retninger kan vi gå?", "løsningsutforsking", "idémyldre om denne muligheten", "hva kan vi bygge?", "tenk gjennom mulige løsninger", "hva er mulige tilnærminger?", "hvilke løsninger finnes?", "hjelp meg å se mulighetene"

---

## Posture

This skill operates at the boundary between discovery and delivery — the moment when an understood opportunity meets the question "so what do we actually do?"

This moment is where most teams fail. They converge on the first reasonable idea, dress it as a decision, and move to planning. The rest of the option space — including potentially better, cheaper, or more testable directions — goes unexplored.

Your job is to force genuine divergence *before* any evaluation happens. That means generating solutions from different strategic angles, not variations of the same idea. A list of five solutions that are all "improved versions of feature X" is not ideation — it is elaboration of a decision already made.

The discipline here is drawn from Cagan: **a team that always knows what it's going to build before doing discovery is not an empowered product team — it is a feature factory with extra steps.** The point of exploring multiple solution directions is not to create work. It is to make the choice of which direction to pursue a real, informed decision rather than a default.

Before generating anything, you need a confirmed opportunity. A solution that is not attached to a real opportunity is a feature request in disguise. Do not proceed without one.

---

## Intake

When invoked, run a short intake before doing anything else. Ask these questions together — they can be answered in a single message:

1. *"Which opportunity are we generating solutions for? Describe it in the user's terms, not the product's. If you have an OST, share the opportunity node."*

2. *"What do we know about this opportunity — is it assumed, observed from research, or validated? What's the evidence?"*

3. *"What outcome is this opportunity connected to? Knowing the outcome helps us evaluate whether a solution direction is pointing in the right direction."*

4. *"What constraints are in play — technical, business, team capability, timeline? I'll generate across the full possibility space, but constraints affect which directions are worth pursuing now versus later."*

5. *"Has anything already been tried or seriously considered for this opportunity? I want to make sure we're genuinely exploring, not just generating cover for a decision that's already been made."*

After gathering answers, do a quick confirmation pass:

- If the opportunity is phrased in product or solution language ("users need a better X"), reframe it. *"That's a solution framing. What's the underlying user need or friction that makes them want X? Let's anchor to that before we generate directions."*
- If there is no clear outcome, ask for it. A solution that moves the outcome is a good solution. A solution that doesn't is scope creep.
- If the team already has a preferred solution in mind, name it. *"It sounds like you're already leaning toward [X]. I'll include that as one direction — but I'm going to generate four others from different angles, because the point of this exercise is to make sure [X] is the right choice, not the only one you looked at."*

Confirm your understanding of the opportunity in one sentence before proceeding.

---

## Phase 1: Derive Design Principles

Before generating any solutions, derive 3–5 design principles specific to this opportunity.

Design principles are not values ("be simple", "be fast"). They are **opinionated constraints on the solution space** that emerge from what you know about the opportunity, the users, and the context. A good design principle rules things out — if a principle doesn't eliminate any solution directions, it isn't doing any work.

> *Draw on Brown:* Design principles are how a team makes design decisions consistently without relitigating the same values in every meeting. They are discovered, not invented — they should emerge from research, not be wished into existence.

Derive principles by reasoning through:
- What do we know about how users experience this opportunity? (What they value, what frustrates them, what context they're in)
- What does the desired outcome tell us about what a solution must achieve?
- What constraints (technical, business) are non-negotiable, and what do they imply about the solution space?
- What have prior attempts or analogous products revealed about what doesn't work here?

**Format each principle as a directional statement, not a vague aspiration:**

| # | Principle | What it rules out |
|---|-----------|-------------------|
| P1 | [e.g. "Reduce decision load at the moment of highest friction"] | [e.g. "Solutions that add configuration options or choices at that step"] |
| P2 | ... | ... |

Present the principles. Ask: *"Do any of these feel wrong, or are there constraints I've missed that should shape the solution space?"* Adjust before proceeding to Phase 2.

---

## Phase 2: Generate Solution Directions by Angle

Generate **5 solution directions**, one for each of the following strategic angles. These angles are not optional — the point is that they produce genuinely different types of solutions, not variations of the same approach.

Do not evaluate as you generate. Diverge first. Evaluation happens in Phase 3.

---

### Angle 1: The Minimal Solution
**Question:** What is the lightest-weight thing we could do that still meaningfully addresses this opportunity?

Minimal does not mean poor quality. It means the version that requires the least investment to deliver real value. This angle is systematically undervalued because it looks unimpressive in a roadmap — but it often tests value risk faster and cheaper than any other direction.

Force yourself to go genuinely small. If the minimal solution sounds like a reasonable product decision, go smaller.

> *Draw on Cagan:* The purpose of discovery is to find the product equivalent of a surgical strike — the smallest change that generates the most learning or value. Teams that skip the minimal option are implicitly assuming they already know the right scale of the solution.

---

### Angle 2: The Workflow Redesign
**Question:** What if we changed the context around the opportunity, not just the touchpoint?

Most products address symptoms. This angle asks: what is happening *before* and *after* the moment of friction, and what would it look like to address the whole flow rather than a single interaction? This often produces solutions that are harder to build but substantially more valuable — because they eliminate the problem rather than managing it.

Draw on the journey context from intake. If you don't have journey context, note it explicitly: *"A fuller workflow analysis would strengthen this direction — consider using the `research-synthesis` skill to map the journey before building this option."*

---

### Angle 3: The Analogue
**Question:** How has a best-in-class product in a *different* domain addressed the same underlying type of problem?

This angle breaks category thinking. The type of problem (trust, onboarding, decision overload, lack of feedback, coordination cost) almost certainly has precedents in adjacent domains. Mining those precedents surfaces solution patterns the team wouldn't generate from inside their own product context.

Identify the underlying *problem type* first — then find 1–2 analogues from different industries. Describe how their solution addressed the same underlying dynamic, then translate the *mechanism*, not the interface.

> *Draw on Brown:* The best inspiration for a solution rarely comes from direct competitors. Competitors have the same category blindness you do. Look at how Duolingo handles dropout prevention, how Airbnb handles trust between strangers, how Monzo handles financial anxiety — the mechanisms transfer even when the domains don't.

---

### Angle 4: The Empowerment Solution
**Question:** What if instead of solving the problem for users, we gave them the capability to solve it themselves?

Many products solve problems by removing user agency — the product makes the decision, does the thing, completes the step. This angle asks: what would it look like to make the user more capable, more informed, or more in control instead?

Empowerment solutions are often more durable — they create a different kind of relationship with the product — but they require more from users, so they carry higher usability risk. Note this explicitly.

---

### Angle 5: The Systems Solution
**Question:** What if this opportunity is a symptom, and there is a root cause upstream that no one has directly addressed?

This angle asks the team to question whether they are solving the right problem at the right level. Sometimes the friction users experience at point X exists because of a structural failure at point Y — and no amount of improving X will fully resolve it.

This direction often requires cross-team or cross-product coordination. If it does, name it — the solution may be correct but face viability risk precisely because of organizational complexity.

---

### Output format for each direction

Present all five directions in this structure:

```
---
## [Number]. [Direction title]
**Angle:** [Minimal / Workflow Redesign / Analogue / Empowerment / Systems]

**Premise:** [One sentence — what is this solution doing, in plain language?]

**How it addresses the opportunity:**
[2–4 sentences. Explain the mechanism: why would this move the opportunity in the direction of the outcome? Be specific — do not just restate the premise.]

**Strongest assumption:**
We believe [the single riskiest thing that has to be true for this direction to work].

**Design principles check:**
[Does this direction satisfy the principles from Phase 1? Flag any tension explicitly.]

**Rough shape:**
[What would a version 1 of this look like? Specific enough to be testable — not a spec, but not just a label.]
---
```

After presenting all five, add a brief note: *"These are directions, not decisions. Before we evaluate, sit with all five — including the ones that feel uncomfortable or too simple."*

---

## Phase 3: Evaluate and Recommend

**Only begin this phase once all five directions have been presented and the user has had a chance to react.**

If the user immediately begins dismissing options without engaging with them, slow it down: *"Before we rule anything out, I want to make sure we're evaluating on the right criteria. What specifically concerns you about [direction]? Is it the risk, the cost, or does it not feel like it addresses the opportunity?"*

---

### Evaluation matrix

Score each direction across three dimensions. Do not calculate an overall score — use the matrix to have a conversation, not to produce a winner algorithmically.

| Direction | Value potential | Testability | Fit with constraints | Biggest risk |
|-----------|----------------|-------------|----------------------|--------------|
| 1. Minimal | | | | |
| 2. Workflow | | | | |
| 3. Analogue | | | | |
| 4. Empowerment | | | | |
| 5. Systems | | | | |

**Column definitions:**
- **Value potential:** If this worked, how much would it move the outcome? (1–5)
- **Testability:** How quickly and cheaply could we get signal on the riskiest assumption? (1–5, where 5 = days, 1 = months)
- **Fit with constraints:** How well does this work within the stated constraints? (1–5)
- **Biggest risk:** Name it, don't score it. The most important column.

Ask the user to help fill in the scores. Don't fill them unilaterally — the act of scoring forces the conversation that produces the recommendation.

---

### Prototype recommendation

After completing the matrix, produce a recommendation in this form:

```
---
## Recommendation: Prototype [Direction N] first

**Why this direction:**
[2–3 sentences. Explain the reasoning — not just "highest score," but what combination of value potential,
testability, and risk profile makes this the right first test. Reference the evaluation matrix explicitly.]

**What to test:**
[Name the single most important assumption. The prototype should be designed to resolve this — not to
show off the solution.]

**What to build as a prototype:**
[The minimum fidelity needed to test that assumption. Be specific. If a paper sketch resolves the key
assumption, say so. Do not recommend a high-fidelity prototype for a value risk assumption.]

**What this prototype cannot tell us:**
[Name the things a positive prototype result will NOT validate — so the team doesn't over-interpret results.]

**If this direction fails:**
[Which direction to test next, and why.]
---
```

The recommendation must include a *"if this direction fails"* path. A recommendation without a fallback is a guess dressed as a plan.

---

## After the recommendation

Once the recommendation is delivered, ask two closing questions:

1. *"Is there a direction here that the team is emotionally attached to — that would be pursued regardless of what the prototype tells us?"* If yes, that direction should not be the first prototype. It should be the last, after the team has seen what the evidence says about the others.

2. *"Does this output need to go back into the OST?"* Five solution directions have just been generated for a specific opportunity node. They should be recorded as solution branches under that opportunity in `DISCOVERY.md`. Offer to update the OST, or prompt the user to do so with the `ost-builder` skill.

---

## What this skill does not do

- It does not produce a single recommended solution without exploring alternatives first.
- It does not generate five variations of the same idea and call it divergent thinking.
- It does not proceed without a confirmed, opportunity-framed problem statement.
- It does not validate your pre-existing idea by surrounding it with weaker alternatives.
- It does not produce feature specifications, user stories, or delivery estimates. That is after prototype, after learning, after a direction is confirmed.
- It does not skip design principles to get to ideation faster. Principles are not a preamble — they are what makes the evaluation in Phase 3 principled rather than subjective.

---

## Reference

See `DISCOVERY_BUNDLE.md` for the canonical source bibliography and full bundle routing map.
