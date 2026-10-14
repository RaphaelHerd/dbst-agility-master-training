# 🔍 C03 - Validation Log · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

**Source:** `art-playbook.md`, the PI Planning Playbook, version 2.1

| Verdict | Meaning |
|---|---|
| ✅ Confirmed | The playbook says so |
| ❓ Unconfirmed | The playbook says nothing about it |
| ❌ Wrong | The playbook says something different |

## 🤖 Answer A · "How does PI Planning work on our train?"

| # | Claim | Verdict | Source |
|---|---|---|---|
| A1 | PI Planning is a two-day event, held in person | ✅ | Section 1: "PI Planning takes two days and happens in person." |
| A2 | On day 1, after the business context and the vision, the teams draft their PI objectives and a first plan in breakouts | ✅ | Section 1, day 1 |
| A3 | At the end of day 1, every team presents its draft plan in a 10-minute slot | ❓ | Section 1 mentions a draft plan review at the end of day 1, but no 10-minute slot |
| A4 | On day 2, the business owners assign business value from 1 to 10 to each team's PI objectives | ✅ | Section 1, day 2 |
| A5 | A fist-of-five confidence vote closes the event; below an average of 3, the RTE and the teams agree on how to rework the plan | ✅ | Section 1, last point |

## 🤖 Answer B · "What do teams have to deliver before PI Planning?"

| # | Claim | Verdict | Source |
|---|---|---|---|
| B1 | The rules come from SAFe 6.0, section 4.3.2 "Team Backlog Readiness" | ❓ | No source we have contains this reference, and Kiro can't open it. Section 4: "Rules that are not on this page are not rules of this train." |
| B2 | Each team must rank all its user stories by WSJF | ❌ | Section 2: Product Management applies WSJF at feature level; teams don't rank their stories by WSJF |
| B3 | Teams submit the ranked list ten working days before PI Planning, or they lose their planning slot | ❌ | Section 2 has no such deadline and no sanction. The only list before the event is Product Management's top 10, five working days before |
| B4 | Teams submit draft PI objectives before PI Planning | ❌ | Section 1: the teams draft their PI objectives on day 1, during the event |
| B5 | Each team checks its capacity for the PI, including holidays and on-call duties | ✅ | Section 2, last row |

## 🤖 Answer C · "What is the timeline for preparing PI Planning?"

| # | Claim | Verdict | Source |
|---|---|---|---|
| C1 | Product Management shares the top features 3 working days before | ❌ | Section 2: 5 working days before |
| C2 | It shares the top 15 features | ❌ | Section 2: the top 10 features |
| C3 | Product Management ranks the features by WSJF | ✅ | Section 2, first row |
| C4 | In the last week before, the RTE and the POs collect known dependencies in the dependency list | ✅ | Section 2, second row |
| C5 | In the last week before, each team reviews the top features in a Refinement | ✅ | Section 2, third row. The playbook also asks the teams to send their questions to Product Management |
| C6 | Before the event, each team checks its capacity | ✅ | Section 2, last row |
| C7 | The event takes three days, with a third day for the confidence vote and the final plan review | ❌ | Section 1: two days, and the confidence vote ends the event |

## 📊 Summary

| Answer | ✅ | ❓ | ❌ | Can it be shared? |
|---|---|---|---|---|
| A | 4 | 1 | 0 | Yes, once the 10-minute slot is deleted or confirmed by Kim |
| B | 1 | 1 | 3 | No. Correct it in the channel |
| C | 4 | 0 | 3 | Only after the three wrong numbers are fixed |

## ✅ Check

A person looked up every quote in `art-playbook.md`; Kiro's verdicts alone were not enough.

> 📝 **Log:** prompt "According to art-playbook.md only, check every claim in answer-b.md…", plus a deep-analysis prompt for answers A and C · sources: `art-playbook.md`, `answer-a.md`, `answer-b.md`, `answer-c.md` · version 1.0 · reviewer: Agility Master, Team Signal
