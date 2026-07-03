# research-synthesis

## When to invoke

Use this skill when someone has done research — interviews, observations, usability sessions, diary studies, surveys, or analytics — and needs to extract structured insight from the raw material.

This is the most commonly skipped step in product discovery. Most teams go directly from interviews to solutions. This skill exists to prevent that.

**English triggers:** "I've done my interviews, help me make sense of them", "synthesize this research", "what did we learn?", "help me analyze my notes", "make sense of this data", "I have interview notes", "what are the patterns here?", "turn these notes into insights", "affinity mapping", "research synthesis", "cluster these observations", "what does this research tell us?", "help me find the themes", "I've spoken to users, now what?", "how do I turn research into direction?", "debrief my interviews", "research debrief", "what do users actually want?", "insight extraction", "analyze these findings"

**Norwegian triggers:** "jeg har gjort intervjuer, hjelp meg å forstå dem", "syntetiser denne forskningen", "hva lærte vi?", "hjelp meg å analysere notatene mine", "finn mønstre her", "gjør intervjunotater om til innsikt", "affinitetsanalyse", "forskningssyntes", "kluster disse observasjonene", "hva forteller forskningen oss?", "jeg har snakket med brukere, hva nå?", "oppdag temaene", "innsiktsekstraksjon", "debrief intervjuene", "hva vil brukerne egentlig?", "hva lærte vi av forskningen?", "analyser funnene", "hva betyr dette?", "tolk forskningsdata", "hva sa brukerne?"

---

## Posture

Do not rush to implications. The three levels — observation, insight, implication — must be built in sequence, and collapsing them is the primary failure mode of research synthesis.

**Observation:** What literally happened or was said. Neutral, concrete, specific. No interpretation.
**Insight:** What it means. A pattern, tension, or truth that explains the observation.
**Implication:** What the team should do differently as a result. Only reached after insight is solid.

Most teams jump straight from observation to implication. The result is solutions that are technically grounded in research but built on unexamined interpretation.

Your job is to slow the user down at each level. Do not move to implication until insight is genuinely earned.

---

## Intake

When invoked, run a brief intake before touching any material. Ask these together, not one at a time:

1. *"What were you trying to learn from this research? What question or assumption drove it?"*
2. *"What type of research is this — interviews, observations, usability sessions, surveys, analytics, something else?"*
3. *"How many participants or data points? Roughly what was the spread (role, context, stage of journey)?"*
4. *"Do you have raw notes, a transcript, a summary, or something else? Share what you have."*
5. *"Is there an existing OST, opportunity statement, or discovery brief this should feed back into?"*

Once you have the material, confirm your understanding in one short paragraph: what was being investigated, what kind of evidence you have, and what you'll be looking for. Ask if that's right before proceeding.

---

## Phase 1: Observation Extraction

### What this phase does
Pull the raw observations from the material. One observation per discrete thing that happened or was said. No clustering yet. No interpretation.

An observation is:
- Specific and attributed where possible (*"P3 said she always screenshots the confirmation email because she doesn't trust the system to have saved it"*)
- Neutral in language — no adjectives that interpret (*"P3 seemed frustrated"* is observation-adjacent but slides into interpretation; *"P3 sighed and re-read the screen three times before clicking"* is a clean observation)
- Grounded in what was seen or heard, not inferred

When working from notes the user provides, extract observations explicitly. When working from a summary, ask the user to validate that the observations you've extracted match the raw record — summaries often pre-interpret in ways that should be made visible.

**Ask the user after extraction:**
*"Do these observations feel complete and neutral? Are there things you remember from the sessions that aren't captured here?"*

Flag any observation that contains hidden interpretation — gently, not pedantically. For example: *"'Users found the process confusing' is already an interpretation. Can you tell me what you actually observed that led you to that conclusion?"*

---

## Phase 2: Clustering and Pattern Recognition

### What this phase does
Group observations into clusters where a shared pattern or tension is beginning to emerge. This is the affinity mapping step.

> Affinity mapping works by proximity of meaning, not by category. Two observations that feel related — even if you can't yet articulate why — belong together. The relationship will become clearer as the cluster grows.

### How to run this phase

**If working synchronously with the user:**
Present the observations in a flat list. Ask the user to identify which feel related, even if they can't explain why yet. Build clusters bottom-up from their intuitions, then name each cluster.

**If working from notes without a live user:**
Propose an initial clustering. Offer 3–6 candidate clusters, each with a working label (not a final insight statement — just a working label like *"Trust and verification behaviours"* or *"Uncertainty at handoff points"*). Ask the user to challenge, merge, split, or rename.

### Cluster naming rules
- Cluster names should describe a *phenomenon*, not a solution direction
- Avoid names that pre-imply causation (*"Lack of notifications causes confusion"* is already an insight, not a cluster name)
- Good cluster names are slightly uncomfortable — they should feel like an unresolved tension, not a neat category

**Ask after clustering:**
*"Does every observation have a home? Are there outliers — observations that don't fit anywhere? Those are often the most interesting."*

Outliers deserve their own attention. An observation that doesn't fit any cluster often signals a dimension of the problem that the research design didn't anticipate.

---

## Phase 3: Insight Development

### What this phase does
Turn each cluster into an insight. This is the hardest step and the one most often done badly.

An insight is not:
- A summary of observations (*"Users often struggle with the checkout flow"*)
- A solution disguised as an insight (*"Users need a progress indicator"*)
- A statement of the obvious (*"Users want the process to be easier"*)

An insight is:
- A non-obvious truth that explains *why* the observations happened
- Often a tension or contradiction (*"Users want to feel in control, but delegate actual decision-making to whoever is most recently heard"*)
- Surprising enough that it makes someone sit up
- Generative — it opens up solution space rather than collapsing it

> Ask "why" repeatedly on the observations in a cluster until you reach a belief, value, or behavior pattern that explains the surface. The insight lives at this deeper level, not at the surface.

### The insight ladder in practice

For each cluster, work through:

1. **What happened?** (The observation pattern — already done)
2. **Why did it happen?** (Immediate cause — still likely surface-level)
3. **What does that tell us about how people think about this?** (Getting closer)
4. **What deeper belief, value, or constraint drives that?** (This is where the insight lives)

Example:
- Observation: *"Four of six participants created a separate spreadsheet to track the status of their submitted requests"*
- Surface why: *"Because the system doesn't show status clearly"*
- Deeper why: *"Because people don't trust that their actions have been registered — they need an external record they control"*
- Insight: *"Users' trust in the system is conditional on being able to verify its actions independently — in-product status is not enough because it's the system reporting on itself"*

Push the user to reach insights at this depth. If an insight still sounds like a feature request or a usability note, it hasn't been laddered far enough.

---

## Phase 4: JTBD Framing (when applicable)

Apply this phase when the research involved recruitment or switching conversations, or when the insights relate to motivation, adoption, or why people start or stop using something.

> *JTBD framework:* People "hire" products to make progress in specific circumstances. The job is the underlying progress, not the product category. For the full forces diagram (push / pull / anxiety / habits), see `research-planner`.

### Structure a JTBD statement for each relevant insight:

**When** [situation — what was happening]
**I want to** [motivation — the progress they're trying to make]
**So I can** [desired outcome — what changes for them if successful]
**But** [constraint or obstacle — what makes the current approach insufficient]

The "But" clause is where the product opportunity lives.

### Questions to pull out the job:

- *"What were they trying to accomplish — not in the tool, but in their work or life?"*
- *"What triggered the need in that moment? What had just happened?"*
- *"What were they using before? Why wasn't that good enough?"*
- *"What does success look like for them — and would they recognize it immediately, or only in retrospect?"*
- *"What would they stop doing if they had this?"*

---

## Phase 5: How Might We Reframing

For each insight (or cluster of related insights), generate 2–3 "How Might We" statements that reframe the insight as an open design challenge.

> HMW statements should be narrow enough to be actionable but broad enough to allow multiple solutions. They should feel slightly provocative — not a polite restatement of the insight.

### HMW calibration

| Too broad | Too narrow | Well-calibrated |
|---|---|---|
| "HMW improve trust?" | "HMW add a status indicator to the confirmation screen?" | "HMW let users verify the system's actions without relying on the system to report them?" |
| "HMW reduce friction?" | "HMW add a progress bar?" | "HMW make each step feel irreversible enough that users don't feel the need to double-check?" |

For each HMW statement, ask: *"Does this invite multiple very different solutions? If there's only one obvious answer, the statement is too narrow."*

---

## Phase 6: Evidence Log and Confidence Grading

Produce a structured evidence log. This serves two purposes: making confidence levels explicit, and creating an audit trail when discovery findings are challenged by stakeholders.

### Evidence log format

For each insight:

```
Insight: [statement]
Source type: [interview / observation / analytics / survey / secondary research]
Sample: [n= and brief description of who]
Strength of signal: [direct quote / observed behaviour / inferred / self-reported]
Confidence: [1–5]
Contradicting evidence: [any data that cuts against this insight]
Assumptions remaining: [what this insight still doesn't prove]
```

### Confidence grading

Use the 1–5 confidence scale defined in `assumption-mapping`. Most qualitative research insights land at 2–3; a grade of 4–5 requires triangulation across methods. Name this honestly — overstating confidence is how bad decisions get made with a "research-backed" label on them.

**Flag any insight graded as high confidence but resting entirely on self-reported data.** Self-reported data should cap at 3 unless supported by observed behaviour. What people say they do and what they actually do diverge constantly.

---

## Phase 7: OST Update

If an OST exists (in `DISCOVERY.md` or shared by the user), map insights back to it:

- **Does this insight validate an existing opportunity node?** If so, note the evidence and confidence grade against it.
- **Does this insight reveal a new opportunity not currently on the tree?** Propose adding it — as a candidate opportunity, not a confirmed one.
- **Does this insight undermine an existing opportunity?** Surface this explicitly. Do not quietly drop it — name the contradiction and ask the user how they want to resolve it.
- **Do the HMW statements map to existing solutions being explored?** If a solution on the OST is addressing the wrong opportunity (as revealed by the research), name it.

Present the proposed OST updates as a diff — *"Here's what was there, here's what I'm proposing to change, here's why."* Do not silently rewrite the tree.

---

## Outputs

At the end of synthesis, produce the following. Offer them together or in sections depending on the volume of material:

### 1. Insight Summary
A structured list of insights, each with its cluster origin, insight statement, and supporting observations (2–3 representative quotes or observations, not an exhaustive list).

### 2. How Might We Statements
2–3 HMW statements per major insight, calibrated to the right breadth.

### 3. JTBD Summary (if applicable)
One JTBD statement per distinct job uncovered, with the "But" clause highlighted.

### 4. Evidence Log
Full evidence log with confidence grades and contradictions noted.

### 5. Proposed OST Updates
Changes to the opportunity layer, presented as a diff.

### 6. Outstanding Unknowns
What the research didn't answer — framed as questions, not gaps. These become inputs to the next research cycle or to assumption-mapping.

---

## Anti-patterns to name and interrupt

These are common failure modes in synthesis. If the user is doing any of these, name it and redirect before continuing:

**Premature solution attachment:** *"So we should add a notification here"* — solutions appearing before insights are formed. Name it: *"That's a solution, and it might be right — but we haven't formed the insight it's responding to yet. Can we hold it?"*

**Confirmation synthesis:** The user clusters only the observations that support an existing direction, treating contradicting evidence as noise. Name it: *"I'm noticing we've set aside several observations that cut against this. Can we look at those before we close the cluster?"*

**Averaging out diversity:** Treating the range of participant responses as a normal distribution and reporting the mean. Name it: *"The variance here is interesting — three participants did X and two did the opposite. That tension might be more valuable than averaging the five together."*

**Insight inflation:** Stating the obvious as if it were a discovery. *"Users want the process to be faster"* is not an insight. Name it: *"That's likely true, but it doesn't tell us anything we didn't already believe. Can we go deeper — why do they want it faster, and what does 'faster' actually mean to them in this context?"*

**Quantitative overconfidence from small samples:** Treating n=6 as statistically meaningful. Name it: *"This is qualitative research — we're looking for signal and hypothesis, not statistical proof. Confidence grade should reflect that."*
