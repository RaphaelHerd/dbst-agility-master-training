# ✅ C03 - The Near-Miss · Sample Solution

> 📘 **Sample solution** for Team Signal &nbsp;|&nbsp; 🤖 **Your results will look different:** AI answers vary from run to run. Compare the substance, not the wording.

## 🧭 How to Use This Solution

1. **Finish the challenge first.** The learning happens while you work with Kiro, not while you read a solution.
2. **Put the samples next to your results:** the validation log and your corrected Definition of Done.
3. **Compare:** Did every claim get a verdict? Did you find both invented steps, and the points that went missing or got weaker?

## 📂 Sample Results

| Part | Sample |
|---|---|
| Part 1: validation log | [C03-validation-log.md](C03-validation-log.md) |
| Part 2: corrected Definition of Done | [C03-corrected-dod.md](C03-corrected-dod.md) |

## 🎯 What a Good Result Looks Like

| Deliverable | Your result is good when … |
|---|---|
| **Validation log** | Every claim has a verdict and a source, and "the playbook says nothing about it" is marked ❓, not ❌. The sample splits the answers into 17 claims; your split may differ |
| **Corrected DoD** | Every line traces back to your team DoD or the ART minimum, both invented steps are gone, and the softened and the dropped point are back in their original wording |
| **Your prompts** | They name the playbook as the only source, ask for a quote per claim or line, say what to do when the source is silent, and check in both directions |
| **Label and log** | Both files show the AI label and a log line |

## 💬 Sample Prompts

Prompts like these worked well. Yours don't need the same words; compare what they ask for.

| Step | Sample prompt | Why it works |
|---|---|---|
| **Grounding** | *"According to art-playbook.md only, check every claim in answer-b.md. For each claim, quote the passage that confirms or contradicts it. If the playbook says nothing about a claim, write 'not in the source'."* | One source, a quote as proof, and a way out for claims the source doesn't cover, so Kiro doesn't have to guess |
| **How sure** | *"How sure are you about each verdict, from 1 (guess) to 5 (certain), and why?"* | Shows where to look first; the "why" reveals weak reasoning |
| **Deep analysis** | *"This is a complex task, so take your time. Read every word of the playbook first. Then check answer C claim by claim, with special attention to numbers and dates."* | Slows Kiro down and points it at the spots where errors hide |
| **Line by line** | *"Compare dod-polished.md line by line with dod-agreed.md and section 3 of art-playbook.md. For each line of the polished version, name its source and quote it. Mark every line that has no source. Then list everything from the two sources that is missing or weaker in the polished version. Don't skip a single line."* | Checks in both directions: what was added and what went missing |

## 🔍 Part 1: The Three Answers at a Glance

| Answer | ✅ | ❓ | ❌ | What makes it tricky |
|---|---|---|---|---|
| **A** | 4 | 1 | 0 | Almost everything is right. One detail, the 10-minute slot, is in no source |
| **B** | 1 | 1 | 3 | The near-miss: a precise-looking reference, the word "mandatory" and one correct claim make three wrong rules sound convincing |
| **C** | 4 | 0 | 3 | The structure is right, but the numbers are wrong: 3 instead of 5 working days, the top 15 instead of the top 10 features, three days instead of two |

### 📣 What Should Have Gone Out Instead

> *"Quick check on yesterday's AI tip: our playbook has no rule that teams rank their stories by WSJF or submit anything ten days before PI Planning. Product Management shares the top 10 features five working days before. Please check your team's capacity before the event. Source: PI Planning Playbook, sections 1 and 2."*

### 🎚️ Did "How Sure Are You?" Help?

AI models can sound just as sure when they are wrong as when they are right. Use the rating as a hint where to look first, never as proof. **The quote from the source is the proof.**

## 🧾 Part 2: Four Ways the AI Changed Your Definition of Done

| What the AI did | Line | How it happened |
|---|---|---|
| ❌ **Invented a step from a current problem** | "Every story is load-tested with peak-hour data before release." | The open load test (SIG-145) turned into a rule. With test data arriving late, no story could ever be done |
| ❌ **Invented a best-practice number** | "Unit test coverage is at least 80 %." | A generic number that sounds professional, but nobody agreed on it |
| ⚠️ **Softened a point** | "Documentation is updated where needed." | "documented in the team wiki" became optional |
| ⚠️ **Dropped a mandatory point** | "Acceptance criteria are met and accepted by the Product Owner." | An ART-wide minimum point disappeared, although teams can't remove these |

> ⚠️ None of the four changes looks wrong at first sight. That's why the line-by-line check needs both directions: what was added, and what went missing.

## 💡 What to Take Away

1. **Ground every check in a source:** "according to …", with a quote you have looked up yourself.
2. **Numbers, dates and references** are where AI errors like to hide.
3. **AI drops and softens, too.** Compare in both directions: what was added, and what went missing.

> 🔍 *The near-miss was stopped by a person who checked. From today, that person is you.*
