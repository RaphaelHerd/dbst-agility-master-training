# 🔗 C12 - Nothing Ships in Isolation

> 👥 **Group work**, with an ART Sync round for all groups &nbsp;|&nbsp; 🗓️ **Day 2** · Story day T-2 &nbsp;|&nbsp; 🛠️ **Kiro:** chat, files as context &nbsp;|&nbsp; 📊 **Office:** Excel

## 📖 Context

All four teams have sent their draft PI backlogs, and **Kim** has merged them into one file. Before the **ART Sync at 15:00**, Kim wants to know what depends on what, where a delivery comes too late, and what the biggest risks are.

Right after the ART Sync, **Charlie**, the PO of Team Depot, writes: *"We can't commit to the monitoring rules for your delay feed. Please take it off our list."*

## 🎯 Your Goal

- Find every dependency between the teams, including the ones nobody wrote down.
- Build the program board and a risk register, and report in two minutes.
- Answer a team that backs out of its commitment, with a proposal that holds up.

## 📂 Your Inputs

| File | What's inside |
|---|---|
| `files/kim-request.md` | What Kim needs before the ART Sync |
| `files/train-backlog.csv` | The draft PI backlogs of all four teams, with the planned sprint |
| `files/charlie-dispute.md` | Charlie's mail after the ART Sync |
| `files/wiki-alerting.md` | Two wiki pages about alerting |

## ✅ Your Tasks

You write every prompt yourselves. The steps say what each prompt must achieve, not how to phrase it.

### 🗺️ Part 1 - What Depends on What

1. Add `kim-request.md` and `train-backlog.csv` to the chat and make sure Kiro **reads every item, every word**. Your prompt should ask for:
   - every dependency between teams, including the ones **only hinted at** in a description, and dependencies on people outside the train;
   - for each one: who needs what from whom, by which sprint, and in which sprint it is delivered;
   - a mark on every need that **no item delivers**.
2. Build the **program board** in Excel: teams in rows, sprints in columns. Add a dependency list where a formula marks each dependency as *ok*, *same sprint*, *late* or *missing*.
3. Build the **risk register**: let Kiro propose risks with a probability and an impact from 1 to 3. Excel calculates the score. **You** set the ROAM status and the owner.
4. Prepare your **two-minute report** for the ART Sync: spoken language, **at most 150 words**, with your top dependency, your top risk and what you need from whom.

   All groups present in one ART Sync round. Did everyone find the same top risk?

### 📞 Part 2 - Who Needs to Talk to Whom

1. For your **top dependency**, let Kiro map the communication paths: who needs to talk to whom, about what, how and by when. Include the people who **only need to be informed**, and the **next step** if they can't agree.

### 🛑 Part 3 - "Take It Off Our List"

1. Add `charlie-dispute.md` and `wiki-alerting.md`. Before you answer, **step back**: let Kiro think about what could be behind Charlie's message. Point it to capacity, ownership and **what your team hasn't delivered** itself.
2. Let Kiro draft your **escalation and mitigation message** to Charlie. It proposes a solution, says what it costs Team Depot, and names the next step if you can't agree. Respectful, **at most 200 words**.
3. **Stress-test it** with role prompting and self-refine: let Kiro read the message **as Charlie**, say what would make Charlie say no, and then improve the message.
4. Add the AI label and a log line. A person sends it, or decides not to.

> 💡 **Tip:** The most dangerous dependency is the one that no item delivers. Look for needs without a supplier.

> 💡 **Tip:** The solution shows sample prompts. Open it only after you have tried your own.

> 📚 **Kiro docs:** [Chat](https://kiro.dev/docs/ide/chat/) covers adding files as context.

## 📦 Deliverables

| Deliverable | Where it goes |
|---|---|
| `C12-program-board.xlsx`: program board, dependency list and risk register | Your results folder |
| `C12-art-sync-report.md`: your two-minute report | Your results folder |
| `C12-communication-map.md`: who talks to whom about your top dependency | Your results folder |
| `C12-escalation.md`: your reply to Charlie, with **AI label** and **log line** | Your results folder |
| **One sentence** for the debrief: which dependency did nobody write down? | Debrief |

## 🗣️ Debrief

- Which dependencies did Kiro find only in the descriptions?
- Which risk would you raise first at PI Planning?
- What changed in your message after Kiro read it as Charlie?
- Which words in your prompt made Kiro find the dependencies that were only hinted at?

## 🔗 Where This Leads

In **C13 · The PI Readiness Pack**, everything comes together: tomorrow, Kim presents the train's readiness to the steering committee.

> 🔗 *Kiro finds the links between four plans in seconds. Turning a "no" into an agreement takes people who talk to each other.*
