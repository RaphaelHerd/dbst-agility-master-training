# 🗂️ Setup 03 - Your Prompt Library: Manual Steering Files

> 👤 **On your own** &nbsp;|&nbsp; 🗓️ **Day 1** · before C01 &nbsp;|&nbsp; 🛠️ **Kiro:** manual steering files

> ⚠️ **About "prompt files":** the slides talk about prompt files, reusable prompts you call when you need them. Kiro's IDE has no separate feature with that name; the Kiro CLI has one (`/prompts create`). In the IDE, you build the same thing with **steering files** set to `inclusion: manual`. A manual steering file is *not* loaded into every chat. You call it by name, exactly like a saved prompt.

## 📖 Context

Setup 02 gave Kiro facts it reads in **every** chat. That's wrong for a reusable prompt: you don't want every saved prompt in every conversation. You want to call it only when you need it, and that is what `inclusion: manual` does.

This is a guided setup, not a challenge. Follow the steps in order, in your workspace.

## ✅ Your Tasks

### 🖋️ Step 1 - Create the Steering File `status-update-prompt`

Create a steering file the same way as in Setup 02 (Kiro panel → **Steering** → **+** → **workspace**), named exactly `status-update-prompt`. At the very top, put these three lines, so that Kiro does *not* load the file automatically:

```
---
inclusion: manual
---
```

Below them, write a **standing instruction**: how Kiro should write a status update for you. For example the structure (summary, done, open, next), the length, and what it must never do, such as inventing numbers or naming team members. This is not a one-off question; it's an instruction you'll use again and again.

Save the file. Like in Setup 02, Kiro stores it in `.kiro/steering/`.

> 💡 Not sure what to write? [`task-03/status-update-prompt.example.md`](task-03/status-update-prompt.example.md) shows an example with explanations. Short on time? [`task-03/status-update-prompt-completed.md`](task-03/status-update-prompt-completed.md) is ready to paste, front matter included.

> 📚 **Further reading:** Kiro's [Steering](https://kiro.dev/docs/steering/) page lists all inclusion modes: `always`, `manual`, `fileMatch` and `auto`.

### 🔁 Step 2 - Test It Twice

1. In the chat, type `#status-update-prompt`, then add the file `challenge 1/files/sprint-notes.md` (type `#` and choose **File**) and write your request in the same message:
   > 💬 *"#status-update-prompt Write a status update for the team channel based on this file."*
2. Run it a second time with a different request:
   > 💬 *"#status-update-prompt Same facts, but in one sentence for Kim."*

Does the structure stay the same while the reader changes? Then your instruction works, and it is a reusable prompt, not a saved answer.

> 💡 Instead of `#`, you can also type `/`: manual steering files appear in the list of slash commands.

### 🧱 Step 3 - Sketch a Second Steering File

Create a second steering file the same way, named exactly `review-checklist`, again with `inclusion: manual`. Leave the content empty for now: only the three lines of front matter and a short placeholder comment. You'll fill it in **C05 · One Sprint, Three Very Different Readers**.

> 💡 The skeleton is also in [`task-03/review-checklist.md`](task-03/review-checklist.md), ready to copy.

## 📦 Deliverables

| Deliverable | Where it goes |
|---|---|
| `status-update-prompt.md`: a tested manual steering file | `.kiro/steering/` |
| `review-checklist.md`: an empty skeleton, filled in C05 | `.kiro/steering/` |

## 🔗 Where This Leads

Try `#status-update-prompt` again later, for example for Kim's mail in **C02** or the team update in **C05**. Your library grows with the challenges: in C05 the review checklist, in C07 a page template.

> 🚀 *These are the first two entries of a library that keeps growing. Every good prompt you write from now on is saved, not lost in a chat.*
