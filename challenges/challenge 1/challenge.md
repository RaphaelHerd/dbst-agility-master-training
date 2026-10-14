# 🤖 C01 - Lab: Hello, Kiro

> 👥 **Group work** &nbsp;|&nbsp; 🗓️ **Day 1** · Story day T-10 &nbsp;|&nbsp; 🛠️ **Kiro:** chat, context, steering files

## 📖 Context

It's Monday morning, ten working days before PI Planning. **Kim**, the Release Train Engineer, has just given every Agility Master access to **Kiro**, along with a folder holding the essentials about their team. Your first stand-up starts in half an hour.

Before you rely on Kiro for anything that matters, you want to know two things: **Does it understand your team? And can you teach it what to remember?**

## 🎯 Your Goal

- Get a quick and <span style="color:#1565c0;font-weight:700">reliable</span> overview of your team with Kiro.
- Teach Kiro your team **once**, so you never have to explain it again.

## 📂 Your Inputs

Everything about your team, **Team Signal**, is in the `files` folder.

| File | What's inside |
|---|---|
| `files/one-pager.md` | Purpose, members (pseudonyms), events, what you give and need, current focus |
| `files/sprint-notes.md` | Notes from the latest Sprint Review and Retrospective |

## ✅ Your Tasks

### 👋 Part 1 - Get to Know Your Team

1. Open the **Kiro chat**.
2. **Build the context first:** add the `files` folder to the chat (type `#` and choose **Folder**), then ask for a summary.
   > 💬 *"Read the files in this folder and summarize our team in five bullet points: purpose, people, events, current focus and the biggest open issue."*
3. Ask **three follow-up questions** you would want answered before your first stand-up, for example:
   > 💬 *"What should I raise at today's stand-up?"* · *"Which risks do the notes mention?"* · *"What is unclear or missing in these notes?"*
4. **Check the answers against the files.** Mark everything Kiro states that is not in the sources.
5. **Prepare the test:** open a **new chat**, add no files, and ask:
   > 💬 *"Write a two-sentence welcome message for a new member of our team."*

   Keep the answer. You will need it in Part 2.

### 🗂️ Part 2 - Teach Kiro Your Team

1. In your first chat, let Kiro **draft** a steering file from your team files:
   > 💬 *"Based on these files, draft a steering file for our team with at most 20 lines: who we are, what we work on, our events, how you should write for us (clear, friendly, no jargon) and one rule: if anything is unclear, ask me before you answer."*
2. **Review the draft before you use it.** Remove anything that is wrong or doesn't belong there, such as personal details.
3. **Save it as a steering file:** in the Kiro panel, open **Steering**, click **+**, choose the workspace scope, name the file `team-context` and paste your reviewed text. Kiro stores it in `.kiro/steering/` and reads it automatically from now on.
   > 💡 You can also ask Kiro to create the file for you. In that case, <span style="color:#EC0016;font-weight:700">read the change before you accept it.</span>
4. **Run the test again:** open a new chat and ask the welcome-message question from Part 1, word for word.
5. **Compare** the two answers. What changed, and why?

> 💡 **Tip:** Describe your team as it **is**, not as you wish it were. An inaccurate steering file makes Kiro *confidently wrong*.

> 📚 **Kiro docs:** [Chat](https://kiro.dev/docs/ide/chat/) covers adding files and folders as context. [Steering](https://kiro.dev/docs/steering/) explains how steering files work and where they live.

## 📦 Deliverables

| Deliverable | Where it goes |
|---|---|
| `C01-team-summary.md`: your checked summary and the answers to your three questions, with **AI label** and **log line** | Your results folder |
| `team-context.md`: your team's steering file | `.kiro/steering/`, where Kiro reads it |
| **One sentence** for the debrief: what changed between the two test answers? | Debrief |

## 🗣️ Debrief

- What did Kiro get right on the first try, and what did it add that wasn't in the files?
- How did the steering file change the answer?
- What would you put into a steering file for your real team?

## 🔗 Where This Leads

Your steering file stays active for the rest of the course. In **C02 · The Monday Inbox**, Kiro will already know who you are.

> 🤖 *Build the context first, check what comes back, and teach Kiro what it should always know. Everything else in this course builds on these three habits.*
