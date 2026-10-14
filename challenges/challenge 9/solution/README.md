# ✅ C09 - Ask Jira, Then Automate With Brakes · Sample Solution

> 📘 **Sample solution** for Team Signal &nbsp;|&nbsp; 🤖 **Your results will look different:** AI answers vary from run to run. Compare the substance, not the wording.

## 🧭 How to Use This Solution

1. **Finish the challenge first.** The learning happens while you work with Kiro, not while you read a solution.
2. **Open the samples** and put them next to your own results.
3. **Compare:** Do your queries return the same items? Which brakes does your automation have?

## 📂 Sample Results

| Deliverable | Sample |
|---|---|
| JQL cheat sheet | [C09-jql-cheat-sheet.md](C09-jql-cheat-sheet.md) |
| Weekly report | [C09-weekly-report.md](C09-weekly-report.md) |
| Automation design with change request | [C09-automation-design.md](C09-automation-design.md) |

## 🎯 What a Good Result Looks Like

| Deliverable | Your result is good when … |
|---|---|
| **JQL** | Each query returns exactly the expected items in the export, and you can explain every condition |
| **Weekly report** | It stays under 150 words, lists the facts, and says what the numbers don't mean |
| **Automation** | It has a delay, a once-only brake and an escalation ladder, plus a change request, a test plan and a warning; the approval stays with Kim and the Jira administrator |

## 🔎 Part 1: The Expected Results

| # | Question | Result | The row that almost fooled the query |
|---|---|---|---|
| 1 | Our blocked stories | SIG-145, SIG-147 | SIG-157 is blocked, but it's a task |
| 2 | Finished last week | 6 items | DEP-512 is "Won't Do"; CON-310 was finished the Sunday before |
| 3 | Bugs open for more than 30 days | SWI-198, CON-296, DEP-498 | SIG-150 is 27 days old |
| 4 | Waiting for another team | 5 items | CON-305 and SWI-222 wait for Rail Ops, not for a team |
| 5 | Stories without points | SIG-158, SWI-225, CON-315, DEP-514 | Four bugs have no points, on purpose |

> 💡 **Few-shot and contrastive in action:** the bad examples in `jql-examples.md` show Kiro what to avoid: `updated >= -7d`, `created < 30d` and `= 0`. Without them, mistakes like these are common.

> 💡 **Did Kiro ask before answering?** Questions 1 and 4 are ambiguous: stories or all blocked work? Is Rail Ops "another team"? A good run asks; a quick run guesses.

## ⚙️ Part 2: Why Alex's Rule Needs Brakes

| Without brakes | With brakes |
|---|---|
| A message for every short block | Only after two days |
| The same story again and again | Once, thanks to the label `escalated` |
| Straight to Kim and a big channel | The PO first, then the ART Sync |
| Live on day one | Change request, sandbox test, approval by people |
| A public list that invites comparisons | A written warning: stuck work, not blame |

> ⚠️ **A real JQL trap:** `labels != escalated` doesn't find issues without labels. Check what Kiro wrote, not only what it says the query does.

## 💡 What to Take Away

1. **Show Kiro good and bad examples:** few-shot plus contrastive prompting gives better queries.
2. **Check queries against real rows,** especially the ones that almost match.
3. **Automation needs brakes and a person who approves.** Prompt chaining gets you from the request to a change request, step by step.

> 🔎 *The query answered Kim's question. The brakes made sure the automation didn't create a new problem.*
