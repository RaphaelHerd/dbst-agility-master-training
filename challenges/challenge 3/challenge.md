# 🔍 C03 - The Near-Miss

> 👥 **Group work** &nbsp;|&nbsp; 🗓️ **Day 1** · Story day T-9 &nbsp;|&nbsp; 🛠️ **Kiro:** chat, files as context

## 📖 Context

Yesterday evening, an Agility Master on the train almost sent this message to all teams:

> 💬 *"Heads-up: SAFe makes it mandatory to rank all stories by WSJF and submit them to the RTE ten working days before PI Planning. That's today!"*

A colleague stopped it just in time. The source was an AI answer. It sounded convincing, and <span style="color:#EC0016;font-weight:700">it was wrong</span>.

**Kim** has collected three AI answers that are now circulating on the train. Before anyone acts on them, Kim wants every claim checked against the **PI Planning Playbook**. And there is a second job: someone asked an AI to merge your team's Definition of Done with the ART-wide minimum and polish the wording for the PI Planning page. Nobody has checked the result yet.

## 🎯 Your Goal

- Check every claim in three AI answers against the source, and give each claim a verdict.
- Find the steps in your team's Definition of Done that nobody ever agreed on, and what went missing.

## 📂 Your Inputs

| File | What's inside |
|---|---|
| `files/ai-answers/answer-a.md`, `answer-b.md`, `answer-c.md` | Three AI answers about PI Planning. Answer B is the near-miss |
| `files/sources/art-playbook.md` | The PI Planning Playbook: the train's single source of truth |
| `files/dod-agreed.md` | Your team's Definition of Done, as agreed in a Retrospective |
| `files/dod-polished.md` | The AI-polished version for the PI Planning page |

## ✅ Your Tasks

### 🔍 Part 1 - Check Every Claim

1. Add `art-playbook.md` and `answer-b.md` to the chat (type `#` and choose **File**). Start with answer B: it almost went out.
2. **Ground Kiro in the source** with "according to":
   > 💬 *"According to art-playbook.md only, check every claim in answer-b.md. For each claim, quote the passage that confirms or contradicts it. If the playbook says nothing about a claim, write 'not in the source'."*
3. **Ask how sure Kiro is:**
   > 💬 *"How sure are you about each verdict, from 1 (guess) to 5 (certain), and why?"*

   The rating is a hint, not proof. **Look up every quote in the playbook yourself.**
4. Check answers A and C the same way, and ask for a **deep analysis**:
   > 💬 *"This is a complex task, so take your time. Read every word of the playbook first. Then check answer C claim by claim, with special attention to numbers and dates."*
5. Write your **validation log**: one row per claim, with a verdict and the source.

   | Verdict | Meaning |
   |---|---|
   | ✅ Confirmed | The playbook says so |
   | ❓ Unconfirmed | The playbook says nothing about it |
   | ❌ Wrong | The playbook says something different |

### 🧾 Part 2 - Find the Invented Steps

1. Open a **new chat** and add `dod-agreed.md`, `dod-polished.md` and `art-playbook.md`. Section 3 of the playbook holds the ART-wide minimum.
2. Let Kiro **compare all three line by line**:
   > 💬 *"Compare dod-polished.md line by line with dod-agreed.md and section 3 of art-playbook.md. For each line of the polished version, name its source and quote it. Mark every line that has no source. Then list everything from the two sources that is missing or weaker in the polished version. Don't skip a single line."*
3. **Check Kiro's table yourself.** Is every quote really in the file?
4. Write the **corrected Definition of Done**: everything from your team DoD and the ART minimum, and nothing else. Add the AI label and a log line.

> 💡 **Tip:** AI doesn't only add things. It also drops and softens them. Compare in both directions.

> 📚 **Kiro docs:** [Chat](https://kiro.dev/docs/ide/chat/) shows how to add single files as context.

## 📦 Deliverables

| Deliverable | Where it goes |
|---|---|
| `C03-validation-log.md`: every claim of the three answers with verdict and source, with **AI label** and **log line** | Your results folder |
| `C03-corrected-dod.md`: your line-by-line check and the corrected Definition of Done, with **AI label** and **log line** | Your results folder |
| **One sentence** for the debrief: which claim would you have believed without the check? | Debrief |

## 🗣️ Debrief

- Which claim sounded most convincing, and why?
- Did Kiro's "how sure" ratings match what you found in the source?
- What did the AI invent in your Definition of Done, and what did it drop or soften?

## 🔗 Where This Leads

Today you caught the errors after they happened. In **C04 · The AI Working Agreement**, you write the rules that stop them before they reach anyone.

> 🔍 *A precise-looking answer is not a correct answer. Ground it in the source, check it yourself, and only then share it.*
