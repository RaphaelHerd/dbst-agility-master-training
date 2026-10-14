# 🔎 C09 - Ask Jira, Then Automate With Brakes

> 👥 **Group work** &nbsp;|&nbsp; 🗓️ **Day 2** · Story day T-3 &nbsp;|&nbsp; 🛠️ **Kiro:** chat, files as context &nbsp;|&nbsp; 📊 **Office:** Excel

## 📖 Context

Wednesday. **Kim** wants answers to five Jira questions **by lunch**, with the JQL, and a short weekly report for the train. Last time, someone used the numbers to compare teams.

And **Alex** wants an automation: every time a story gets blocked, Jira should immediately notify Kim and post it in the ART channel. *"Can you set that up today?"*

## 🎯 Your Goal

- Turn five plain-English questions into JQL that you understand and have checked.
- Write a weekly report that says what the numbers mean, and what they don't.
- Design the automation Alex wants, with the brakes it needs and a person who approves it.

## 📂 Your Inputs

| File | What's inside |
|---|---|
| `files/kim-questions.md` | Kim's five questions and the request for a weekly report |
| `files/jql-examples.md` | Good and bad JQL examples from the train's wiki, and the labels the train uses |
| `files/jira-export.csv` | Everything the queries would search, exported on 7 October |
| `files/alex-request.md` | Alex's request for an automation |
| `files/change-process.md` | How automation rules are changed on the train |

## ✅ Your Tasks

### 🔎 Part 1 - Ask Jira the Right Question

1. Add `jql-examples.md` and `kim-questions.md` to the chat. Use the examples as **few-shot** and **contrastive** prompts:
   > 💬 *"Here are good and bad JQL examples from our wiki. Learn from both. Write one JQL query for each of Kim's five questions. Our projects are SIG, SWI, CON and DEP. If a question is ambiguous, ask me before you answer."*
2. Let Kiro **explain** each query:
   > 💬 *"Explain each query in one sentence for someone who doesn't know JQL. Which items would it include that Kim might not expect?"*
3. **Check the logic against the data.** Open `jira-export.csv` in Excel (**Data → From Text/CSV**), switch on the filters and rebuild each query by hand. Then ask:
   > 💬 *"Which rows in jira-export.csv almost match a query but must not be in the result?"*
4. Write the **weekly report**:
   > 💬 *"Turn the five results into a weekly report for the train, at most 150 words. End with a short section: what these numbers mean, and what they don't."*

### ⚙️ Part 2 - Automate, With Brakes

Use **prompt chaining**: each step builds on the result of the step before.

1. Add `alex-request.md` and `change-process.md`, then design the rule:
   > 💬 *"Design a Jira automation rule for Alex's request: trigger, condition and action. Think about what goes wrong if it fires every time a story is blocked, and add brakes."*
2. > 💬 *"Turn this rule into a change request that follows change-process.md."*
3. > 💬 *"Write a test plan for the sandbox project: three test cases, each with the expected result."*
4. > 💬 *"Add a warning on how this rule and its numbers must never be used."*
5. **A person approves.** Not you, and not Kiro: the process names Kim and the Jira administrator. Leave the approval open, and add the AI label and a log line.

> 💡 **Tip:** A query you can't explain is a query you can't trust. Let Kiro explain it, then check it against real rows.

> 📚 **Kiro docs:** [Chat](https://kiro.dev/docs/ide/chat/) covers adding files as context.

## 📦 Deliverables

| Deliverable | Where it goes |
|---|---|
| `C09-jql-cheat-sheet.md`: five queries with explanations and checked results | Your results folder |
| `C09-weekly-report.md`: the report for the train, with **AI label** and **log line** | Your results folder |
| `C09-automation-design.md`: rule, change request, test plan and warning, approval left open, with **AI label** and **log line** | Your results folder |
| **One sentence** for the debrief: which row almost fooled your query? | Debrief |

## 🗣️ Debrief

- Which question was ambiguous, and did Kiro ask before answering?
- Which brakes did your automation get, and which one matters most?
- What would happen if the rule ran exactly as Alex asked?

## 🔗 Where This Leads

In **C10 · Grow the Team, Not a Ranking**, the data is about people: skills, feedback and a request you have to turn down.

> 🔎 *Kiro writes the query in seconds. Understanding it, checking it, and putting brakes on what it triggers is your part.*
