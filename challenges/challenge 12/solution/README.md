# ✅ C12 - Nothing Ships in Isolation · Sample Solution

> 📘 **Sample solution** for Team Signal &nbsp;|&nbsp; 🤖 **Your results will look different:** AI answers vary from run to run. Compare the substance, not the wording.

## 🧭 How to Use This Solution

1. **Finish the challenge first.** The learning happens while you work with Kiro and Excel, not while you read a solution.
2. **Open the samples** and put them next to your own results.
3. **Compare:** Did you find the hidden dependencies? Did your reply to Charlie offer a deal, or just push back?

## 📂 Sample Results

| Deliverable | Sample |
|---|---|
| Program board, dependency list and risk register | [C12-program-board.xlsx](C12-program-board.xlsx) |
| Two-minute report for the ART Sync | [C12-art-sync-report.md](C12-art-sync-report.md) |
| Communication map | [C12-communication-map.md](C12-communication-map.md) |
| Reply to Charlie | [C12-escalation.md](C12-escalation.md) |

## 🎯 What a Good Result Looks Like

| Deliverable | Your result is good when … |
|---|---|
| **Program board** | All eleven dependencies are listed, and a formula marks late, missing, same-sprint and ok deliveries |
| **Risk register** | Excel calculates the scores; people set ROAM status and owners |
| **ART Sync report** | Two minutes: one top dependency, one top risk, a clear ask with names |
| **Communication map** | Who, with whom, about what, how and by when, plus the people to inform and the escalation steps |
| **Reply to Charlie** | It acknowledges your own part, proposes a deal with a clear cost, and escalates together, not against |

## 🗺️ Part 1: The Eleven Dependencies

| Status | Dependencies |
|---|---|
| 🔴 **Late** | Switch needs feed v2 in Sprint 1, delivered in Sprint 3 · Signal's alerting needs Depot's rules in Sprint 1, delivered in Sprint 3 · Signal's load test needs the peak-hour environment in Sprint 2, delivered in Sprint 3 |
| ⛔ **Missing** | Alert definitions for Depot: **no item at all** · test data from the provider · text templates and at-risk criteria from Rail Ops · the event-feed analysis for duplicate notifications |
| 🟡 **Same sprint** | Concourse's push notifications and Signal's platform-change events, both in Sprint 2 |
| 🟢 **OK** | Walking times use the station master data from last PI · release 3.3 after the pipeline update |

> 💡 **The hidden ones:** "Builds on the monitoring rules" and "possibly in the event feed" are dependencies too, even though nobody called them that. That's where *ensure all content is analyzed* pays off.

```
Status   =IF(G2="","missing",IF(G2>D2,"late",IF(G2=D2,"same sprint","ok")))
Score    =Probability*Impact
```

## 🛑 Part 3: From "No" to a Deal

| Weak reply | Strong reply |
|---|---|
| "DEP-P2 was agreed. Please stick to it." | "You have a point: we never sent our alert definitions." |
| "Otherwise we'll escalate to Kim." | "Let's take this to Kim **together**." |
| No offer | A clear deal: we do the work, you review for one hour |

> 💡 **Step back before you reply.** The step-back shows that Charlie's "no" has reasons: capacity, unclear ownership and a delivery Signal never made. A reply that ignores them escalates the conflict instead of solving it.

## 💡 What to Take Away

1. **Let Kiro read every word of every plan:** the most dangerous dependencies are the unwritten ones.
2. **Scores by formula, decisions by people:** Excel calculates the risk, people own it.
3. **Stress-test a difficult message** by letting Kiro read it as the person who receives it.

> 🔗 *Four plans became one board, and a "no" became a proposal. Tomorrow, Kim takes it to the steering committee.*
