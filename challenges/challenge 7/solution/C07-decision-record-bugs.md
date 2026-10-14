# 🐞 C07 - Decision Record: No Story Points for Bugs · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

### METADATA
- **Title:** Decision: no story points for bugs
- **Type:** decision
- **Team:** ART
- **Tags:** estimation, pi-planning
- **Owner:** Release Train Engineer
- **Status:** proposed, waiting for Kim's confirmation
- **Version:** 1.1 · **Last reviewed:** T-5

### SUMMARY
In week one of the PI, the train agreed in the ART channel to stop estimating bugs in story points. One PO agreed only on a condition that was never written down: the time bugs take must stay visible for capacity planning.

### DECISIONS
| What | Who decided | When | Valid until |
|---|---|---|---|
| Bugs get no story points | Kim, after a poll in the ART channel | Week one of the current PI | open: no review date set |

### OPEN QUESTIONS
| Question | Who answers | By when |
|---|---|---|
| How does the time bugs take stay visible, as Charlie asked? | Kim with the POs | open |
| Do teams reserve capacity for bugs, for example the 15 % Team Signal mentioned? | Each team | open |
| Do Team Concourse and Finance agree? Neither took part in the poll | Kim | open |
| When is the decision reviewed? | Kim | open |

### DETAILS
- **Context:** planning took too long, and the effort for bugs varies a lot.
- **Reasons given:** bugs are hard to estimate; some take ten minutes, others three days. Points for bugs inflate velocity.
- **Condition:** Charlie (PO, Depot) agreed only as long as the time bugs take stays visible.
- **Consequences:** velocity in story points no longer includes bug work, so plans based on points alone overstate the capacity for new features. Forecasts need another measure that includes bugs, for example the number of items finished.
- **Voices in the poll:** Member A (Signal), Member B (Switch), Sam (PO, Switch), Charlie (PO, Depot) and Kim. **Not heard:** Team Concourse, testers and Finance.

### CHANGE LOG
| Version | Change |
|---|---|
| 1.0 | AI draft from the chat notes: decision and reasons only |
| 1.1 | After the critic's review: Charlie's condition, consequences for planning and forecasts, missing voices and open questions added; status set to "proposed" |

### SOURCES
`bug-decision-notes.md`

### AI LABEL AND LOG
> 📝 **Log:** prompts "#knowledge-page-template Write a decision record…", "Act as an expert and critic…", "Use your feedback to write version 1.1…" · sources: `bug-decision-notes.md` · version 1.1 · reviewer: Agility Master, Team Signal
