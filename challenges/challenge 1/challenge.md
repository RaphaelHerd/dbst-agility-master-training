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

You write every prompt yourselves. The steps say what each prompt must achieve, not how to phrase it.

### 👋 Part 1 - Get to Know Your Team

1. Open the **Kiro chat**.
2. **Build the context first:** add the `files` folder to the chat (type `#` and choose **Folder**). Then write a prompt that gets you a **summary of your team in five bullet points**: purpose, people, events, current focus and the biggest open issue.
3. Write **three follow-up questions** of your own: what would you want to know before your first stand-up?
4. **Check the answers against the files.** Mark everything Kiro states that is not in the sources.
5. **Prepare the test:** open a **new chat** and add no files. Ask a short question that only someone who knows your team can answer well, for example for a welcome message to a new team member. **Write your question down word for word,** and keep the answer. You will need both in Part 2.

### 🗂️ Part 2 - Teach Kiro Your Team

1. Back in your first chat, write a prompt that lets Kiro **draft a steering file** from your team files. The draft must:
   - have **at most 20 lines**;
   - say who you are, what you work on, which events you have and how Kiro should write for you;
   - contain one rule: **if anything is unclear, Kiro asks before it answers.**
2. **Review the draft before you use it.** Remove anything that is wrong or doesn't belong there, such as personal details.
3. **Save it as a steering file:** in the Kiro panel, open **Steering**, click **+**, choose the workspace scope, name the file `team-context` and paste your reviewed text. Kiro stores it in `.kiro/steering/` and reads it automatically from now on.
   > 💡 You can also ask Kiro to create the file for you. In that case, <span style="color:#EC0016;font-weight:700">read the change before you accept it.</span>
4. **Run the test again:** open a new chat and ask your test question from Part 1, word for word.
5. **Compare** the two answers. What changed, and why?

> 💡 **Tip:** A good prompt says what Kiro should read, what you want back, and in which form. If the answer misses the mark, improve the prompt and run it again. The solution shows sample prompts; open it only after you have tried your own.

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
- Which of your prompts needed a second try, and what did you change?
- How did the steering file change the answer to your test question?
- What would you put into a steering file for your real team?

## 🔗 Where This Leads

Your steering file stays active for the rest of the course. In **C02 · The Monday Inbox**, Kiro will already know who you are.

> 🤖 *Build the context first, check what comes back, and teach Kiro what it should always know. Everything else in this course builds on these three habits.*
