# ⚙️ C09 - Automation Design: Escalate Long-Blocked Stories · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

## 1️⃣ The Request, and What Would Go Wrong

Alex asked: *"Every time a story gets blocked, immediately notify Kim and post it in the ART channel."* Run exactly like that, the rule would:

- send a message for every short block, even one that is solved within an hour;
- send the same story again and again whenever it is blocked anew;
- bypass Alex as PO and go straight to Kim and a large channel;
- create a public list that invites people to compare teams.

## 2️⃣ The Rule, With Brakes

| Part | Design |
|---|---|
| **Name** | Escalate long-blocked Signal stories |
| **Trigger** | Scheduled, every working day at 09:00 |
| **Condition (JQL)** | `project = SIG AND issuetype = Story AND status = Blocked AND status CHANGED TO Blocked BEFORE -2d AND (labels is EMPTY OR labels != escalated)` |
| **Actions** | 1. Comment on the story: *"Blocked for more than two days. What do you need to move on?"* · 2. Notify the PO · 3. Add the label `escalated` |
| **Not automatic** | No message to Kim and no post in the ART channel. Escalated stories appear in the ART Sync through the filter `labels = escalated` |

**The brakes:**
- 🕑 **Two days of patience:** short blocks never trigger the rule.
- 🏷️ **Once only:** the label `escalated` stops repeat messages.
- 🪜 **Escalation ladder:** the PO first, the ART Sync second.
- 🎯 **Small start:** one team only, after a test in the sandbox.

> 💡 **Why `labels is EMPTY OR …`?** In JQL, `labels != escalated` does not find issues without any label. Without the extra condition, the rule would miss exactly the stories with no labels.

## 3️⃣ Change Request

| Field | Content |
|---|---|
| **What** | New automation rule "Escalate long-blocked Signal stories", as designed above |
| **Why** | SIG-145 and SIG-147 were blocked for weeks before anyone outside the team noticed |
| **Risk** | Too many notifications; misuse of the escalation list to compare teams |
| **Switch-off** | Disable the rule in Jira Automation; remove the label `escalated` |
| **Rule owner** | Agility Master, Team Signal |
| **Approval** | **Open:** Kim (RTE) and the Jira administrator in Team Depot |

## 4️⃣ Test Plan in the Sandbox

| # | Test story | Expected result |
|---|---|---|
| 1 | Blocked three days ago, no labels | Comment, PO notified, label `escalated` added |
| 2 | Blocked yesterday | Nothing happens |
| 3 | Blocked three days ago, label `escalated` already set | Nothing happens |

## 5️⃣ How This Rule Must Never Be Used

The escalations show **where work is stuck**, not who is to blame. The rule's audit log and the label `escalated` must not be used to compare teams or to evaluate the people working on the stories. The comment names no person.

## 6️⃣ Log

| Date | Rule | Version | Approver |
|---|---|---|---|
| open | Escalate long-blocked Signal stories | 1.0 | open |

Review four weeks after go-live: does the rule still do what it should?

> 📝 **Log:** prompt chain "Design a Jira automation rule…" → "Turn this rule into a change request…" → "Write a test plan…" → "Add a warning…" · sources: `alex-request.md`, `change-process.md` · version 1.0 · reviewer: Agility Master, Team Signal
