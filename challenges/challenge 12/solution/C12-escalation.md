# 🛑 C12 - Reply to Charlie · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

## 🔭 Step Back First

| What might be behind it | Evidence |
|---|---|
| **Capacity:** Depot is overloaded | Around 40 % of its capacity goes to ad-hoc requests |
| **Ownership is unclear** | Wiki page 10 says Depot defines alert rules; page 11 says Depot waits for Signal |
| **We didn't deliver our part** | No item on our board delivers the alert definitions |

So Charlie's "no" is not stubbornness. It's a reasonable reaction to an unclear deal.

## ✉️ The Message, Version 1.1

**Subject:** Alerting for the delay feed: a proposal

Hi Charlie,

Thanks for being direct. You have a point: we never sent you our alert definitions, so you couldn't start. And our wiki says two different things about who defines alerts.

Our proposal:

1. We deliver the alert definitions in Sprint 1.
2. We build the monitoring rules ourselves in Sprint 2. One of your site reliability engineers reviews them in a one-hour session, so they fit your platform. DEP-P2 comes off your list.
3. For the first two weeks, our team handles the new alerts. After that, they join the normal on-call rotation, if you agree.

What it costs you: one hour of review instead of a full item.

Who owns alert rules on the train is still open. Let's take this proposal to Kim together in tomorrow's ART Sync, so the wiki says one thing from now on.

Best regards,
Agility Master, Team Signal

## 🧪 What the Stress Test Changed

Kiro read version 1.0 as Charlie and named three reasons to say no:

| Charlie's objection | Change in version 1.1 |
|---|---|
| "A joint session still costs us capacity we don't have" | Signal does the work; Depot only reviews for one hour |
| "And who answers the new alerts at night?" | Signal handles them for the first two weeks |
| "Going to Kim sounds like a threat" | "Let's take this to Kim **together**" |

> 📝 **Log:** prompts "Before we reply, step back…", "Write a reply to Charlie…", "Read the message as Charlie. What would make you say no? Then improve the message." · sources: `charlie-dispute.md`, `wiki-alerting.md`, `C12-program-board.xlsx` · version 1.1 · reviewer: Agility Master, Team Signal
