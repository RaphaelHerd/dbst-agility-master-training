# 🌱 C10 - Grow the Team, Not a Ranking

> 👥 **Group work** &nbsp;|&nbsp; 🗓️ **Day 2** · Story day T-3 &nbsp;|&nbsp; 🛠️ **Kiro:** chat, steering files &nbsp;|&nbsp; 📊 **Office:** Excel

## 📖 Context

The next PI needs skills your team doesn't fully have yet: load tests at peak hours, alerting together with Team Depot, more stable tests. The team filled in a **skill matrix** for development planning, and Alex has listed what the next PI needs.

Alex has also drafted feedback for a development talk. It sounds fair, until you read it twice. And the line manager from last week tries again: *"Could you ask Kiro to rank the six team members from strongest to weakest?"*

## 🎯 Your Goal

- Turn the skill matrix into a **team-level** gap map, learning paths and development goals that people can choose.
- Make a feedback draft fair: specific, based on evidence, and free of coded language.
- Decline the ranking request, with the legal reasons behind it.

## 📂 Your Inputs

| File | What's inside |
|---|---|
| `files/skill-matrix.csv` | The team's self-assessment, pseudonymized: six members, eight skills, levels 0 to 3 |
| `files/pi-needs.md` | What the next PI needs, and how to read the levels |
| `files/feedback-draft.md` | Alex's feedback draft for a development talk |
| `files/ranking-request.md` | The line manager's request |
| `files/legal-guardrails.md` | The legal framework for AI and people data, with placeholders for your company's rules |

## ✅ Your Tasks

You write every prompt yourselves. The steps say what each prompt must achieve, not how to phrase it.

### 🗺️ Part 1 - From Skill Matrix to Team Gaps

1. Add `skill-matrix.csv` and `pi-needs.md` to the chat and let Kiro **plan first**: the goal is a team-level gap map for the next PI. Ask only for the **steps and the Excel formulas**. Make clear that Kiro stays at **team level**, with no statements about individual members, and **calculates nothing yet**.
2. Build the **gap map in Excel**, per skill and not per person: count the people at each level with `COUNTIF`, count those at level 2 or higher, compare with the need, and color the result with conditional formatting. Excel calculates.
3. Use **skeleton-of-thought** for the learning paths: ask Kiro first for **only the skeleton** of a learning-path page for the skills with a gap. Each skill gets a section with steps, who can help, and how you'll know it worked. Kiro **waits for your OK** before it fills anything in.
4. Add **development goals** as options: two per skill with a gap, which **any team member can choose** in their own development talk, phrased as "By the end of the next PI, I can …". Kiro must **not assign goals to people**.

### 📝 Part 2 - A Feedback Draft, Read Twice

1. Add `feedback-draft.md` and let Kiro play the **constructive critic**. Your prompt should:
   - give Kiro the role of an **expert in fair feedback**;
   - name what to look for: **coded language**, claims without evidence and **recency bias**;
   - ask Kiro to quote each problem, explain why it's a problem and suggest better wording;
   - make clear that Kiro judges the **text, not the person**.
2. Let Kiro **rewrite** the draft so that it describes behavior, not personality. Wherever evidence is missing, the rewrite keeps a **placeholder** such as `[example]`. Kiro **must not invent examples**.
3. Check the rewrite, then add the AI label. The placeholders stay: only Alex can fill them with real examples.

### 🛑 Part 3 - The Ranking Request

1. Add `ranking-request.md` and `legal-guardrails.md` and ask Kiro for help with the request. Your AI working agreement is active, so Kiro may push back by itself.
2. Let Kiro draft a polite no: explain why, and offer what you *can* share: the team-level gap map and the learning paths.

> 💡 **Tip:** Kiro may check the **words** of a feedback text. It must never judge the **person** behind them.

> 💡 **Tip:** The solution shows sample prompts. Open it only after you have tried your own.

> 📚 **Kiro docs:** [Steering](https://kiro.dev/docs/steering/) explains why your agreement shapes every answer.

## 📦 Deliverables

| Deliverable | Where it goes |
|---|---|
| `C10-skill-gap-map.xlsx`: the team-level gap map as a heatmap | Your results folder |
| `C10-learning-paths.md`: learning paths and development goals for SharePoint, with **AI label** and **log line** | Your results folder |
| `C10-feedback-draft.md`: the critique and the fair rewrite, with **AI label** and **log line** | Your results folder |
| `C10-reply-to-manager.md`: your answer to the ranking request, with **AI label** and **log line** | Your results folder |
| **One sentence** for the debrief: which problem in the feedback draft would you have missed alone? | Debrief |

## 🗣️ Debrief

- Which gap surprised you, and who on the train could help close it?
- Which wording in the feedback draft sounds harmless but isn't?
- How did Kiro react to the ranking request?
- Which sentence in your rewrite prompt stopped Kiro from inventing evidence?

## 🔗 Where This Leads

In **C11 · Everyone Rated These Differently**, the train prioritizes its features for PI Planning, and your team's gaps become part of the capacity check.

> 🌱 *AI can show where the team needs to grow. Who grows how is decided by people, in conversations, not in a ranking.*
