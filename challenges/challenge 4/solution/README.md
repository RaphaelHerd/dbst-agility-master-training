# ✅ C04 - The AI Working Agreement · Sample Solution

> 📘 **Sample solution** for Team Signal &nbsp;|&nbsp; 🤖 **Your results will look different:** AI answers vary from run to run. Compare the substance, not the wording.

## 🧭 How to Use This Solution

1. **Finish the challenge first.** The learning happens while you work with Kiro, not while you read a solution.
2. **Put the samples next to your results:** the two cleaned exports and your agreement.
3. **Compare:** What did Kiro miss in your run? Which conflicts did you decide differently, and why?

## 📂 Sample Results

| Deliverable | Sample |
|---|---|
| Cleaned Jira export | [C04-jira-export-clean.csv](C04-jira-export-clean.csv) |
| Cleaned retro export | [C04-retro-export-clean.md](C04-retro-export-clean.md) |
| AI working agreement as a steering file | [ai-working-agreement.md](ai-working-agreement.md) |

> 💡 The agreement only works as a steering file in `.kiro/steering/`. Your Word version has the same content. A CSV file has no room for a label, so the sample's log line in the retro file covers both exports.

## 🎯 What a Good Result Looks Like

| Deliverable | Your result is good when … |
|---|---|
| **Cleaned exports** | No names, initials, @mentions or nicknames are left; no health details, private details or judgments about people; nothing shows who wrote what; and the facts the risk analysis needs are still there |
| **Agreement** | It fits on one page, covers all seven elements, settles every conflict from the thread, contains nothing your group didn't decide, and keeps the placeholders for your company's rules |
| **Steering file and Word version** | The steering file is in `.kiro/steering/`, and the Word version has the same content plus the AI label and a log line |

## ✂️ Part 1: What Kiro Typically Misses

| What | Example from the exports | Why it matters |
|---|---|---|
| Initials | "FR" (SWI-222), "AB" (retro note 4) | In a small team, initials point to one person |
| @mentions | "@klange" (SIG-147) | A handle is a name |
| Nicknames | "Tobi" (DEP-507) | A nickname is a name |
| Last names on their own | "Graf" (DEP-504) | Easy to overlook, and still a name |
| Short first names | "Jo" (retro note 3), "Nina" (retro note 6) | Short names often slip through |
| Health details next to a pseudonym | "was off sick" (SIG-145), "back problems" (CON-314), retro note 9 | Health data stays health data, even when the name is gone |
| Private details | "parental leave" (CON-305) | The task only needs "absent from next month" |
| Judgments | "takes far too long with everything" (SWI-222) | A judgment about a person has no place in a prompt, with or without a name |
| Who wrote what | The author column, even with pseudonyms | It allows exactly the person-level analysis that is off limits |

> 💡 **Keep the fact, drop the reason.** "Nobody is testing it this week" is all the risk analysis needs. Why someone is absent is nobody's business.

> 💡 **Pseudonyms are the minimum.** When a task doesn't need people at all, as here, leave them out completely. That's why the sample contains no pseudonyms.

## 🤝 Part 2: Three Viewpoints, One Agreement

### 👀 The Viewpoints

| | 🎯 PO (Alex) | 💻 Dev lead (Member A) | 🛡️ Works council (Robin) |
|---|---|---|---|
| **Wants** | Speed: Kiro drafts backlog items and the status updates for Kim | Freedom: each developer decides how to use Kiro | Protection: no personal data, no analysis of individuals, transparency, a named reviewer |
| **Fears** | Bureaucracy: full reviews and labels everywhere | Surveillance: logged prompts and chats | AI used to judge people, and AI use that nobody can see |
| **Common ground** | Robin asks for a named reviewer only when a result leaves the team, so internal drafts stay quick | Robin also rules out using AI to judge individuals | Member A also rules out using Kiro to judge individuals |

### ⚔️ The Two Biggest Conflicts, and How the Sample Decides

| Conflict | Sample decision |
|---|---|
| **Traceability vs. no logging:** Kim wants AI use to be traceable; Member A wants no logging of prompts | **Log results, not people:** one log line per released result, no recording of chats, and the log is never used to evaluate anyone |
| **Speed vs. control:** Alex wants a quick look by the author; Robin wants a named person to check | **The destination decides:** drafts that stay in the team are checked by the author; everything that leaves the team gets a named reviewer |

### ❓ Ask Before Answering: Kiro's Questions and the Group's Answers

| Kiro asked | The group decided |
|---|---|
| What counts as "leaving the team"? | Anything another team, a stakeholder or Rail Ops reads, and anything that feeds a decision |
| Who reviews results that leave the team? | A named person, usually the one who shares the result |
| Where is the log kept? | As a log line in the result itself, not in a separate tool |
| Do chat messages need an AI label? | No, only results that leave the team |
| How often do you review the agreement, and how is the works council involved? | In every second Retro; changes go to the works council before they take effect |

## 💡 What to Take Away

1. **Clean first, prompt second.** Data you delete before the prompt can't leak.
2. **Pseudonymizing is not the finish line.** Check what's left: initials, handles, health hints, judgments.
3. **Kiro finds common ground; people settle conflicts.** An agreement nobody decided is an agreement nobody keeps.

> 🤝 *Your agreement is now a steering file. From here on, Kiro knows your rules, and so does everyone who reads your results.*
