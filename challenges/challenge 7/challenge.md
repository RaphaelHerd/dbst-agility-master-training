# 📚 C07 - Write It Down Before It's 'How We've Always Done It'

> 👥 **Group work** &nbsp;|&nbsp; 🗓️ **Day 2** · Story day T-5 &nbsp;|&nbsp; 🛠️ **Kiro:** chat, manual steering files &nbsp;|&nbsp; 📝 **Office:** Word

## 📖 Context

Monday, five working days to PI Planning. **Kim** wants to collect last week's decisions for the train, and can't find them. The wiki has **14 messy pages**: no owners, no dates, duplicates, an outdated playbook and two pages that contradict each other.

Worse: one decision from week one of the PI was **never written down** at all. "We don't estimate bugs" shows up as an open point in every team's sprint notes.

## 🎯 Your Goal

- Give the wiki a template and a tag list, so that decisions can be found again.
- Summarize your team's last week in one knowledge page. This is also your recap of Day 1.
- Write the missing decision record, and make sure it tells the whole story, not just one side.

## 📂 Your Inputs

| File | What's inside |
|---|---|
| `files/wiki-export.md` | The 14 pages of the train's wiki space |
| `files/bug-decision-notes.md` | What was said about estimating bugs in week one of the PI |
| `results/` (your folder) | Your results from C01 to C06. Something missing? Use the samples in the `solution` folders of C01 to C06 |

## ✅ Your Tasks

### 🗂️ Part 1 - Pages That Can Be Found

1. Add `wiki-export.md` to the chat and make sure Kiro **reads every page**:
   > 💬 *"Read all 14 pages. Don't skip a single word. List the decisions you find, with their page number, the pages that contradict each other, and the pages that are outdated or duplicates."*
2. Let Kiro design a **template with delimiters**:
   > 💬 *"Design a knowledge-page template that makes decisions easy to find. Mark each section with ### and put every fill-in instruction between <<< and >>>. Sections: metadata, summary, decisions, open questions, details, change log, sources, AI label and log. If a section has no source, the page says 'open'."*
3. **Save the template twice:**
   - as a **reusable prompt:** in the Kiro panel, open **Steering**, click **+**, name the file `knowledge-page-template`, put these three lines at the very top and paste the template below them:

     ```
     ---
     inclusion: manual
     ---
     ```
   - in **Word**: paste it, then **File → Save As → Word Template** as `C07-knowledge-page-template.dotx`, your version for SharePoint.
4. Let Kiro propose **tags and metadata**:
   > 💬 *"Propose metadata fields and at most 15 tags for this wiki. Then give each of the 14 pages a type, tags and a status, and say whether to keep, merge or archive it."*
5. **Write the recap of your week:** type `#knowledge-page-template` in the chat, add your `results` folder, then ask:
   > 💬 *"Fill in the template for one page: Team Signal, what we did and decided last week. Use only our results from C01 to C06."*

### ✍️ Part 2 - The Decision Nobody Wrote Down

1. Add `bug-decision-notes.md` and let Kiro draft the record with your template: `#knowledge-page-template` *"Write a decision record for 'we don't estimate bugs'. Version 1.0."*
2. Let Kiro play the **constructive critic**:
   > 💬 *"Act as an expert and critic in team decision-making. Criticize this decision record, convince me why it's weak, and tell me how to improve it. Look especially for one-sided reasoning and for voices that are missing."*
3. Let Kiro **self-refine**:
   > 💬 *"Use your feedback to write version 1.1. Use only facts from the notes; where something is unknown, write 'open'. Add a change log."*
4. **Check version 1.1.** Is anything in it that isn't in the notes? Delete it. The status stays **proposed**: Kim confirms the decision, not Kiro.
5. Add the AI label and a log line.

> 💡 **Tip:** A template in a steering file is a prompt you never have to type again. Kiro reads it only when you call it with `#`.

> 📚 **Kiro docs:** [Steering](https://kiro.dev/docs/steering/) explains manual inclusion and how to call a steering file with `#`.

## 📦 Deliverables

| Deliverable | Where it goes |
|---|---|
| `knowledge-page-template.md`: your template as a manual steering file | `.kiro/steering/`, where Kiro reads it |
| `C07-knowledge-page-template.dotx`: the Word template for SharePoint | Your results folder |
| `C07-tags.md`: metadata fields, tags and the sorted 14 pages | Your results folder |
| `C07-week-recap.md`: your team's week as a knowledge page, with **AI label** and **log line** | Your results folder |
| `C07-decision-record-bugs.md`: the decision record, version 1.1 with change log, **AI label** and **log line** | Your results folder |
| **One sentence** for the debrief: what did the critic find that you would have missed? | Debrief |

## 🗣️ Debrief

- Which two pages contradict each other, and what does that explain?
- Where did the three wrong numbers in C03's answer C probably come from?
- What did version 1.0 of the decision record leave out?

## 🔗 Where This Leads

In **C08 · The Number Sascha Will Actually Believe**, you forecast with data from Jira. The decision on bugs matters there: it changes what you can count.

> 📚 *A decision nobody wrote down gets made again and again. Kiro drafts the record in minutes; people make sure it's fair and complete.*
