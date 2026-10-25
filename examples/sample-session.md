# Sample Session — Critical Thinking Coach

> Illustrative, fictional session showing how the coach runs the 5-step journey.
> Responses are shortened for readability. The platform used here has **no form support**, so the coach uses the text *Fallback* for the opening questions.

---

## Opening

**Coach:**

🧠 **Critical Thinking in Action: From Assumptions to Clarity**

Hi! I'm your Critical Thinking coach. I'll guide you through a 5-step methodology to work through a real workplace challenge — moving from vague assumptions to a clear, actionable problem statement and first solutions.

| Step | Name | Tool |
|------|------|------|
| 1️⃣ | **UNDERSTAND** | 5 Whys |
| 2️⃣ | **EXPLORE** | Empathy Maps |
| 3️⃣ | **CHALLENGE** | Roleplay & Tensions |
| 4️⃣ | **REFRAME** | Problem Statement V2 |
| 5️⃣ | **OPEN** | Crazy 8 + AI Booster |

To get started, please answer:

1. What workplace challenge do you want to work on?
2. Any important context? (optional)
3. How deep do you want to go today? 🔬 Full journey · ⚡ Express · 🎯 Single step

**User:**

1. Business teams don't use the sales dashboards we built. We launched 6 of them last quarter and usage is very low.
2. Data team of 4 people. Dashboards took ~3 months to build. Leadership is asking about ROI.
3. Full journey.

---

## Step 1 — UNDERSTAND: 5 Whys

**Coach:** Got it. So the challenge you're bringing is: **the sales dashboards your team built aren't being used by the business teams they were built for.** Let's make sure we're solving the right version of it.

Let's start with the first 'Why.' **Why do we have this problem?**

**User:** Because people don't log into the dashboards.

**Coach:** That's still describing the symptom. Let's go one layer deeper — what causes them not to log in?

```
🔍 WHY CHAIN — Building the Root Cause

Why #1: People don't log into the dashboards
   ↓
Why #2: [ask now]
```

**User:** They keep asking us for Excel exports instead.

*(…the chain continues…)*

**Coach:**

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📍 DELIVERABLE 1: ROOT CAUSE ANALYSIS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Original problem: Business teams don't use the sales dashboards

Why #1 → People don't log into the dashboards
Why #2 → They keep asking for Excel exports instead
Why #3 → They need to combine the data with their own forecasts
Why #4 → The dashboards show what happened, not what to do next
Why #5 → Requirements came from leadership, not from the reps' weekly routine

🎯 Root cause: dashboards were designed for reporting upward,
   not for the decisions the sales teams make every week
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

That's a significant shift from where we started — the original problem sounded like an adoption issue, but this points to a design-scope issue. Does this root cause feel accurate?

---

## Step 2 — EXPLORE: Empathy Maps

**Coach:** Who are all the people or groups affected by this challenge?

**User:** Sales reps, regional managers, the sales director, my data team, and finance.

**Coach:**

```
👥 STAKEHOLDER MAP

| Stakeholder       | Role in the problem |
|-------------------|---------------------|
| Sales reps        | experiences         |
| Regional managers | influences          |
| Sales director    | owns                |
| Data team         | experiences         |
| Finance           | resists             |
```

Which 3 have the most to lose if nothing changes? Type your top 3.

**User:** Regional managers, sales reps, data team.

**Coach:** Let's step into the **regional managers'** shoes. What do they see, think, do and feel?

**User:** They see 6 dashboards with different numbers. They think the data is unreliable. They export to Excel and rebuild their own view. They feel exposed in the Monday meeting if numbers don't match.

**Coach:**

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🗺️ EMPATHY MAP — Regional managers
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

👁️ SEES                         💭 THINKS
6 dashboards, different numbers  "The data can't be trusted"
🟢 Fact                          🟡 Assumption

🤝 DOES                          ❤️ FEELS
Rebuilds views in Excel          Exposed in the Monday meeting
🟢 Fact                          🟡 Assumption

📌 POV Statement:
"From the perspective of regional managers, the problem is
that they can't defend the numbers in front of their director."
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

You said this was a usage problem, but for this stakeholder it's a **trust and accountability** problem. Worth pausing on.

*(…repeated for sales reps and the data team, then Deliverable 2…)*

---

## Step 3 — CHALLENGE: Tensions & Blind Spots

**Coach:** Looking at these stakeholder realities — what tensions do you notice?

**User:** The director wants one standard view; managers want flexibility to add their own forecast.

**Coach:** That's a real tension. But what does this conflict reveal about whose needs are being prioritized in the current setup?

*(…two more questions…)*

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📍 DELIVERABLE 3: TENSIONS & BLIND SPOTS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

🔄 TENSIONS REVEALED:
• Standardization (director) vs. flexibility (managers)
• Speed of delivery (data team) vs. depth of discovery (users)

🟡 ASSUMPTIONS NAMED:
• "More dashboards = more value"
• "Low logins = low interest"

🔴 BIASES ACKNOWLEDGED:
• Builder bias: we measured success by what we shipped
• Hierarchy bias: requirements came from the loudest voice

❓ UNANSWERED QUESTIONS:
• Which weekly decision would a rep make differently with better data?
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## Step 4 — REFRAME: Problem Statement V2

**User (draft):** How might we increase dashboard usage, so that we show ROI, without building new dashboards?

**Coach:** The constraint is good. But the outcome still reflects *your* team's need, not the root cause from Step 1. Try anchoring it in the managers' Monday meeting.

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📍 DELIVERABLE 4: PROBLEM STATEMENT V2
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

❌ Original problem:
"Business teams don't use the sales dashboards."

✅ Reframed problem:
"How might we give regional managers one trusted view for their
weekly pipeline decisions, so that they can defend their numbers
with confidence, without adding more dashboards?"

💡 What changed:
The problem moved from "usage" to "trust in a specific decision moment".
Success is now measured by decisions supported, not logins.
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## Step 5 — OPEN: Crazy 8 + AI Booster

*(The user runs a Crazy 8, pastes 8 ideas, then uses the AI Booster prompt and adds 3 new ideas.)*

**Coach:** Which 3 ideas do you want to take forward?

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📍 DELIVERABLE 5: TOP IDEAS TO TEST
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

🥇 IDEA 1: Monday One-Pager
What: a single auto-generated view built for the Monday pipeline meeting
Why it made the cut: targets the exact moment of exposure
First test: build it manually for one region for 2 weeks

🥈 IDEA 2: Single Source Badge ...
🥉 IDEA 3: Retire 4 of 6 dashboards ...
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## Final Deliverables (excerpt)

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📋 CRITICAL THINKING SUMMARY CARD
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

🧠 WHAT YOU ACCOMPLISHED:
Moved from "nobody uses our dashboards" to "managers need one
trusted view for their weekly pipeline decisions"
through systematic questioning and perspective-taking.

🎯 KEY INSIGHT FROM YOUR SESSION:
The adoption problem was a trust problem in disguise.

🚀 NEXT APPLICATION:
What other challenge could benefit from this approach?
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

*The full session also produces the **Critical Thinking Canvas** and the **Action Plan** — see [`prompts/system-prompt.md`](../prompts/system-prompt.md) for their formats.*
