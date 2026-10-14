# ⚖️ C11 - Everyone Rated These Differently

> 👥 **Group work** &nbsp;|&nbsp; 🗓️ **Day 2** · Story day T-2 &nbsp;|&nbsp; 🛠️ **Kiro:** chat, files as context &nbsp;|&nbsp; 📊 **Office:** Excel

## 📖 Context

Thursday, two working days to PI Planning. Product Management has shared the top 10 features, ranked by WSJF. But the ranking is an **average of three business owners**, and they scored the same features very differently. **Kim** wants to know where they disagree, and which assumption would change the top 3, before the meeting with Product Management.

Then **Alex** writes: two of your six team members won't be available in the next PI, and Team Concourse needs your platform-change events by the end of Sprint 2.

## 🎯 Your Goal

- Turn three sets of scores into one transparent WSJF ranking: Excel calculates, and the disagreements stay visible.
- Run a decision check: which assumption would change the top 3?
- Compare three PI scenarios against your new capacity, and decide as a team.

## 📂 Your Inputs

| File | What's inside |
|---|---|
| `files/kim-request.md` | Kim's request and the WSJF formula |
| `files/wsjf-scores.csv` | The scores of three business owners for ten features |
| `files/features.csv` | The ten features with job sizes from the teams and short notes |
| `files/capacity-news.md` | Alex's news, your velocity and your planned work for the next PI |

## ✅ Your Tasks

### 📊 Part 1 - One Ranking, Open Eyes

1. Add `kim-request.md`, `wsjf-scores.csv` and `features.csv` to the chat. Let Kiro **plan the consolidation and write the formulas**:
   > 💬 *"For each feature and each WSJF component, we need the average, the median and the spread between the highest and the lowest score. Then WSJF from the averages and from the medians. Write the Excel formulas and explain them. Don't calculate anything yourself."*
2. Build the sheet in **Excel** and rank the features. Where do the owners disagree most?
3. Run a **decision check** with step-back prompting:
   > 💬 *"Step back first: which principles should decide the order of features on a release train? Then look at our ranking: which single assumption would change the top 3? Check the notes in features.csv, too."*
4. Look for **bias**:
   > 💬 *"Compare the three business owners. Does anyone score their own area consistently higher? What does that mean for an average?"*
5. Write the **rationale for Kim**: the ranking, the biggest disagreements, what would change the top 3, and questions for Product Management. Not a decision: that stays with Product Management.

### 👥 Part 2 - Two People Fewer

1. Add `capacity-news.md` and let Kiro draft **three scenarios**:
   > 💬 *"Draft three scenarios for our next PI with two people fewer and the new dependency from Team Concourse. For each one: what we do, what moves to a later PI, and who is affected. Don't calculate the load; we'll do that in Excel."*
2. In **Excel**, calculate your capacity: average velocity × five sprints, adjusted to four of six people, minus 15 % for bugs. Then the load of each scenario as a share of the capacity.
3. Step back once more:
   > 💬 *"Which assumptions are hidden in our capacity calculation, and how could they be wrong?"*
4. **Decide as a group**, and write down who must be told: other teams, Kim, and anyone who relies on an earlier forecast.

> 💡 **Tip:** An average of three opinions can hide that nobody agrees. Show the spread next to every average.

> 📚 **Kiro docs:** [Chat](https://kiro.dev/docs/ide/chat/) covers adding files as context.

## 📦 Deliverables

| Deliverable | Where it goes |
|---|---|
| `C11-wsjf.xlsx`: scores, WSJF ranking and the scenario comparison | Your results folder |
| `C11-wsjf-rationale.md`: your note for Kim, with **AI label** and **log line** | Your results folder |
| `C11-scenarios.md`: the three scenarios, your decision and who must be told, with **AI label** and **log line** | Your results folder |
| **One sentence** for the debrief: which assumption surprised you most? | Debrief |

## 🗣️ Debrief

- Which feature divides the business owners most, and why?
- Which single assumption changes the top 3?
- Which scenario did you choose, and what does it mean for earlier promises?

## 🔗 Where This Leads

In **C12 · Nothing Ships in Isolation**, all four teams' plans come together, and your decisions meet everyone else's dependencies.

> ⚖️ *Kiro can line up the numbers and the assumptions. Which feature comes first, and which promise moves, is decided by people.*
