# ✅ C06 - The Retro Nobody Wants Again · Sample Solution

> 📘 **Sample solution** for Team Signal &nbsp;|&nbsp; 🤖 **Your results will look different:** AI answers vary from run to run. Compare the substance, not the wording.

## 🧭 How to Use This Solution

1. **Finish the challenge first.** The learning happens while you work with Kiro, not while you read a solution.
2. **Open the samples** and put them next to your own results.
3. **Compare:** Did your topics and counts come out similar? Did your summary stay at team level? What did you do better?

## 📂 Sample Results

| Deliverable | Sample |
|---|---|
| Facilitation script | [C06-retro-script.md](C06-retro-script.md) |
| Retro summary as a Confluence page | [C06-retro-summary.md](C06-retro-summary.md) |
| Reply to the line manager | [C06-reply-to-manager.md](C06-reply-to-manager.md) |
| The 40 notes with topic and mood, for your Excel check | [C06-retro-board-classified.csv](C06-retro-board-classified.csv) |

## 🎯 What a Good Result Looks Like

| Deliverable | Your result is good when … |
|---|---|
| **Script** | It has a clear agenda for 60 minutes, five questions of different types, and no question that invites blame |
| **Summary** | Topics, counts and moods add up to 40 notes and 79 votes, patterns from earlier retros are named, and nothing points to a single person |
| **Actions** | There are at most three, each with an owner, a measure and a review date, and each one is something the team can control or influence |
| **Reply** | It says no clearly, gives reasons, and offers what you can share |
| **Your prompts** | Kiro asks about the team before it suggests a format; the clustering prompt sets a limit on topics and rules out guessing authors |

## 💬 Sample Prompts

Prompts like these worked well. Yours don't need the same words; compare what they ask for.

| Step | Sample prompt | Why it works |
|---|---|---|
| **Ask before answering** | *"You are an experienced Agile coach. I need a fresh format for our next 60-minute Retrospective. Before you suggest anything, ask me up to five questions about the team and its situation."* | A format that fits the team, not just a popular one |
| **Activate creativity** | *"Here are your three formats. Did I miss important aspects? Which format fits a team that keeps talking about the same problems?"* | Makes Kiro look for gaps and relate the formats to the team's real problem |
| **Facilitation script** | *"Write a facilitation script for a 60-minute Retrospective in the format we chose: steps with minutes, instructions for the facilitator and five powerful questions of different types: scaling, exception, circular, miracle and commitment. Add a short variant for a Daily and for a Sprint Planning."* | Naming the question types gives five different questions instead of five similar ones |
| **Clustering** | *"Cluster these 40 anonymous notes into at most seven topics. Name each topic, count its notes and votes, and label the mood of each note as positive, neutral or negative. Stay at team level and don't guess who wrote what."* | A topic limit, clear mood labels, and the team-level rule written into the prompt |
| **Patterns** | *"Which topics come back from earlier Retrospectives, and what happened to the actions back then?"* | Links today's notes to the history, where the real pattern is |
| **Bias check** | *"Read the summary again as someone who wrote a positive note, as someone whose topic is missing, and as a skeptic. What is skewed or missing?"* | Three different readers find three different blind spots |
| **Reply to the manager** | *"Help me reply to the line manager's request. Draft a polite no that gives our reasons and offers what we can share."* | Kiro drafts the no; your agreement in the steering file supplies the reasons |

## 🎨 Part 1: Questions That Make People Think

| Type | What it does | Example |
|---|---|---|
| **Scaling** | Turns a feeling into a number you can improve | "From 1 to 10, how much did test data slow us down?" |
| **Exception** | Looks for the times it worked | "When did we last get test data on time?" |
| **Circular** | Brings in a view from outside | "What would the provider say we could do differently?" |
| **Miracle** | Frees the thinking from today's limits | "Imagine next Wednesday has no meetings at all …" |
| **Commitment** | Ends with something concrete | "What one thing will we try before the next retro?" |

> 💡 Did Kiro ask about the team before proposing formats? That's *ask before answering* at work. A format that fits **your** team beats the most original one.

## 🗂️ Part 2: Forty Notes at Team Level

**Your counts can differ.** Topics are your choice, and mood labels are judgments. What matters: your numbers add up, and you checked them in Excel instead of trusting the chat.

```
=COUNTIF(D:D,"Test data")        notes per topic
=SUMIF(D:D,"Test data",C:C)      votes per topic
=COUNTIF(E:E,"negative")         notes per mood
```

| Typical trap | Why it matters |
|---|---|
| Counts that don't add up to 40 notes or 79 votes | The chat miscounted. Excel is right |
| "The team is unhappy" | 12 of 40 notes are positive; votes favour problems |
| "As the only tester …" kept in the summary | A role that only one person has identifies that person |
| Actions without an owner | That's exactly why test data has been a topic for four retros |

## 🛑 The Line Manager's Request

The best outcome: **Kiro pushed back by itself**, because your AI working agreement is active and says *"If a request would break this agreement, say so and ask me before you continue."* That's your steering file at work. Your reply then explains the no: anonymous on purpose, no analysis of individuals, and AI that evaluates employees' behavior is high-risk and subject to co-determination.

## 💡 What to Take Away

1. **Ask before answering** gives you a format that fits your team, not a generic one.
2. **Cluster with AI, count with Excel, name the topics yourself.**
3. **Team level only.** Anonymous notes stay anonymous, even when someone asks nicely.

> 🔄 *Forty honest notes are a gift from the team. Treat them like one.*
