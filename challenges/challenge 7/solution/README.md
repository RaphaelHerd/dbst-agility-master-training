# ✅ C07 - Write It Down Before It's 'How We've Always Done It' · Sample Solution

> 📘 **Sample solution** for Team Signal &nbsp;|&nbsp; 🤖 **Your results will look different:** AI answers vary from run to run. Compare the substance, not the wording.

## 🧭 How to Use This Solution

1. **Finish the challenge first.** The learning happens while you work with Kiro, not while you read a solution.
2. **Open the samples** and put them next to your own results.
3. **Compare:** Does your template make decisions easy to find? Did your decision record tell the whole story?

## 📂 Sample Results

| Deliverable | Sample |
|---|---|
| Template as a manual steering file | [knowledge-page-template.md](knowledge-page-template.md) |
| Tags, metadata and the sorted 14 pages | [C07-tags.md](C07-tags.md) |
| Your week as a knowledge page | [C07-week-recap.md](C07-week-recap.md) |
| Decision record, version 1.1 | [C07-decision-record-bugs.md](C07-decision-record-bugs.md) |

> 💡 The template only works as a steering file in `.kiro/steering/`. The three lines at the top are required: they tell Kiro to load the file only when you call `#knowledge-page-template`. Your Word template has the same sections.

## 🎯 What a Good Result Looks Like

| Deliverable | Your result is good when … |
|---|---|
| **Template** | Clear sections marked with delimiters, fill-in instructions, a decisions section with who and when, and the rule "write 'open' when there is no source" |
| **Tags** | A short list (at most 15), one way of writing them, and every one of the 14 pages sorted with a recommendation |
| **Week recap** | It uses your template, names decisions with who and when, and invents nothing that isn't in your results |
| **Decision record** | Version 1.1 names the condition, the consequences and the missing voices; the status is "proposed", not "approved" |
| **Your prompts** | The reading prompt demands every page, the template prompt fixes delimiters and sections, and the critic prompt names what to look for |

## 💬 Sample Prompts

Prompts like these worked well. Yours don't need the same words; compare what they ask for.

| Step | Sample prompt | Why it works |
|---|---|---|
| **Read every page** | *"Read all 14 pages. Don't skip a single word. List the decisions you find, with their page number, the pages that contradict each other, and the pages that are outdated or duplicates."* | Forces a complete read and asks for three concrete lists |
| **Template** | *"Design a knowledge-page template that makes decisions easy to find. Mark each section with ### and put every fill-in instruction between <<< and >>>. Sections: metadata, summary, decisions, open questions, details, change log, sources, AI label and log. If a section has no source, the page says 'open'."* | Delimiters separate structure from instructions; the "open" rule stops invented content |
| **Tags** | *"Propose metadata fields and at most 15 tags for this wiki. Then give each of the 14 pages a type, tags and a status, and say whether to keep, merge or archive it."* | A limit keeps the tag list usable; applying it to all 14 pages tests it at once |
| **Week recap** | *"#knowledge-page-template Fill in the template for one page: Team Signal, what we did and decided last week. Use only our results from C01 to C06."* | The template from the steering file plus a strict source |
| **Decision record** | *"#knowledge-page-template Write a decision record for 'we don't estimate bugs'. Version 1.0."* | Same template, so the record looks like every other page |
| **Constructive critic** | *"Act as an expert and critic in team decision-making. Criticize this decision record, convince me why it's weak, and tell me how to improve it. Look especially for one-sided reasoning and for voices that are missing."* | Telling Kiro where to look gets a sharper critique than "improve this" |
| **Self-refine** | *"Use your feedback to write version 1.1. Use only facts from the notes; where something is unknown, write 'open'. Add a change log."* | Refines without inventing, and documents what changed |

## 🗂️ Part 1: What the 14 Pages Reveal

| Finding | Why it matters |
|---|---|
| **Pages 10 and 11 contradict each other** about who defines the alerts | That's the root of the deadlock between Signal and Depot |
| **Page 5 is the old playbook,** with three days, the top 15 and three working days | All three wrong numbers in C03's answer C are on this page. Outdated pages feed AI answers, too |
| **Page 2 holds three decisions** without date or owner, one with a question mark | A decision without who and when can't be found and can't be trusted |
| **Pages 7 and 8 are duplicates** | Two versions of the truth, one of them always outdated |

> 💡 Did Kiro find all of this on the first try? *Ensure all content is analyzed* ("don't skip a single word") makes it more likely, but only your check makes it certain.

## ✍️ Part 2: What the Critic Found

**Version 1.0** typically reads like this: *"The train decided not to estimate bugs, because bugs are hard to estimate and inflate velocity. This saves planning time."* It sounds complete. It isn't.

| The critic's finding | What changed in version 1.1 |
|---|---|
| **One-sided:** only the arguments in favor | The condition and the consequences are added |
| **A condition went missing:** Charlie agreed only if the time bugs take stays visible | Named in the summary and as an open question |
| **Consequences for planning are missing** | Plans in story points now overstate the capacity for features; forecasts need another measure |
| **Voices are missing:** Concourse, testers and Finance were not in the poll | Listed under "not heard" |
| **No review date, no owner** | Owner: the Release Train Engineer; review date marked "open" |

> ⚠️ **Watch the self-refine step.** When Kiro improves its own text, it likes to fill gaps: *"approved by the steering committee"*, *"review after one PI"*. If the notes don't say it, it says "open".

## 💡 What to Take Away

1. **A template in a manual steering file** is a prompt you never have to type again.
2. **Critic, then self-refine:** ask Kiro to attack its own draft before you trust it.
3. **Version and label decisions,** and leave the final "yes" to the person who owns them.

> 📚 *The bug decision is written down at last. Next, you'll see why it matters for counting.*
