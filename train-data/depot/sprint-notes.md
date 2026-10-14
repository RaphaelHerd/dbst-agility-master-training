# 🛠️ Team Depot - Sprint 14 Review and Retrospective

> Confluence page · Team Depot · Sprint 14 (2 weeks) · Notes by the Agility Master

## Sprint Goal

The new logging platform runs in the test environment for two teams.

## Sprint Review

| Item | Status | Note |
|---|---|---|
| DEP-501 Logging platform in the test environment | Done | |
| DEP-503 Migrate the logs of Team Signal | Done | |
| DEP-509 Update the on-call runbook | Partly done | Two of five services documented |
| DEP-504 Migrate the logs of Team Concourse | Not done | Postponed because of release 3.2 |
| DEP-507 Monitoring rules for the delay feed | Not done | No alert definitions from Team Signal yet |

**Committed:** 5 items · **Completed:** 2 items

## Stakeholder Feedback

- **Kim (RTE):** worried that the logging migration collides with PI Planning and release 3.2.
- **Team Signal:** needs alerting for feed outages as soon as possible.

## Retrospective (Anonymous Notes)

**What went well**
- The new logging platform was set up fully automated.
- On-call handovers worked smoothly.

**What did not go well**
- Ad-hoc requests took around 40 % of our capacity.
- Waiting for alert definitions blocked our monitoring work.

**Actions**

| Action | Owner |
|---|---|
| Introduce a request form for ad-hoc requests | Member C |
| Agree on alert definitions with Team Signal | open |

## Open Points

- The decision from week one not to estimate bugs is still not written down.
- The date for the Concourse log migration is not confirmed.
