# 📣 C05 - One Sprint, Three Very Different Readers

> 👥 **Group work** &nbsp;|&nbsp; 🗓️ **Day 1** · Story day T-7 &nbsp;|&nbsp; 🛠️ **Kiro:** chat, steering files &nbsp;|&nbsp; 📊 **Office:** Excel, Word

## 📖 Context

The steering committee meets next week, and **Kim** is collecting Sprint 14 from every team. The same facts have to reach three very different readers: **your team**, the **steering committee** and **Rail Ops**. Each of them needs a different text, and each of them will notice a wrong number.

Alex, your PO, also needs a decision from the steering committee. And since yesterday, your team has an AI working agreement: <span style="color:#EC0016;font-weight:700">nothing leaves the team without passing your review gate.</span>

## 🎯 Your Goal

- Turn one set of facts into three drafts, each written for its reader.
- Check every number before anything leaves the team.
- Turn your AI working agreement into a reusable review checklist, and run all three drafts through it.

## 📂 Your Inputs

| File | What's inside |
|---|---|
| `files/kim-request.md` | Kim's mail: the three drafts and the rules for them |
| `files/sprint-notes.md` | Your Sprint 14 notes |
| `files/jira-export.csv` | Your Sprint 14 items from Jira |
| `files/decision-needed.md` | Alex's note on the decision for the steering committee |
| `files/ai-working-agreement.md` | A sample agreement, in case yours from C04 isn't ready |

## ✅ Your Tasks

You write every prompt yourselves. The steps say what each prompt must achieve, not how to phrase it.

### ✍️ Part 1 - One Set of Facts, Three Drafts

1. **Facts first.** Add the `files` folder to the chat and write a prompt that turns the sprint notes and the Jira export into a **fact list**: goal, items with status, numbers and blockers. Make sure Kiro reads **every line** of both files and **marks every place where they disagree**.
2. **Check the fact list.** Where the files disagree, decide which one is right. Do any math in **Excel**, not in the chat.
3. **One prompt per reader.** Give Kiro a role, a tone and a skeleton, and tell it what to leave out:

   | Reader | Role and tone | Skeleton | Leave out |
   |---|---|---|---|
   | 👥 Your team | Agility Master to the team: friendly and direct | Done · open · next | Background the team already knows |
   | 🏛️ Steering committee | Agility Master to decision-makers: factual | Decision needed · background · options · recommendation · if no decision is made | Ticket IDs and technical detail |
   | 🚉 Rail Ops | Agility Master to operations: plain language | What changes for you · what we need from you | Ticket IDs, internal system names, people's names, jargon |

   For the decision paper, use **skeleton-of-thought**: your prompt tells Kiro who reads the paper and how much time they have, asks for **only the skeleton** of a one-page paper first, and makes Kiro **wait for your OK** before it fills anything in.
4. **Check every number** in all three drafts against the sprint notes and Jira.

### 🚦 Part 2 - Your Review Gate

1. Write a prompt that turns your AI working agreement into a **review checklist** for drafts that leave the team: **at most 10 checks**, each one answerable with **pass or fail**.
2. **Save it as a reusable prompt:** open the steering file `review-checklist` that you sketched in Setup 03 and paste the checklist below the three lines of front matter. No file yet? In the Kiro panel, open **Steering**, click **+**, name the file `review-checklist`, paste the checklist and put these three lines at the very top, so that Kiro loads the file only when you call it:

   ```
   ---
   inclusion: manual
   ---
   ```
3. **Run each draft through your gate:** type `#review-checklist` in the chat, followed by the draft.
4. **Fix what fails.** Then a person signs off: add the AI label and a log line to each draft.
5. Copy the decision paper into **Word** and save it as `C05-decision-paper.docx`.

> 💡 **Tip:** The checklist finds problems. Whether a draft is good enough is still your call.

> 💡 **Tip:** The solution shows sample prompts. Open it only after you have tried your own.

> 📚 **Kiro docs:** [Steering](https://kiro.dev/docs/steering/) explains manual inclusion and how to call a steering file with `#`.

## 📦 Deliverables

| Deliverable | Where it goes |
|---|---|
| `C05-team-update.md`, `C05-decision-paper.docx` and `C05-rail-ops-note.md`: three signed-off drafts, each with **AI label** and **log line** | Your results folder |
| `review-checklist.md`: your reusable review checklist | `.kiro/steering/`, where Kiro reads it |
| **One sentence** for the debrief: which check caught something you had missed? | Debrief |

## 🗣️ Debrief

- Where did Jira and the sprint notes disagree, and who noticed first: you or Kiro?
- What did Kiro have to leave out for Rail Ops, and did it?
- How did your three reader prompts differ from each other?
- Which check in your review gate caught something?

## 🔗 Where This Leads

Your review checklist stays in your toolbox for the rest of the course. In **C06 · The Retro Nobody Wants Again**, you use AI on the most sensitive data a team has: what people say in a retro.

> 📣 *One set of facts, three readers, one review gate. Kiro writes the versions; you make sure every one of them is true.*
