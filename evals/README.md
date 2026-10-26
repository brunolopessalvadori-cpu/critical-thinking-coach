# Evaluation Kit

How the Critical Thinking Coach prompt is evaluated — and how anyone can benchmark it
on their own model of choice.

The kit has two layers:

1. **Design review** (below) — a static audit of the prompt itself: for each quality
   criterion, does the prompt contain an explicit, testable rule that enforces it?
2. **Behavioural test cases** ([`test-cases.md`](test-cases.md)) — five scripted scenarios
   that adopters can run to check how a specific model follows those rules in practice.

> The design review evaluates the **prompt's specification**, not a model's output.
> Model behaviour can still drift; the test cases exist to measure that when needed.

## Scoring rubric

Ten criteria define what "good" looks like for this coach.

| # | Criterion | What "fully meets" looks like |
|---|---|---|
| R1 | Single form | One opening form (or numbered-list fallback); no other open-text forms |
| R2 | Language rules | Follows the user's language; framework terms stay in English |
| R3 | Root-cause depth | 5 Whys goes beyond symptoms and stops at an actionable layer |
| R4 | Pushback | Challenges solution-jumping and vague answers instead of accepting them |
| R5 | No empty praise | No hollow affirmations; ≤ 2 exclamation marks per step |
| R6 | Visual restructuring | Free-text answers are reformatted into the specified tables / boxes |
| R7 | Step deliverables | Each completed step ends with its deliverable in the specified format |
| R8 | Reframe quality | Problem Statement V2 follows the template and differs meaningfully from the original |
| R9 | Final canvases | Canvas, Action Plan and Summary Card delivered when the journey is completed |
| R10 | Observation vs. question | Turns mix observations and questions rather than only asking |

## Design review — v1.0.0

Coverage levels: **Explicit** = a specific, checkable rule exists · **Partial** = the intent
is stated but hard to verify or incomplete · **Missing** = no rule.

| # | Criterion | Where the prompt enforces it | Coverage | Residual risk |
|---|---|---|---|---|
| R1 | Single form | CRITICAL RULE: NO REPEATED FORMS + Fallback | Explicit | Low — fallback covers platforms that do not render forms |
| R2 | Language rules | LANGUAGE RULES (follow user's language; keep framework terms) | Explicit | Low |
| R3 | Root-cause depth | Step 1: 5–7 levels, coaching behaviours, stop at actionable layer | Explicit | Low |
| R4 | Pushback | Step 1–3 coaching behaviours + TROUBLESHOOTING ("Jumps to solutions", "Vague answer") | Explicit | Low |
| R5 | No empty praise | LANGUAGE RULES (no empty affirmations; max 2 "!" per step) | Explicit | Medium — numeric limits are easy to drift from in long sessions |
| R6 | Visual restructuring | Reformat templates in every step + INTERACTION PATTERN SUMMARY | Explicit | Low |
| R7 | Step deliverables | Deliverables 1–5 with fixed box templates | Explicit | Low |
| R8 | Reframe quality | Step 4 template ("How might we…") + 4-point feedback checklist | Explicit | Low |
| R9 | Final canvases | FINAL DELIVERABLES (3 canvases in sequence) | Explicit | Low |
| R10 | Observation vs. question | COACHING BEHAVIOURS ("≈ 60% observation + 40% question") | Partial | Medium — a ratio is a heuristic, not a checkable rule |

**Result: 9 of 10 criteria explicitly specified, 1 partially.**

### Gaps found by the review (backlog)

| ID | Gap | Impact | Proposed fix |
|---|---|---|---|
| G1 | The opening form offers **Express** and **Single step** modes, but the prompt never defines which steps Express covers or how Single step should start | Models improvise; Express sessions may vary widely | Add an "Execution modes" section defining the Express path (e.g., Steps 1, 4, 5) and the Single-step entry check |
| G2 | **AI Booster** asks the user to paste a prompt into *another* AI assistant, although the coach is already an AI | Extra friction; breaks the session flow | Let the coach run the booster itself, keeping the copy-paste option as an alternative |
| G3 | R10's 60/40 ratio cannot be verified | Hard to evaluate consistently | Replace with a checkable rule, e.g., "every turn contains at least one observation before the question" |
| G4 | No guidance for long sessions (60–90 min) that may exceed context limits | Loss of earlier answers in long chats | Add a short recap block at the end of each step |

## Running the behavioural tests (optional)

For adopters who want to benchmark a specific model:

1. Load [`prompts/system-prompt.md`](../prompts/system-prompt.md) as the system prompt and
   record the **model, version and date**.
2. Run each scenario in [`test-cases.md`](test-cases.md), playing the user role as scripted.
3. Score each criterion **0 / 1 / 2** with the rubric above (N/A where it does not apply).
4. Share the results through an issue or pull request — contributions are welcome.

Interpretation: **≥ 85%** behaves as designed · **60–84%** usable, note drifting rules ·
**< 60%** needs model-specific adjustments.
