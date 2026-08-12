# Outcome Framing

## When to use this skill

Use when someone wants to define what success looks like for a product initiative, feature, or discovery effort.

**Explicit triggers (English):**
- "Define success metrics"
- "Help me write OKRs"
- "What does good look like for this?"
- "How do we measure this?"
- "What should our north star metric be?"
- "How will we know if this worked?"

**Explicit triggers (Norwegian):**
- "Definer suksessmålinger" / "Hva er suksesskriteriene?"
- "Hjelp meg å skrive OKR-er" / "Hjelp meg med OKR-ene"
- "Hva er et godt resultat?" / "Hva ser bra ut her?"
- "Hvordan måler vi dette?" / "Hva bør vi måle?"
- "Hva bør nordstjernemålet vårt være?"
- "Hvordan vet vi om dette virket?" / "Hvordan vet vi om det fungerte?"
- "Hjelp meg med målsetting" / "Hva er KPI-ene våre?"
- "Hva er målet med dette?" / "Definer målene"
- "Hva vil suksess se ut som?" / "Hva betyr suksess her?"

Note: Norwegian product teams commonly mix English and Norwegian — also respond to hybrid phrases like *"hjelp meg med OKRs"*, *"hva er north star-en vår?"*, or *"kan du hjelpe med metrics?"*

**Implicit triggers — invoke proactively when:**
- Someone states a goal in output terms ("we want to ship X by Q3" / "vi skal lansere X innen Q3")
- Someone offers a vanity metric as a success definition ("success is 10,000 signups" / "suksess er 10 000 registreringer")
- Someone is about to start discovery or ideation without a defined outcome
- Someone says "vi skal levere X" (we're going to deliver X) without naming what should change as a result

---

## Core philosophy

This skill holds three principles as non-negotiable.

**1. An outcome is a behavior change, not a delivery**
Shipping a feature is not an outcome. Usage is not an outcome. An outcome is: *a specific person does a specific thing more, less, or differently — and that change creates value.* If you can't name who changes and what they do differently, you don't have an outcome.

**2. Outcomes must connect upward**
A team measuring the right thing in isolation can still be working against company goals. Every team-level outcome lives in a hierarchy: behavior change → product outcome → business result → company strategy. A metric with no upward connection is a vanity metric in disguise.

**3. Key Results must be outcomes, not outputs**
*(OKR discipline)*
"Launch X" is not a Key Result. "Complete the redesign" is not a Key Result. "X% of users do Y by date Z" is a Key Result. Any KR that could appear on a project plan rather than a scoreboard is an output.

---

## The challenge posture

Before helping someone *write* an outcome, challenge what they think they already have. This is the most important part of the skill. Be direct — name exactly what is wrong with a proposed metric. Do not soften it.

### Vanity metric red flags

| What they say | What to challenge |
|---|---|
| "Success is X users / downloads / signups" | Raw counts — compared to what baseline? What do those users need to *do* after that point? |
| "Success is high engagement / time on site" | Engagement doing what? High time-on-site can mean confusion, not value. |
| "Success is we shipped the feature by Q3" | That's an output. What changes in the world because of it? |
| "Success is good NPS / satisfaction scores" | Satisfaction with what behavior? What specifically drives the score up? |
| "Success is revenue growth" | Too lagging and too broad for a team-level outcome. What behavior change by which users creates that revenue? |
| "Success is X% increase in engagement" | Engagement with what? Measured how? An increase toward what end? |

### The three challenge questions — ask these in sequence

1. **WHO changes?** Which specific users, customers, or stakeholders behave differently?
2. **WHAT do they do differently?** What action, decision, or frequency shifts?
3. **WHY does that matter?** What business or customer value does that behavior change create?

If the answer to any of these is vague, keep pushing. A good outcome survives all three questions with specificity.

---

## Phase 1: Intake

Gather context through conversation — do not present these as a questionnaire.

> **Carrying context forward:** If a Situational Map from `discovery-guide` exists for this initiative, open with: *"I can see from your Situational Map that [key finding]. Is that still current?"* — then proceed from the relevant point rather than re-running the full intake. Do not re-ask questions already answered in the map.

- What's the initiative, product area, or problem?
- What does the team currently say success looks like?
- What's the business context — what goal does this connect to at the company level?
- Who are the primary users this affects?
- What timeframe are you working within?
- Is there an existing OKR structure to connect to?

---

## Phase 2: Challenge

Apply the challenge posture to whatever success definition they bring.

**Examples of the challenge in action:**

> *User: "Success is 10,000 new users signing up."*
> Challenge: "That's a count, not an outcome. What do those 10,000 users need to do after signing up? What behavior are you trying to produce — and what makes 10,000 the right number? Is that tied to a revenue model, a retention curve, something else?"

> *User: "Success is that we launch the onboarding redesign by Q3."*
> Challenge: "That's an output — shipping the redesign. What should change for users as a result? What's the behavior you're trying to produce, and how will you know the redesign produced it rather than something else?"

> *User: "Success is improving customer satisfaction."*
> Challenge: "Satisfaction is a result, not an action. What do you want customers to *do* differently that would make them more satisfied? And how are you measuring satisfaction — NPS, CSAT, renewal rate, something else?"

> *User: "Success is increasing DAU."*
> Challenge: "Doing what? DAU counts heads — it doesn't tell you whether users are getting value. What core action should those active users be completing? What does a good active day look like for them?"

---

## Phase 3: Outcome Construction

Once the behavior change is clear, build the full outcome package.

### The outcome statement

Format: *[User segment] will [do specific behavior] at [frequency or magnitude] by [timeframe], because [underlying motivation or need they have].*

**Example:**
*New users on the professional plan will complete their first core workflow within 7 days of signup, at a rate of 60%+, because they need early evidence of value to justify continued use.*

Note what this statement does: it names *who*, *what they do*, *how much*, *when*, and *why they would do it*. A statement that cannot be written in this format is not ready.

---

### Metrics framework

**Primary outcome metric**
The single most direct measure of the behavior change. Time-bound. Specific enough to be unambiguous. There should be exactly one — if a team has five "primary metrics," they have none.

**Leading indicators (2–3)**
Early signals that the outcome is on track, visible before the lagging outcome confirms it. These are the team's week-to-week compass.
- Activation events (first meaningful action)
- Feature adoption milestones
- Early retention signals (Day 3, Day 7 return)
- Support deflection rates

**Lagging indicators (1–2)**
Proof the outcome actually happened — visible after the fact, often weeks or months later.
- Retention at 30/60/90 days
- Conversion from trial to paid
- Revenue impact from cohort
- Churn reduction

**Guardrail metrics (1–3)**
What must NOT be damaged in pursuit of this outcome. These define the boundaries of acceptable tradeoff. Guardrails are as important as the primary metric — they prevent local optimization that damages the broader system.

Examples:
- Support ticket volume must stay below X
- NPS must not drop below Y
- Activation rate for adjacent user segments must not fall
- Revenue from existing customers must not be cannibalized

---

### Strategy connection

Map the outcome to the broader hierarchy:

```
Company goal:         [name the business objective this serves]
  └── Product pillar: [which area of product strategy]
       └── Outcome:   [the outcome statement]
            └── OKR:  [Objective + Key Results, if applicable]
```

If the outcome cannot be connected to a company goal, that is a signal — not a formatting problem. Raise it.

---

## Phase 4: OKR drafting (if requested)

### Objective
- Qualitative, directional, motivating
- Answers: *what are we trying to achieve, and why does it matter?*
- Should be memorable — a team should be able to say it without looking it up
- Does NOT contain a number (numbers belong in Key Results)

### Key Results (2–5 per objective)
Each must be:
- An outcome, not an output
- Measurable and falsifiable — you can look at a number and say pass/fail
- Time-bound
- Owned by the team (not dependent entirely on external factors)

A strong set of KRs includes:
- At least one leading indicator (early signal)
- At least one lagging indicator (proof)
- At least one guardrail KR if the work carries real risk to adjacent outcomes

### Anti-patterns — reject these explicitly

| Pattern | Why it fails |
|---|---|
| "Launch X" | Output — describes a delivery, not a result |
| "Improve X" | Not measurable — improve by how much, from what baseline? |
| "Explore / investigate X" | Activity, not outcome |
| "Deliver X to Y teams" | Output and internal-facing |
| "X% increase in engagement" | Engagement with what? Toward what end? |
| "Complete X research" | Output — what does the research need to *reveal or change*? |

---

## Output format

Deliver the outcome package in this structure:

---

### Outcome Package: [Initiative Name]

**Outcome statement**
[Formatted outcome statement — who / what / how much / when / why]

**Primary metric**
[Name] — [definition] — [target] — [timeframe]

**Leading indicators**
- [Indicator]: [what it measures] / [target or direction]
- [Indicator]: [what it measures] / [target or direction]

**Lagging indicators**
- [Indicator]: [what it measures] / [expected timeframe to see signal]

**Guardrail metrics**
- [Metric]: must stay [above/below] [threshold]

**Strategy connection**
- Company goal: [name]
- Product strategy pillar: [name]
- OKR: [Objective, if applicable]

**What we're NOT measuring here — and why**
[List 1–2 metrics the team might expect to see, and briefly explain why they were excluded — outputs, vanity metrics, wrong level of specificity, or belonging to another team. This section prevents the outcome package from being silently re-expanded later.]

---

## Sanity check — run this before delivering

Ask these four questions before finalizing any outcome package:

1. **Could this metric improve even if users are failing?** If yes — vanity metric. Reconsider.
2. **Could a different team's work move this metric significantly without you?** If yes — too high-level or wrong attribution. Tighten it.
3. **Is there a scenario where you hit this metric and the intended business outcome still doesn't follow?** If yes — the connection to strategy is broken. Fix it.
4. **Would a reasonable person look at this metric in 6 months and agree it proved the outcome happened?** If not — it's a proxy at best. Name what it's a proxy for.

---

## Related skills

For the full bundle routing map, see `discovery-guide`.
