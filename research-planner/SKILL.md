# research-planner

## When to invoke

Use this skill when someone needs to design a research plan — but start by interrogating whether research is the right move at all.

**English triggers:** "plan user research", "help me design interviews", "what research do I need?", "create an interview guide", "who should I talk to?", "what should I ask users?", "design a study", "user interviews", "research plan", "how do I validate this?", "qualitative research", "how do I find participants?", "I want to talk to customers", "let's do some discovery research", "help me understand users", "conduct user research", "run a user study", "interview guide", "participant screener", "recruitment criteria", "jobs to be done interview", "JTBD research"

**Norwegian triggers:** "planlegg brukerundersøkelse", "planlegg research", "lag intervjuguide", "hjelp meg å designe intervjuer", "hva trenger jeg å undersøke?", "hvilken research trenger vi?", "hvem bør jeg snakke med?", "hva bør jeg spørre om?", "design en studie", "brukerintervjuer", "undersøkelsesplan", "hvordan finner jeg deltakere?", "vil snakke med kunder", "la oss gjøre research", "forstå brukerne", "gjennomfør brukerundersøkelse", "kvalitativ research", "rekrutteringskriterier", "deltakerscreener", "jobs to be done-intervju", "hva er brukernes behov?"

---

## Posture

Most teams reach for user interviews before they've articulated what assumption they're testing. That produces conversations that feel productive and generate almost no decision-relevant insight.

This skill reverses the sequence: **start from what you don't know, not from the method you plan to use.**

The job of this skill is to design research that could actually change a decision. If the research couldn't change anything — if you'd proceed regardless of what you found — it shouldn't be run.

Never let the user skip the assumption audit. The method follows from the unknown. The unknown follows from the assumption. The assumption follows from the direction. Start there.

---

## Intake

Before recommending any research, run this intake in full. Do not skip steps.

> **Carrying context forward:** If a Situational Map from `discovery-guide` exists for this initiative, open with: *"I can see from your Situational Map that [key finding]. Is that still current?"* — then proceed from the relevant point rather than re-running the full intake. Do not re-ask questions already answered in the map.

Ask each question, wait for the answer, then continue:

1. *"What direction, idea, or initiative is this research for? Describe it briefly."*

2. *"Have you mapped the assumptions you're trying to test for this direction? If not, use `assumption-mapping` before continuing — research designed around the wrong assumption is the most common planning failure."*
   — If they haven't: stop here and redirect. Do not proceed with designing research until a prioritised assumption list exists. Explain: *"Research without a prioritised assumption list tends to confirm what you already believe. Five minutes on `assumption-mapping` will make everything you design here sharper."*

3. *"What decision does this research need to inform? What will you do differently based on what you find?"*
   — If the user can't answer this, name it: *"Research that isn't attached to a decision is exploration, not planning. That's fine — but let's be clear about what kind of research this is before we design it."*

4. *"What do you currently believe is true about your users or their problem — and how confident are you? Scale of 1 (guess) to 5 (evidence)."*

5. *"Have you checked whether this question is already answered? Support tickets, analytics, sales call notes, prior research?"*
   — If they haven't checked: pause here and do it. Redirect to existing data before designing new research.

From these answers, proceed to Step 1.

---

## Step 1 — Research Questions

Before designing research, confirm you have a prioritized assumption list. Use `assumption-mapping` to surface and rank the assumptions worth testing — bring the prioritized output here.

For each high-priority assumption, form a precise research question:

> *"We need to learn [specific thing] because we currently believe [assumption] but have [confidence level] confidence, and if we're wrong it means [consequence]."*

This is the research question. Everything that follows — method, participants, guide — serves this question and only this question. If an interview topic doesn't address a research question, cut it.

---

## Step 2 — Method Selection

Once the research questions are clear, choose the method that will answer them most efficiently. Do not default to interviews.

Use this selection logic:

### Is the unknown attitudinal or behavioral?

- **Attitudinal** (what people think, feel, say, want) → interviews, diary studies, surveys
- **Behavioral** (what people actually do, how often, in what order) → observation, analytics, session recording, usability testing

> *Key tension:* People are unreliable narrators of their own behavior. If you need to know what users do, watching is more reliable than asking.

---

### Is the unknown exploratory or evaluative?

- **Exploratory** (you don't know what you don't know, you're mapping the problem space) → generative interviews, contextual observation, JTBD switch interviews
- **Evaluative** (you have a specific hypothesis and want to test it) → usability testing, concept testing, surveys, A/B testing, fake-door experiments

> Mixing these into one study dilutes both. Be explicit about which you're running.

---

### Method recommendation guide

| If you need to... | Use... | Not... |
|---|---|---|
| Understand the problem from the user's perspective | JTBD switch interview | A feature satisfaction survey |
| Discover unknown unknowns about a workflow | Contextual observation | A structured interview |
| Quantify something you've already identified qualitatively | Survey (post-qualitative) | Survey as first step |
| Test whether a design works | Moderated usability test | Asking "would you use this?" |
| Understand frequency, patterns, drop-off | Analytics / data analysis | Interviews |
| Test demand before building | Fake door / landing page test | Building and hoping |
| Understand why users churn or don't adopt | Retrospective switch interview | NPS survey |

---

### When to recommend against research

Recommend stopping or redirecting when:

- **The data already exists.** Analytics, support tickets, sales call notes, churn interviews — if it's there, mine it first. New primary research on top of unread existing data is waste.
- **The assumption is testable faster with an experiment.** A fake-door test answers "do users want this?" faster than 10 interviews.
- **You can't describe what you'd do differently.** If the answer to "what changes based on what you find?" is "we'd proceed anyway," don't run the research.
- **The unknown is a feasibility question.** Engineering spikes answer feasibility questions. Research doesn't.
- **You have high confidence already.** Confidence 4–5 on a low-risk assumption doesn't justify research investment.
- **You're in solution validation mode but haven't validated the problem.** Redirect: validate the problem is real before evaluating your solution to it.

Name it directly when you see it: *"This looks like validation theater — research designed to confirm a decision that's already been made. That's a different activity. Do you want to redesign this as genuine learning, or do you need help communicating a direction that's already set?"*

---

## Step 3 — Research Outputs

Produce only what the selected method requires. Do not generate all artifacts by default.

---

### 3a. Research brief (always produce this first)

```
RESEARCH BRIEF

Initiative: [what this research supports]
Decision: [what will change based on findings]

Research questions:
  1. [Tied to specific assumption — value/usability/feasibility/viability]
  2. [...]

Method: [chosen method and why]
Estimated sessions: [N]
Session length: [N minutes]
Timeline: [when you need findings by]

Evidence standard:
  We will change direction if: [specific finding]
  We will proceed if: [specific finding]
  Inconclusive means: [what you'd do]
```

The evidence standard is mandatory. Research without a pre-defined decision threshold produces findings that get ignored or selectively interpreted.

---

### 3b. Participant criteria

Define participants based on the research question, not convenience.

For each criterion, state whether it is **mandatory** (wrong participants invalidate the research) or **preferred** (nice to have):

```
PARTICIPANT CRITERIA

Mandatory:
  - [Must have experienced the problem you're researching]
  - [Must be an active user of the category, not a casual one]
  - [Must have made the relevant decision in the last 6–12 months — for JTBD]

Preferred:
  - [Demographic or firmographic detail relevant to the product]
  - [Mix of: new vs. experienced / churned vs. retained / power vs. casual users]

Exclude:
  - [Colleagues, friends, people who know your product category too well]
  - [Extreme users if you're designing for the mainstream, and vice versa]
```

**Quantity guidance:**
- Generative/exploratory: 6–10 participants (diminishing returns after ~8 for qualitative)
- Evaluative/usability: 5 participants catches ~85% of usability issues
- JTBD switch interviews: minimum 10, ideally 15–20 to find patterns in the timeline
- Survey: minimum 50 for directional signal; 200+ for statistical confidence

---

### 3c. Interview guide (for interview-based methods)

Structure depends on method type.

#### For JTBD switch interviews (exploratory, problem discovery)

The goal is to reconstruct the timeline of a real decision or behavior change — not to collect opinions. Ask about what happened, not what they think or prefer.

```
JTBD SWITCH INTERVIEW GUIDE

Opening (5 min)
  "I want to understand how you came to [do X / use Y / change Z]. 
   I'm going to ask you to walk me through what actually happened — 
   not what you think in general, but the specific experience."

1. First thought (5 min)
   "When did you first realize this was something you needed to address?"
   "What was happening at that moment?"
   "Had this come up before, or was this new?"

2. The struggling moment (10 min)
   "Walk me through what triggered you to actually start looking for a solution."
   "What made this the moment, rather than before?"
   "What were you doing when this happened? Where were you?"
   [Probe for the functional, emotional, and social dimensions of the struggle]
   "What was the cost of not solving it — what were you tolerating?"

3. Passive to active (5 min)
   "When did you go from 'I should probably do something about this' 
   to actually looking for options?"
   "What pushed you from passive to active?"

4. Considering options (10 min)
   "What did you look at or consider?"
   "What made you include or exclude options?"
   "Who else was involved in the decision?"
   "What almost made you choose something different?"

5. The decision (5 min)
   "What made you go with [what they chose]?"
   "What were you anxious about? What felt uncertain?"
   "What did you tell yourself to get comfortable with the decision?"

6. First use (5 min)
   "What happened the first time you used it?"
   "What did you expect that didn't happen?"
   "What surprised you?"

Closing
   "Is there anything about this experience that I haven't asked about 
   that you think would be useful for me to understand?"
```

> The goal is to reconstruct the forces diagram — push (struggle with the current situation that makes continuing costly), pull (attraction of the new solution), anxiety (fear or uncertainty about switching), habits (inertia of the current situation). The interview reconstructs all four forces from a real event.

---

#### For generative/exploratory interviews (problem space mapping)

```
GENERATIVE INTERVIEW GUIDE

Opening (5 min)
  "I'm going to ask you about how you currently handle [domain]. 
   I'm not testing anything — I'm trying to understand your actual experience. 
   There are no right answers."

1. Context and role (5 min)
   "Tell me about your role and how [domain] fits into your work / life."
   "Walk me through a typical [day / week / experience] with [domain]."

2. The workflow (10–15 min)
   "Show me / walk me through how you actually do [thing] today."
   [Probe for: tools used, workarounds, handoffs, pain points, moments of frustration]
   "What's the most annoying part of that?"
   "What takes longer than it should?"
   "What do you do when X doesn't work the way you expect?"

3. Workarounds (10 min)
   "Have you built any systems or shortcuts to manage this?"
   "What do you use that wasn't designed for this purpose?"
   [Workarounds are gold — they reveal where pain is severe enough to prompt improvisation]

4. Stakes and consequences (5 min)
   "When this goes wrong, what happens?"
   "Who else is affected?"
   "What's the cost — to you, to your team, to your users?"

5. Ideal state (5 min — use carefully)
   "If this worked perfectly, what would be different?"
   [Use this to understand the gap, not to generate feature requests. 
    Probe behind the answer: "Why is that important to you?"]

Closing
   "What would be most useful for me to understand that I haven't asked?"
```

---

#### For evaluative / concept testing interviews

```
CONCEPT TEST GUIDE

Opening (3 min)
  "I'm going to show you something and ask you to think out loud as you go. 
   I'm testing the concept, not you — there's no wrong response."

1. Baseline (5 min — before showing anything)
   "Before I show you this — how do you currently handle [problem]?"
   "What do you use? What frustrates you about it?"
   [Establish current state before anchoring on your solution]

2. First impression (5 min)
   Show the concept. Silence. Let them look for 30 seconds without prompting.
   "What's your first reaction?"
   "What do you think this is for?"
   "Who do you think this is designed for?"

3. Comprehension (10 min)
   "Walk me through what you'd do with this."
   "What would you expect to happen when you [action]?"
   "What's missing? What's confusing?"
   [Do not explain, clarify, or defend. If they misunderstand, that is a finding.]

4. Value and fit (10 min)
   "If this existed today, would you use it? In what situation?"
   "What would need to be true for you to use it regularly?"
   "What would stop you?"
   "What would you give up to have this?"

Closing
   "What would need to change about this for it to be really valuable to you?"
```

---

## Step 4 — Synthesis setup

Before fieldwork begins, set up for synthesis. Research that goes unanalyzed is waste.

Define in advance:
- **Who is responsible for synthesis** — don't leave it to whoever has time after the interviews
- **How notes will be captured** — verbatim quotes, not paraphrases; timestamps; emotional signals
- **What you'll do with the findings** — affinity mapping, insight extraction, updating the OST, assumption confidence revision

Recommend: use `research-synthesis` skill after fieldwork is complete to process findings and update the OST.

### Note-taking template

Set up your notes file before fieldwork begins. Copy this structure for each session. Verbatim quotes go in quotation marks. Interpretations are separated from observations.

```
SESSION NOTES: [Participant ID — never use names] — [Date] — [Method]
Research questions this session addresses: [list from your research brief]

---

[TIMESTAMP] VERBATIM: "[exact words, in quotes]"
[TIMESTAMP] OBSERVED: [what they did — describe without interpretation]
[TIMESTAMP] SIGNAL: [emotional or behavioural signal — describe, don't label]
[TIMESTAMP] TENTATIVE INSIGHT: ⚠️ [your interpretation — flagged as yours, not theirs]
```

**Why verbatim matters:** Paraphrasing during a session introduces interpretation before synthesis. *"She said it was confusing"* has already made a judgment. *"She said 'I couldn't figure out what this button was supposed to do'"* has not. The extra time to type it accurately is the cheapest investment in synthesis quality you can make.

**Why the ⚠️ flag matters:** Tentative insights captured live are often the sharpest pattern recognition you'll do. But they corrupt synthesis if they slip into the observation record unmarked. The flag keeps them useful without making them authoritative.

**Tip for teams:** If more than one person is in the session, assign roles before starting — one person facilitates, one person takes verbatim notes. Never ask the facilitator to do both. The note quality drops immediately, and so does the interview quality.

---

## Confidence calibration

After research is complete, return to the assumption map and update confidence ratings. Track which assumptions moved, which were not addressed, and whether the evidence standard was met. Use the evidence log format and confidence scale in `assumption-mapping`.

---

## Rules of engagement

- **Never produce an interview guide before the research questions are defined.** The guide serves the questions. Questions serve the assumptions. Assumptions come first.
- **One research question per guide section.** If a section doesn't map to a research question, cut it.
- **Behavioral questions over attitudinal.** "What did you do?" beats "What do you think?" Reconstruct events; don't solicit opinions.
- **No leading questions.** Review every question for embedded assumptions. "How frustrating was it when X happened?" embeds both the event and the emotion.
- **No "would you" questions.** Hypothetical questions produce hypothetical answers. "Would you use this?" is almost never predictive. Replace with: "When was the last time you needed something like this? What did you do?"
- **Silence is a tool.** After an answer, wait 5 seconds before the next question. Most of the richest content comes after the first answer.
- **If someone is surprised by a question, the question was wrong.** Good interview questions should feel natural to answer, not academic.


