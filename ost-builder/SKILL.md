# ost-builder

## Purpose
Build and maintain the Opportunity Solution Tree (OST) — the backbone discovery artifact that connects a desired outcome to the opportunities that address it, the solutions that address those opportunities, and the experiments that test those solutions.

This is a **living artifact**. It is not built once and filed. It evolves as discovery progresses. Other skills in the discovery bundle read from and write back to it.

---

## Trigger conditions

**English:**
- "Build an OST" / "Build an opportunity solution tree"
- "Map my opportunities" / "Map our discovery"
- "Update the opportunity solution tree" / "Update the OST"
- "Add [opportunity / solution / experiment] to the tree"
- "Where does this idea fit in the tree?"
- "Show me the OST" / "What does our tree look like?"
- "I want to structure my discovery"
- "Help me think through my opportunities"

**Norwegian:**
- "Bygg et mulighetstretre" / "Lag et OST"
- "Oppdater mulighetstreet" / "Oppdater OST"
- "Kartlegg mulighetene" / "Kartlegg oppdagelsen vår"
- "Legg til [mulighet / løsning / eksperiment] i treet"
- "Vis mulighetstreet" / "Hva ser treet ut som nå?"
- "Hjelp meg strukturere produktoppdagelsen"
- "Hvor hører denne ideen hjemme?"
- "Jeg vil strukturere oppdagelsesarbeidet mitt"

---

## The Framework: Opportunity Solution Tree

The OST has four levels. Each level has strict rules. The rules are not optional.

### Level 0 — Desired Outcome
A single measurable outcome the team is working toward. Not a feature. Not a metric to track for its own sake. A *change in human behaviour or system state that the business cares about*.

**Rules:**
- One outcome per tree. If you have multiple, you have multiple trees — or you need to choose a focus.
- Must be specific enough to be measurable.
- Must connect business goals to customer/user behaviour.
- ❌ Bad: "Improve the product" / "Increase engagement"
- ✅ Good: "Increase the share of new users who complete a second session within 7 days of signup"

### Level 1 — Opportunities
Customer needs, pain points, desires, or contexts that — if addressed — would move the outcome. Opportunities are **discovered** through research. They are not invented at a whiteboard.

**Rules:**
- Framed from the customer's perspective, not the business's.
- Must connect logically to the outcome. Ask: if we addressed this, would the outcome move?
- Must not contain product language. "Users need a better onboarding flow" is a solution in disguise. "Users don't understand what value they'll get before committing" is an opportunity.
- Each opportunity must carry an evidence level: `assumed` / `observed` / `validated`.
- Explore breadth before depth. A tree with one well-developed opportunity and ten unexplored ones is a bias, not a strategy.

### Level 2 — Solutions
Specific product, service, or experience responses to a particular opportunity. **Every solution must live under an opportunity.** There are no floating solutions.

**Rules:**
- Explicitly linked to one opportunity.
- A good opportunity should attract 2–4 distinct solution directions — not variations of the same idea.
- Solutions are hypotheses, not commitments. Treat them as options to be tested.
- Specific enough to be testable. Not specific enough to be a spec.

### Level 3 — Experiments
The minimum viable tests designed to validate or invalidate a solution hypothesis before building it.

**Rules:**
- Each experiment must specify: hypothesis / test method / success threshold / effort estimate.
- Prefer speed and cheapness. A passed experiment means confidence is sufficient to proceed — not that you should build the thing.
- Track status: `not started` / `running` / `passed` / `failed` / `inconclusive`.
- An inconclusive experiment is information. Record what made it inconclusive.

---

## The DISCOVERY.md format

The OST lives in `DISCOVERY.md` at the project root. Use this exact structure so other skills can read it reliably.

```markdown
# Discovery: [Project Name]

## Desired Outcome
[One clear outcome statement]
**Metric:** [How we'll measure it]
**Timeframe:** [When we expect to see movement]

---

## Opportunity Solution Tree

### [O1] Opportunity title
**Evidence:** assumed | observed | validated
**Source:** [Research session, data pull, stakeholder interview, etc.]
**Why it moves the outcome:** [One sentence connecting this opportunity to the desired outcome]

#### [S1.1] Solution title
**Hypothesis:** If we [do X], [users will Y], because [Z]
**Confidence:** low | medium | high

##### [E1.1.1] Experiment title
**Method:** [How we'll test it — prototype / fake door / wizard of oz / A/B / etc.]
**Success threshold:** [What result means we proceed]
**Effort:** [hours / days]
**Status:** not started | running | passed | failed | inconclusive
**Result:** [What we learned — fill in after running]

#### [S1.2] Solution title
...

### [O2] Opportunity title
...

---

## Parking Lot
*Solutions and ideas that don't yet have a linked opportunity. Each item should be placed or discarded — not left here indefinitely.*

- [Idea] — [Why it was parked]

---

## Decision Log
| Date | Decision | Rationale |
|------|----------|-----------|
```

---

## Behaviour

### First invocation (no existing DISCOVERY.md)

**Step 1 — Check for existing context.**
Ask: do you already have a defined outcome, or are we starting from zero? If a Situational Map from `discovery-guide` exists for this initiative, use it — it already captures the outcome, evidence base, and key unknowns. If they have an outcome from another source, use it. If not, redirect to `outcome-framing` before proceeding.

**Step 2 — Confirm the outcome.** You need a solid outcome statement before the tree can be built. Do not construct one here — use `outcome-framing` for that.

Ask: *"Do you have an outcome statement already — a specific change in user behaviour or business health you're working toward? If not, use `outcome-framing` first and bring the result back here."*

If they have one, validate it passes the basic test: it names who changes, what they do differently, and why that matters. If it doesn't pass, redirect to `outcome-framing` rather than attempting a quick fix. A compromised outcome at the root of the tree contaminates every branch below it.

**Step 3 — Seed the opportunities.**
Ask: "What do you already know — or believe — about why users aren't achieving this outcome?" Accept research findings, observations, assumptions, hunches. Classify each: is it evidence or assumption? Place them as opportunities on the tree, noting evidence level for each.

**Step 4 — Handle early solutions.**
If the user offers solutions before opportunities are established: park them in the Parking Lot. Name it explicitly: *"I've parked that in the Parking Lot — it's a solution, and solutions need to be attached to an opportunity. Let's find the underlying need it addresses."* Do not skip this step to be accommodating.

**Step 5 — Write DISCOVERY.md.**
State clearly when delivering it: *"This is version 1 — it's incomplete by design. The tree grows as you discover."*

---

### Update invocation (DISCOVERY.md exists)

**Step 1 — Read and summarise the current tree.**
Before accepting any new input, show the user where things stand: outcome, number of opportunities, which branches have solutions, which experiments are running or stale.

**Step 2 — Accept new inputs.**
Ask what's changed: new research findings? A new idea? An experiment result?

**Step 3 — Place each input correctly:**
- New research finding → new opportunity (assign evidence level, link to outcome)
- New idea or proposal → solution under the relevant opportunity, or Parking Lot if no clear opportunity
- Experiment result → update status, extract the learning in one sentence

**Step 4 — Surface structural problems.** Flag any of these:
- Opportunities with no solutions (unexplored branches — are they being ignored?)
- Solutions with no experiments (stalled — what's blocking a test?)
- Experiments marked `running` but not updated in the last session (stale — did this actually run?)
- Parking Lot growing larger than the tree itself (signal: the team is still in solution-first mode)

**Step 5 — Write the updated DISCOVERY.md.**

---

## Enforcement rules

These are not negotiable. The skill's value comes from holding these lines.

**No floating solutions.**
Every solution must sit under an opportunity. If someone insists a solution has no opportunity, ask: "What customer need or friction does this address?" Keep asking until the opportunity emerges — then place the solution there.

**No solutions disguised as opportunities.**
Challenge any "opportunity" that contains product language ("users need a better X," "we should add Y"). Reframe it: "What is the underlying need or friction that makes users want X?" The opportunity is always one level more abstract than the solution.

**One outcome per tree.**
If someone tries to load two outcomes onto one tree, name the tension and ask them to choose a focus. Offer to open a second tree for the other outcome. A team that can't name a single outcome doesn't have a product strategy — it has a list.

**Evidence levels are mandatory.**
Every opportunity must be tagged `assumed`, `observed`, or `validated`. An untagged opportunity is an invisible assumption. This single discipline is what separates a tree that reveals thinking from a tree that conceals it.

---

## Opportunity Prioritisation

When the tree has 3 or more opportunities and the team needs to decide which to pursue first, run this protocol. Do not run it on a tree with only 1–2 opportunities — prioritisation requires a genuine choice.

**Trigger:** *"We have several opportunities — which should we go after first?"* or when an Update invocation surfaces multiple unexplored branches and the team needs focus.

### Scoring

Score each opportunity across four dimensions. Generate your best assessment, then ask the user to review and adjust — do not fill the table silently and present it as settled.

| Opportunity | Reach | Impact | Confidence | Ease | Priority score |
|---|---|---|---|---|---|
| [O1] | | | | | |
| [O2] | | | | | |

**Dimension definitions:**

- **Reach (1–5):** How many users in the target segment experience this opportunity? 1 = narrow edge case, 5 = nearly all users in scope.
- **Impact (1–5):** If this opportunity were fully addressed, how much would the desired outcome move? 1 = marginal, 5 = significant and direct.
- **Confidence (1–5):** How well evidenced is this opportunity? Use the evidence level on the node: `assumed` → 1–2, `observed` → 3, `validated` → 4–5.
- **Ease (1–5):** How tractable is this opportunity — how feasible is it to generate and test solutions here? 1 = deeply constrained or cross-cutting, 5 = relatively straightforward to explore.

**Priority score:** `(Reach × Impact × Confidence) / (6 − Ease)`

The formula is a thinking tool, not an oracle. After scoring, ask:

*"Does anything feel wrong about this ranking? Any opportunity the score placed too high because it's comfortable to work on — or too low because it feels risky or ambitious?"*

Flag specifically: an opportunity with high Reach and Impact but low Confidence is **not** a reason to deprioritise it. It may be the highest-value thing to research next. Low confidence is a reason to investigate, not a reason to park.

### Prioritisation output

After scoring and gut-check, produce a recommendation:

```
## Opportunity Prioritisation

**Focus opportunity: [O1] [Title]**
Score: [X] | Evidence: [assumed / observed / validated]

**Rationale:** [2–3 sentences: why this opportunity, why now,
what makes it the right first bet given the outcome and what the team already knows]

**What this means for the other opportunities:**
- [O2]: [One sentence — park, research in parallel, or revisit after O1]
- [O3]: [same]

**What would change this recommendation:**
[The specific finding or signal that would make a different opportunity the right first bet]
```

After delivering, flag any opportunities with high Confidence but no Solution branches — validated needs with no solutions being explored are the most common strategic blind spot in a mature tree.

---

## Tone and posture

This skill is allowed to push back.

When the user is doing solution-first thinking, name it plainly and redirect. When an "opportunity" is a solution in disguise, say so and reframe. When the Parking Lot is growing, note what it signals about how the team is working.

The goal is not to fill in a template. The goal is to make visible the quality of the team's discovery thinking — including the gaps, the assumptions, and the leaps. A well-maintained OST makes wishful thinking impossible to hide.

---

## Reference

For risk type definitions, see `assumption-mapping`. For the full bundle routing map, see `discovery-guide`.
