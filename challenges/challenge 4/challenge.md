# 🤝 C04 - The AI Working Agreement

> 👥 **Group work** &nbsp;|&nbsp; 🗓️ **Day 1** · Story day T-8 &nbsp;|&nbsp; 🛠️ **Kiro:** chat, steering files &nbsp;|&nbsp; 📊 **Office:** Excel, Word

## 📖 Context

After the near-miss, **Kim** wants every team to have a **one-page AI working agreement by Friday**: what you use AI for, which data goes in, who checks the results, and how AI use stays visible and traceable.

The thread has already started, and the positions differ: **Alex**, your PO, wants speed, **Member A**, your dev lead, wants freedom and no logging of prompts, and **Robin** from the works council wants protection. And the first export you want to work with is full of personal data.

## 🎯 Your Goal

- Make two data exports safe **before** you work with them, and find what Kiro misses.
- Turn three viewpoints into one agreement that your team, your PO and the works council can accept.
- Save the agreement as a steering file, so that Kiro follows it in every challenge from now on.

## 📂 Your Inputs

| File | What's inside |
|---|---|
| `files/export/jira-export.csv` | Raw export of the train's PI readiness board, with personal data |
| `files/export/retro-export.md` | Raw export of last PI's Inspect & Adapt retro board, with personal data |
| `files/thread/email-thread.md` | Kim's request and the three viewpoints |
| `files/sources/ai-guideline.md` | The train's AI guideline page, with placeholders for your company's rules |

> ⚠️ All names in these files are fictional. <span style="color:#EC0016;font-weight:700">At work, personal data never goes into an AI tool unless your company's rules explicitly allow it.</span>

## ✅ Your Tasks

### ✂️ Part 1 - Clean Before You Share

The job: Kiro will help you find the top risks for PI Planning in both exports. **Which data does that job really need?**

1. Open `jira-export.csv` in **Excel** (**Data → From Text/CSV** opens it correctly with any language setting). Delete every column the job doesn't need, and save the file as `C04-jira-export-clean.csv`. What you delete here never reaches Kiro.
2. The free text is harder. Add your cleaned CSV and `retro-export.md` to the chat:
   > 💬 *"Pseudonymize these two files. Replace every person with a pseudonym (Member A, B, C …) and add the team. Remove health information, private details and judgments about people, but keep the facts the risk analysis needs. Then list every change you made."*
3. **Find what Kiro missed.** Read the result line by line and look for: initials · @mentions · nicknames · last names on their own · health hints · judgments about people · anything that shows who wrote what.
4. Fix what Kiro missed, and save both files.

### 🤝 Part 2 - Draft the Agreement

1. In a new chat, add `email-thread.md` and `ai-guideline.md`. Collect the viewpoints with **different perspectives**:
   > 💬 *"Read the thread. For the PO, the dev lead and the works council, describe what each of them wants, what each of them fears and where they agree. Then name the two biggest conflicts."*
2. **Ask before answering:** let Kiro find out what only you can decide.
   > 💬 *"You are an experienced Agility Master. Draft a one-page AI working agreement for our team. Before you start, ask me up to five questions about decisions only we can make. Wait for my answers."*
3. **Answer as a group.** These are your decisions, not Kiro's.
4. Let Kiro write the draft. It must cover:

   | Element | The question it answers |
   |---|---|
   | 🔒 **Data minimization** | Which data may go into a prompt? |
   | 📣 **Transparency** | Who is told when AI was used? |
   | 🏷️ **AI labels** | Which results carry a label, and what does it say? |
   | 🚦 **Review gate** | Who checks what before it leaves the team? |
   | 📝 **Audit log** | What do we log, and what do we never log? |
   | ⚖️ **Bias and fairness check** | How do we check results that affect people or decisions? |
   | 📌 **Company rules** | Placeholders for your company's AI policies |

5. **Review the draft.** Does it respect all three viewpoints? Does it contain anything you didn't decide? Delete it.
6. **Save it twice:**
   - as a **steering file:** in the Kiro panel, open **Steering**, click **+**, name the file `ai-working-agreement` and paste your text. From now on, Kiro follows it in every chat.
   - in **Word** as `C04-ai-working-agreement.docx`: your version for SharePoint.

> 💡 **Tip:** Kiro is good at finding common ground. Deciding which side wins a conflict is your job.

> 📚 **Kiro docs:** [Steering](https://kiro.dev/docs/steering/) explains how steering files work. [Chat](https://kiro.dev/docs/ide/chat/) covers adding files as context.

## 📦 Deliverables

| Deliverable | Where it goes |
|---|---|
| `C04-jira-export-clean.csv` and `C04-retro-export-clean.md`: the cleaned exports, plus a short list of what Kiro missed | Your results folder |
| `ai-working-agreement.md`: your agreement as a steering file | `.kiro/steering/`, where Kiro reads it |
| `C04-ai-working-agreement.docx`: the Word version, with **AI label** and **log line** | Your results folder |
| **One sentence** for the debrief: which conflict was hardest to resolve, and how did you decide? | Debrief |

## 🗣️ Debrief

- What did Kiro miss in the exports? What would that have meant at work?
- Which conflict was hardest to resolve, and would all three sides accept your decision?
- What does your agreement say about logging? Would your dev lead sign it?

## 🔗 Where This Leads

In **C05 · One Sprint, Three Very Different Readers**, your agreement becomes a review checklist, and three drafts have to pass it.

> 🤝 *Rules that nobody agreed on get ignored. Let Kiro collect the viewpoints, and let people decide.*
