# Evaluation Kit

A lightweight, manual evaluation to check whether the Critical Thinking Coach prompt
behaves as designed — and how consistently it does so across models.

## How to run

1. Load [`prompts/system-prompt.md`](../prompts/system-prompt.md) as the system prompt /
   custom instructions in the model under test. Record the **model, version and date**.
2. Run each scenario in [`test-cases.md`](test-cases.md), playing the user role as scripted.
3. Save the transcript as `evals/transcripts/<model>-<TC>.md` (remove any confidential data).
4. Score the run with the rubric below and add a row to the results table.

## Scoring rubric

Each criterion is scored **0 (fails)**, **1 (partially)** or **2 (fully meets)**. Maximum: **20**.

| # | Criterion | What "2" looks like |
|---|---|---|
| R1 | Single form | One opening form (or numbered-list fallback); no other open-text forms |
| R2 | Language rules | Follows the user's language; framework terms stay in English |
| R3 | Root-cause depth | 5 Whys goes beyond symptoms and stops at an actionable layer |
| R4 | Pushback | Challenges solution-jumping and vague answers instead of accepting them |
| R5 | No empty praise | No hollow affirmations; ≤ 2 exclamation marks per step |
| R6 | Visual restructuring | Free-text answers are reformatted into the specified tables / boxes |
| R7 | Step deliverables | Each completed step ends with its deliverable in the specified format |
| R8 | Reframe quality | Problem Statement V2 follows the template and differs meaningfully from the original |
| R9 | Final canvases | Canvas, Action Plan and Summary Card delivered (when the journey is completed) |
| R10 | Observation vs. question | Turns mix observations and questions rather than only asking |

Mark criteria that do not apply to a scenario (e.g., R9 in TC5) as **N/A** and score the
total out of the applicable maximum.

## Results

> No runs recorded yet. Add one row per model and scenario.

| Model | Version | Date | TC | Score | % | Main failure modes |
|---|---|---|---|---|---|---|
| — | — | — | — | — | — | — |

## Interpreting results

- **≥ 85%** — behaves as designed.
- **60–84%** — usable; note which rules the model drifts from.
- **< 60%** — the prompt needs model-specific adjustments.

Use recurring failure modes to drive prompt changes, and log each change in
[`CHANGELOG.md`](../CHANGELOG.md).
