# 🧭 Setup 02 - Steering Files: Giving Kiro a Memory

> 👤 **On your own** &nbsp;|&nbsp; 🗓️ **Day 1** · before C01 &nbsp;|&nbsp; 🛠️ **Kiro:** steering files

## 📖 Context

Right now, Kiro knows nothing about the case. You would have to explain the train, your role and your preferences again in every chat, for two days. **Steering files** fix that: they are files in your workspace that Kiro reads automatically, before it answers your question.

This is a guided setup, not a challenge. Follow the steps in order, in the workspace from Setup 01.

## ✅ Your Tasks

### 🔬 Step 1 - Ask the "Before" Question

Before you create any steering file, ask Kiro a question that needs context:

> 💬 *"What should I watch out for in the ten days before our PI Planning?"*

Kiro either asks you which train you mean, or it answers with something generic. Keep this answer: it's your "before".

### 📄 Step 2 - Create the Steering File `product-context`

1. Click the **Kiro icon** (a small ghost) in the activity bar at the edge of the window. The **Kiro panel** opens.
2. In the panel, find the **Steering** section and click **+**.
3. Choose the scope **workspace**, not global: this file belongs to this course only.
4. Name the file exactly `product-context` and paste this text:

   > This workspace belongs to a training case. Everything in it is fictional.
   >
   > I am an Agility Master on the release train ART SmartTransfer, ten working days before PI Planning. SmartTransfer is a passenger app that helps people make their train connections. The train has four teams: Signal (real-time train data), Switch (transfer logic), Concourse (the passenger app) and Depot (platform and operations). Kim is the Release Train Engineer. Team members appear only as pseudonyms (Member A, B, C …).
   >
   > You support me with drafts. I check them and decide: AI drafts, people decide.

5. Save it with **Ctrl+S** (Windows) or **Cmd+S** (Mac).

Kiro stores the file in `.kiro/steering/` and creates that folder by itself. Without front matter, a steering file is **always included**: Kiro reads it in every chat from now on.

> 💡 The text is also in [`task-02/product-context.md`](task-02/product-context.md), ready to copy.

> 📚 **Further reading:** Kiro's [Steering](https://kiro.dev/docs/steering/) page explains steering files and the other inclusion modes (`manual`, `fileMatch`, `auto`). You'll use `manual` in Setup 03.

### 🎨 Step 3 - Create the Steering File `my-conventions`

Create a second steering file the same way (Kiro panel → **Steering** → **+** → **workspace**), named exactly `my-conventions`. Write down **your own** preferences for how Kiro should answer you, for example:

- 🗣️ **Tone:** short and direct, or detailed and explanatory?
- 📐 **Structure:** headings and bullet points? A one-line summary first?
- 📏 **Level of detail:** what do you expect by default?

There is no right answer here. The file should reflect how *you* like to work.

> 💡 Not sure where to start? [`task-02/my-conventions.example.md`](task-02/my-conventions.example.md) shows an example with explanations. Short on time? [`task-02/my-conventions-completed.md`](task-02/my-conventions-completed.md) is ready to paste.

### 🔁 Step 4 - Ask the Same Question Again

Open a **new chat** and ask exactly the question from Step 1 again:

> 💬 *"What should I watch out for in the ten days before our PI Planning?"*

Now Kiro answers about ART SmartTransfer and its four teams, without you explaining anything, and in the style you asked for. Both steering files are loaded automatically.

### 📝 Step 5 - Write Down the Difference

Put the two answers side by side in a short note. It's your proof that the steering files really work.

Save it in your `results` folder as `S02-steering-before-after.md` (right-click `results` → **New File**).

## 📦 Deliverables

| Deliverable | Where it goes |
|---|---|
| `product-context.md`: the case context as a steering file | `.kiro/steering/`, created by Kiro |
| `my-conventions.md`: your preferences as a steering file | `.kiro/steering/` |
| `S02-steering-before-after.md`: the two answers compared | Your results folder |

## 🔗 Where This Leads

Kiro now knows the **train**. In **C01 · Lab: Hello, Kiro**, you teach it your **team**, with a third steering file.

> 🚀 *From now on, Kiro knows the case. You never have to explain it again.*
