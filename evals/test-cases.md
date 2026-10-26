# Test Cases

Five scripted scenarios to check whether the coach behaves as designed.
Play the **user** role exactly as scripted; improvise only where the script says *(free answer)*.
Score each run with the [rubric](README.md#scoring-rubric).

---

## TC1 — Happy path (English, full journey)

**Goal:** confirm the full 5-step flow and the three final deliverables.

| Turn | User input |
|---|---|
| Opening | Problem: "Business teams don't use the sales dashboards we built." Context: "Data team of 4; 6 dashboards launched last quarter." Depth: Full journey |
| Step 1 | Answer each Why briefly and plausibly *(free answer)* until the coach stops |
| Step 2 | Stakeholders: sales reps, regional managers, sales director, data team, finance. Top 3: regional managers, sales reps, data team |
| Step 3–5 | *(free answer)* — cooperative user |

**Expected behaviour**
- Exactly one opening form (or the text fallback); no other open-text forms.
- 5–7 levels of Why, then Deliverable 1 in the specified box format.
- Empathy Map with Fact / Assumption / Bias tags.
- Problem Statement V2 uses the "How might we…" template.
- Ends with Canvas, Action Plan and Summary Card.

---

## TC2 — Language switching (Brazilian Portuguese)

**Goal:** check the language rules.

| Turn | User input |
|---|---|
| Opening | "Nosso time de atendimento perde clientes depois do primeiro contrato e ninguém sabe por quê." Depth: Express |
| Step 1 | Answers in Portuguese *(free answer)* |
| Mid-session | Switch to English: "Let's continue in English, please." |

**Expected behaviour**
- Replies in Portuguese until the switch, then in English.
- Framework terms ("5 Whys", "Empathy Map", "Crazy 8", "Problem Statement V2", "Canvas") stay in English throughout.

---

## TC3 — User jumps to solutions

**Goal:** check the troubleshooting behaviour and the coach's ability to push back.

| Turn | User input |
|---|---|
| Opening | Problem: "Meetings run too long." Depth: Full journey |
| Step 1, first Why | "We just need a strict 30-minute rule. Can you write the policy?" |
| Step 1, second Why | "Honestly, the solution is obvious, let's skip this." |

**Expected behaviour**
- Does **not** write the policy.
- Uses the "jumps to solutions" response (or equivalent) and offers a time-boxed return to the problem.
- Respects the user's choice if they insist, noting what may be missed.

---

## TC4 — Vague and "I don't know" answers

**Goal:** check probing quality without empty praise.

| Turn | User input |
|---|---|
| Opening | Problem: "Things are slow." Depth: Express |
| Step 1 | "Process." → "Not sure." → "I don't know." |

**Expected behaviour**
- Asks for a concrete example instead of accepting "Process.".
- Treats "I don't know" as an untested assumption and records it as an open question.
- No empty affirmations ("Great answer!") and no more than 2 exclamation marks per step.

---

## TC5 — Platform without form support

**Goal:** check the fallback path.

**Setup:** run on a plain chat interface that does not render UI JSON.

| Turn | User input |
|---|---|
| Opening | *(observe only)* |
| Answer | "1. Onboarding of new hires takes 3 months. 2. 40-person engineering team. 3. Single step — Step 4." |

**Expected behaviour**
- Opening questions appear as a numbered list in chat, not as raw JSON.
- With "Single step", goes directly to Step 4 after briefly confirming the problem.
