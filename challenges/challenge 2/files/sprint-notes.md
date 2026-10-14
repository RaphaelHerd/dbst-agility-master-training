# 📡 Team Signal - Sprint 14 Review and Retrospective

> Confluence page · Team Signal · Sprint 14 (2 weeks) · Notes by the Agility Master

## Sprint Goal

Delay feed v2 runs in the test environment with a latency below 30 seconds.

## Sprint Review

| Item | Status | Note |
|---|---|---|
| SIG-141 Delay feed v2: new stream processor | Done | Latency in test: 22 seconds |
| SIG-142 Platform-change events for 5 pilot stations | Done | Shown in the demo |
| SIG-144 Data mapping for regional trains | Done | |
| SIG-148 Documentation of the feed format | Done | |
| SIG-150 Fix flaky integration tests | Partly done | 3 of 7 tests are stable |
| SIG-145 Load test with peak-hour data | Not done | Test data from the provider arrived late |
| SIG-147 Alerting for feed outages | Not done | Waiting for Depot (monitoring rules) |

**Committed:** 7 items · **Completed:** 4 items

## Stakeholder Feedback

- **Rail Ops:** "Platform changes in the app must never be older than one minute."
- **Kim (RTE):** asks for a clear status of the delay feed before PI Planning.

## Retrospective (Anonymous Notes)

**What went well**
- Strong demo, the pilot stations worked end to end.
- Pairing between developers and data engineers.

**What did not go well**
- Test data from the provider arrived late, for the third sprint in a row.
- Too many meetings on Wednesdays.

**Actions**

| Action | Owner |
|---|---|
| Ask the provider for test data two weeks in advance | open |
| Move Refinement to Tuesday | Alex |

## Open Points

- The decision from week one not to estimate bugs is still not written down.
- The dependency on Depot for alerting (SIG-147) has no agreed date yet.
