# 🔀 Team Switch - Sprint 14 Review and Retrospective

> Confluence page · Team Switch · Sprint 14 (2 weeks) · Notes by the Agility Master

## Sprint Goal

Alternative routes for broken connections work in the test environment.

## Sprint Review

| Item | Status | Note |
|---|---|---|
| SWI-210 Alternative routes for broken connections | Done | Demo with three real-world scenarios |
| SWI-214 Walking times for 10 stations | Done | Data source for two stations unclear |
| SWI-220 Bug fixes from the last release | Done | |
| SWI-219 Performance tuning | Partly done | 320 ms instead of 200 ms per recommendation |
| SWI-216 Switch to delay feed v2 | Not done | Feed v2 is not yet available in our test environment |
| SWI-222 Acceptance criteria for "connection at risk" | Not done | Rail Ops has not confirmed the criteria |

**Committed:** 6 items · **Completed:** 3 items

## Stakeholder Feedback

- **Rail Ops:** "A connection at risk must be flagged early enough for passengers to react."
- **Sam (PO):** wants SWI-216 to be the top priority for the next sprint.

## Retrospective (Anonymous Notes)

**What went well**
- The alternative-routes demo convinced the stakeholders.
- Good knowledge sharing between developers and algorithm engineers.

**What did not go well**
- Acceptance criteria from Rail Ops are still unclear.
- The shared test environment was down twice.

**Actions**

| Action | Owner |
|---|---|
| Clarify "connection at risk" with Rail Ops | Sam |
| Agree on a date for feed v2 in our test environment with Team Signal | open |

## Open Points

- The decision from week one not to estimate bugs is still not written down.
- Performance target (200 ms) is at risk if feed v2 arrives late.
