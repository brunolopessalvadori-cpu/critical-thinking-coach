# 🧠 Critical Thinking Coach — LLM Prompt

A system prompt that turns any LLM (ChatGPT, Claude, Gemini, Copilot, etc.) into a Critical Thinking coach, guiding the user through a 5-step methodology to move from vague problems to actionable solutions.

> **Core idea:** the biggest risk in complex environments is not a lack of solutions — it's solving the wrong problem.

## What it does

| Step | Name | Tool |
|------|------|------|
| 1️⃣ | UNDERSTAND | 5 Whys |
| 2️⃣ | EXPLORE | Empathy Maps |
| 3️⃣ | CHALLENGE | Roleplay & Tensions |
| 4️⃣ | REFRAME | Problem Statement V2 |
| 5️⃣ | OPEN | Crazy 8 + AI Booster |

At the end, the user receives 3 deliverables: **Critical Thinking Canvas**, **Action Plan**, and **Summary Card**.

## How to use

1. Copy the content of [`prompts/system-prompt.md`](prompts/system-prompt.md).
2. Paste it as the *system prompt* / *custom instructions* / *custom GPT* / *Project instructions* on your platform of choice.
3. Start a conversation — the coach will display the opening message and run the session.

### Compatibility

- **With support for interactive forms** (e.g., interfaces that render UI JSON): the initial form works natively.
- **Without form support:** the model should ask the same questions as plain text (see the *Fallback* section in the prompt).

## Design principles

- **A single form** at the start; everything else happens through chat.
- **Automatically follows the user's language** (framework terms stay in English).
- **Coach, not cheerleader:** direct observations, no empty praise.
- **Visual structure:** the user's free-text answers are reformatted into tables and cards.

## Customization

- Adjust the tone in `LANGUAGE RULES`.
- Swap or add tools within the steps (e.g., replace Crazy 8 with another technique).
- Change the deliverable formats in `FINAL DELIVERABLES`.

## License

MIT — see [LICENSE](LICENSE).

## Contributing

Issues and PRs are welcome: prompt improvements, translations, sample sessions, and adaptations for other platforms.
