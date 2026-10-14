# ✅ C05 - One Sprint, Three Very Different Readers · Sample Solution

> 📘 **Sample solution** for Team Signal &nbsp;|&nbsp; 🤖 **Your results will look different:** AI answers vary from run to run. Compare the substance, not the wording.

## 🧭 How to Use This Solution

1. **Finish the challenge first.** The learning happens while you work with Kiro, not while you read a solution.
2. **Open the samples** and put them next to your drafts.
3. **Compare:** Do your numbers match? Did each draft keep to its reader's rules? Which check in your review gate caught something?

## 📂 Sample Results

| Deliverable | Sample |
|---|---|
| Team update | [C05-team-update.md](C05-team-update.md) |
| Decision paper | [C05-decision-paper.md](C05-decision-paper.md) |
| Note for Rail Ops | [C05-rail-ops-note.md](C05-rail-ops-note.md) |
| Review checklist as a manual steering file | [review-checklist.md](review-checklist.md) |

> 💡 The decision paper is shown as Markdown; your Word version has the same content. All samples carry **version 1.1**, because they were fixed after the review gate.

## 🎯 What a Good Result Looks Like

| Deliverable | Your result is good when … |
|---|---|
| **Team update** | It has at most 120 words: done, open, next. The numbers match the sprint notes, and the Jira mismatch is addressed |
| **Decision paper** | The decision comes first, each option shows its consequence, the recommendation is clearly the PO's, and there are no ticket IDs |
| **Note for Rail Ops** | It has at most 100 words in plain language, with no ticket IDs, system names, people's names or jargon, and a clear ask, even if the ask is "nothing at the moment" |
| **Review checklist** | It has at most 10 pass-or-fail checks derived from your agreement, saved with `inclusion: manual` |
| **All three drafts** | Each one passed your review gate and carries the AI label and a log line |
| **Your prompts** | One prompt per reader, each with a role, a tone, a skeleton and what to leave out; the decision paper starts with the skeleton only |

## 💬 Sample Prompts

Prompts like these worked well. Yours don't need the same words; compare what they ask for.

| Step | Sample prompt | Why it works |
|---|---|---|
| **Facts first** | *"Read every line of sprint-notes.md and jira-export.csv. Summarize Sprint 14 as a fact list: goal, items with status, numbers and blockers. Mark every place where the two files disagree."* | One checked fact list feeds all three drafts, and the mismatch in Jira surfaces before anyone writes |
| **Team update** | *"You are the Agility Master of Team Signal, writing to your own team. Turn our checked fact list into a status update for the team channel: done, open, next. Friendly and direct, at most 120 words, with item IDs."* | Role, tone, skeleton and length in one prompt |
| **Decision paper** | *"You write for a steering committee that has five minutes for this topic. First, give me only the skeleton of a one-page decision paper based on decision-needed.md. Wait for my OK before you fill it in."* | Skeleton-of-thought: you approve the structure before Kiro writes a word |
| **Rail Ops note** | *"You write for Rail Ops shift leads in plain language. Write a note of at most 100 words: what changes for you, what we need from you. No ticket IDs, no internal system names, no people's names, no jargon."* | The exclusions are spelled out, so Kiro can't fall back on team language |
| **Review checklist** | *"Turn our AI working agreement into a review checklist for drafts that leave the team: at most 10 checks, each one answerable with pass or fail."* | Pass or fail makes every check usable as a gate |

## 🔍 Part 1: The Trap in Your Jira Export

Jira marks **SIG-150** as **Done**, but the sprint notes say it is only partly done: 3 of 7 tests are stable.

| | Jira says | Really |
|---|---|---|
| **Items done** | 5 of 7 | 4 of 7 |
| **Story points done** | 18 of 26 | 18 of 26 |

If your update says "5 of 7", Kiro trusted Jira. When two sources disagree, ask the team and fix the source. The story points don't show the mismatch: SIG-150 is a bug, and bugs carry no points because of the decision from week one not to estimate bugs. Let Excel do the sums.

## ✍️ Part 1: Same Facts, Three Texts

| | 👥 Team | 🏛️ Steering committee | 🚉 Rail Ops |
|---|---|---|---|
| **Opens with** | The sprint goal | The decision needed | What's new for them |
| **22 seconds** | Against the sprint goal: below 30 | Against the PI target: 15 | In plain words: "within 22 seconds" |
| **Ticket IDs** | Yes | No | No |
| **Asks for** | An owner for the test-data request | A decision | Nothing at the moment |

## 🚦 Part 2: The Review Gate in Action

An example: a first draft of the note for Rail Ops, run through `#review-checklist`.

> *"Hi Rail Ops team! Great news: SIG-142 is done, so platform-change events now work for 5 pilot stations. Our new stream processor brings the latency of delay feed v2 down to 22 seconds, so your one-minute requirement is already met. Alex and Member C will roll this out soon, and we'll let you know before anything goes live."*

| Check | Result | Evidence | Fix |
|---|---|---|---|
| 1 · Facts | ❌ Fail | "your one-minute requirement is already met" | Delete: the requirement is about platform changes, and the 22 seconds are about delay information in test |
| 2 · Numbers | ✅ Pass | "5 pilot stations", "22 seconds" | None |
| 3 · Open stays open | ❌ Fail | "will roll this out soon", "we'll let you know before anything goes live" | Delete: nobody has agreed on this |
| 4 · Personal data | ✅ Pass | Only a pseudonym and the PO's first name | None |
| 5 · Reader rules | ❌ Fail | "SIG-142", "stream processor", "latency", "delay feed v2", "Alex and Member C" | Remove IDs and names, use plain words |
| 6 · Format and tone | ✅ Pass | Under 100 words | None |
| 7 · Fairness | ✅ Pass | No blame | None |
| 8 · Label | ❌ Fail | Missing | Add the label |
| 9 · Log | ❌ Fail | Missing | Add the log line |

Compare this with the [final note](C05-rail-ops-note.md). The checklist found the problems; a person decided how to fix them.

## ⚖️ A Fairness Question Worth Asking

Option B in your decision paper, going live without the load test, shifts a risk onto people who are not in the room: Team Switch, whose transfer calculations use the feed, and passengers at peak hours. The sample paper names them in a short section. That is the fairness check from your agreement at work: **who is affected but not in the room?**

## 💡 What to Take Away

1. **Facts first, texts second:** one checked fact list feeds all three drafts.
2. **Role, tone, skeleton and exclusions** turn the same facts into the right text for each reader.
3. **A checklist saved as a manual steering file** makes your review gate reusable, and the decision stays with you.

> 📣 *Your review gate is now a tool you can call at any time. Use it whenever something leaves the team.*
