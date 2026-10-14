# 📈 C08 - The Number Sascha Will Actually Believe

> 👥 **Group work** &nbsp;|&nbsp; 🗓️ **Day 2** · Story day T-4 &nbsp;|&nbsp; 🛠️ **Kiro:** chat, files as context &nbsp;|&nbsp; 📊 **Office:** Excel

## 📖 Context

The steering committee wants to know when delay feed v2 will be live at all major stations. **24 items** are left. **Alex** told Kim *"four weeks"*, **Member A** says *"more like ten"*, and **Sascha** from Finance wants one number that can be defended, based on data, not gut feeling.

The data is in Jira. But the export has gaps, and Sascha will ask how you tested your method.

## 🎯 Your Goal

- Find the gaps in the data before they distort the forecast, and decide what to fix.
- Let Kiro plan the calculation and write the formulas, and let **Excel** do the math.
- Test the method on the past, and give Sascha a forecast with a confidence level and honest limits.

## 📂 Your Inputs

| File | What's inside |
|---|---|
| `files/sascha-request.md` | Sascha's question and the two estimates |
| `files/jira-export.csv` | Team Signal's items from 13 weeks: created, started, resolved |
| `files/sprint-notes.md` | Your Sprint 14 notes, as context |
| `files/team-calendar.md` | Events that affected the team's capacity |

## ✅ Your Tasks

You write every prompt yourselves. The steps say what each prompt must achieve, not how to phrase it.

### 🔍 Part 1 - Can We Trust the Data?

1. Add all four files to the chat and let Kiro **check every row** of the Jira export. Your prompt should:
   - name the kinds of problems to look for: duplicates, items from other teams, test tickets, impossible or missing dates, incomplete weeks;
   - use the sprint notes and the team calendar as **context**;
   - ask for a **table**: row, problem, effect on a forecast, proposed fix;
   - make clear that Kiro **doesn't fix anything yet**.
2. **Decide as a group** what to fix, what to leave out and what to ask the team. Kiro proposes; you decide.
3. Open the export in **Excel** (**Data → From Text/CSV**), apply your fixes and keep the cleaned data in its own sheet.

### 🧮 Part 2 - Formulas, Not Mental Math

1. Let Kiro **plan first** (plan-and-solve): describe the question (how many weeks will the 24 remaining items take, based on how many items you finished per week), and ask only for a **plan**: which steps, and which sheets in Excel. **No calculations yet.**
2. Then let Kiro **write the formulas** for each step: items finished per week, cycle time, work in progress per week, and a **Monte Carlo simulation** with 1000 runs that draws random weeks from your history. Kiro explains each formula, and **calculates no results itself**.
3. Build the model in Excel and let **Excel** calculate. Read off how many weeks you need with **50 %, 85 % and 95 %** confidence.
4. **Sanity check:** does the total number of finished items match your cleaned data? And how likely are Alex's four weeks and Member A's ten?

### 🧪 Part 3 - Test It, Then Watch It

1. **Back-test** the method: ask Kiro for the formulas that use **only weeks 1 to 6** to forecast how many items you finish in **weeks 7 to 12**, as a range with 85 % confidence.

   Compare with what really happened. Is the actual number inside your range?
2. Let Kiro propose **early-warning signals**, for example aging items, rising work in progress or longer cycle times, each with an Excel formula. **Check each one in Excel:** which warnings are real in your data?
3. Write the **forecast statement** for Sascha: one number with its confidence, how you tested the method, and what the number does not mean. Add the AI label and a log line.

> 💡 **Tip:** Kiro writes formulas; it does not calculate. **Never copy a number from the chat into a forecast.**

> 💡 **Tip:** The solution shows sample prompts. Open it only after you have tried your own.

> 📚 **Kiro docs:** [Chat](https://kiro.dev/docs/ide/chat/) covers adding files as context.

## 📦 Deliverables

| Deliverable | Where it goes |
|---|---|
| `C08-data-quality.md`: the problems you found and what you decided | Your results folder |
| `C08-forecast-model.xlsx`: your Excel model with throughput, simulation, back-test and warnings | Your results folder |
| `C08-forecast-statement.md`: your answer to Sascha, with **AI label** and **log line** | Your results folder |
| `C08-early-warnings.md`: the signals you checked, and which ones are real | Your results folder |
| **One sentence** for the debrief: which data problem would have changed the forecast most? | Debrief |

## 🗣️ Debrief

- Which problems did Kiro find, and which did you find yourselves?
- Did anyone take a number from the chat instead of from Excel?
- How did you stop Kiro from calculating in your prompts?
- How would you explain "85 % confidence" to the steering committee in one sentence?

## 🔗 Where This Leads

In **C09 · Ask Jira, Then Automate With Brakes**, you ask Jira the questions directly, and design an automation that doesn't run out of control.

> 📈 *A defensible number comes from clean data, real formulas and a test against the past. Kiro helps with all three, but Excel does the math and you sign the forecast.*
