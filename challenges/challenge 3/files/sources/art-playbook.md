# 📘 ART SmartTransfer - PI Planning Playbook

> Confluence page · ART SmartTransfer · Version 2.1 · Owner: Kim, Release Train Engineer

This page is the train's single source of truth for PI Planning.

## 1 · The Event

- PI Planning takes **two days** and happens in person.
- **Day 1:** business context and vision, then team breakouts. Each team drafts its **PI objectives** and a first plan. Draft plan review at the end of day 1.
- **Day 2:** the teams adjust their plans. The **business owners** assign business value from 1 to 10 to each team's PI objectives.
- The event ends with a **confidence vote** (fist of five, 1 to 5). If the average is below 3, the RTE and the teams agree on how to rework the plan before the event ends.

## 2 · Before the Event

| When | What | Who |
|---|---|---|
| 5 working days before | Share the **top 10 features** of the ART backlog, ranked by WSJF | Product Management |
| Last week before | Collect known dependencies in the dependency list (Excel) | RTE with the POs |
| Last week before | Review the top 10 features in a Refinement and send questions to Product Management | Each team |
| Before the event | Check team capacity for the PI, including holidays and on-call duties | Each team |

**Prioritization:** Product Management applies WSJF at **feature** level, together with the business owners. Teams do **not** rank their stories by WSJF; each PO orders the team backlog.

## 3 · Definition of Done: ART-Wide Minimum

Every story on the train meets at least these four points. Teams can add their own points, but they can't remove these.

1. Acceptance criteria are met and accepted by the Product Owner.
2. The code is reviewed by at least one other person.
3. Automated tests pass in the pipeline.
4. The change is deployed to the shared test environment through the pipeline.

## 4 · Changes to This Playbook

Only the RTE changes this page, after agreement in the ART Sync. **Rules that are not on this page are not rules of this train.**
