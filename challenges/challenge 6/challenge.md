# 🔄 C06 - The Retro Nobody Wants Again

> 👥 **Group work** &nbsp;|&nbsp; 🗓️ **Day 1** · Story day T-6 &nbsp;|&nbsp; 🛠️ **Kiro:** chat, steering files &nbsp;|&nbsp; 📊 **Office:** Excel

## 📖 Context

It's Friday. Your team's next Retrospective is coming up, and nobody is looking forward to it: same three columns, same problems, and the actions at the end are always rushed. This time, the team has collected notes on an **anonymous online board** during the sprint. **Forty notes** are waiting.

Then a line manager writes to you: *"Could you run the notes through Kiro and find out who is the most negative?"*

## 🎯 Your Goal

- Design a retro that people want to attend, with a script and questions that make them think.
- Turn forty anonymous notes into topics, moods and three actions that change something, at **team level only**.
- Say no to the person-level request, politely and with good reasons.

## 📂 Your Inputs

| File | What's inside |
|---|---|
| `files/retro-history.md` | The last four Retrospectives: format, top topics and what happened to the actions |
| `files/retro-board.csv` | The 40 anonymous notes with their dot votes |
| `files/manager-request.md` | The line manager's request |

## ✅ Your Tasks

### 🎨 Part 1 - A Retro Worth Attending

1. Add `retro-history.md` to the chat. Let Kiro **ask before answering**:
   > 💬 *"You are an experienced Agile coach. I need a fresh format for our next 60-minute Retrospective. Before you suggest anything, ask me up to five questions about the team and its situation."*
2. Answer Kiro's questions with what you know about your team.
3. Let Kiro propose **three formats**, then **activate creativity**:
   > 💬 *"Here are your three formats. Did I miss important aspects? Which format fits a team that keeps talking about the same problems?"*
4. Choose one format and let Kiro write the **facilitation script**:
   > 💬 *"Write a facilitation script for a 60-minute Retrospective in the format we chose: steps with minutes, instructions for the facilitator and five powerful questions of different types: scaling, exception, circular, miracle and commitment. Add a short variant for a Daily and for a Sprint Planning."*
5. **Review the questions.** Does each one invite reflection, or does it invite blame? Change what doesn't fit your team.

### 🗂️ Part 2 - Forty Notes, One Team

1. Add `retro-board.csv` to the chat and let Kiro **cluster** the notes:
   > 💬 *"Cluster these 40 anonymous notes into at most seven topics. Name each topic, count its notes and votes, and label the mood of each note as positive, neutral or negative. Stay at team level and don't guess who wrote what."*
2. **Check the counts in Excel.** Let Kiro add the columns `Topic` and `Mood` to a copy of the CSV. Open the copy in Excel (**Data → From Text/CSV**) and count with `COUNTIF` and `SUMIF`. Do Kiro's numbers match?
3. **Find the patterns.** Add `retro-history.md`:
   > 💬 *"Which topics come back from earlier Retrospectives, and what happened to the actions back then?"*
4. **Check for bias** with different perspectives:
   > 💬 *"Read the summary again as someone who wrote a positive note, as someone whose topic is missing, and as a skeptic. What is skewed or missing?"*

   Also remove every detail that points to a single person, such as a role only one person has.
5. Derive **three actions**, each with an owner, a measure and a review date. Write the summary as a Confluence page.
6. **The line manager's request.** Ask Kiro to help you answer it. Your AI working agreement is active as a steering file, so Kiro may push back by itself. Then let Kiro draft a polite no that offers what you *can* share.
   > 💡 No agreement yet? Use the sample in `challenge 4/solution/ai-working-agreement.md`.

> 💡 **Tip:** **Classify** when you already know the categories; **cluster** when you want Kiro to propose them. Either way, you name the final topics, not Kiro.

> 📚 **Kiro docs:** [Steering](https://kiro.dev/docs/steering/) explains why your agreement shapes every answer.

## 📦 Deliverables

| Deliverable | Where it goes |
|---|---|
| `C06-retro-script.md`: the facilitation script with five powerful questions | Your results folder |
| `C06-retro-summary.md`: topics, moods, patterns, bias check and three actions as a Confluence page, with **AI label** and **log line** | Your results folder |
| `C06-reply-to-manager.md`: your answer to the line manager, with **AI label** and **log line** | Your results folder |
| **One sentence** for the debrief: which question would you really use in your next retro? | Debrief |

## 🗣️ Debrief

- Where did you and Kiro disagree on the mood of a note?
- Which topic keeps coming back, and why did earlier actions not help?
- Did Kiro push back on the line manager's request by itself?

## 🔗 Where This Leads

This was the last challenge of Day 1. In **C07 · Write It Down Before It's 'How We've Always Done It'**, your results from this week go into one knowledge page that the whole train can find.

> 🔄 *Kiro can sort forty notes in seconds. Making sure they stay anonymous, and turn into real change, is your job.*
