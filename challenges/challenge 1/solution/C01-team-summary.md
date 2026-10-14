# 📡 C01 - Team Summary: Team Signal · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

## 🧭 Our Team in Five Bullets

- **Purpose:** We are the real-time backbone of SmartTransfer: live train positions, delays and platform changes, passed on to the other teams within seconds.
- **People:** Product Owner Alex, the Agility Master and six team members (Member A to F): two backend developers, two data engineers, one tester and one DevOps engineer.
- **Events:** two-week sprints with the Daily at 09:15, Refinement on Wednesday at 13:00, and Sprint Review and Retrospective every second Thursday at 14:00 and 15:30.
- **Current focus:** delay feed v2 (latency from 60 to 15 seconds), platform-change events for all major stations, and stable integration tests.
- **Biggest open issue:** Sprint 14 delivered 4 of 7 items. The load test is stuck because test data arrived late for the third sprint in a row, and outage alerting waits for Team Depot without an agreed date.

## ❓ Follow-up Questions

**1. What should I raise at today's stand-up?**
- The alerting work (SIG-147) depends on Team Depot and still has no agreed date.
- The action "ask the provider for test data two weeks in advance" has no owner yet.
- 4 of 7 integration tests are still flaky (SIG-150).

**2. Which risks do the notes mention?**
- Test data from the provider arrives late, for the third sprint in a row; the load test (SIG-145) is still open.
- There is no alerting for feed outages yet (SIG-147).
- Flaky integration tests slow down every release.
- Rail Ops expects platform changes in the app never to be older than one minute.

**3. What is unclear or missing in these notes?**
- Who owns the test-data action.
- When Team Depot can deliver the monitoring rules for SIG-147.
- Who owns the platform-change events once they are live: Signal or Concourse.
- Which latency target applies when: the sprint goal says below 30 seconds, the PI focus says 15 seconds.
- The decision from week one not to estimate bugs is still not documented.

## ✅ Check

Every statement was checked against `one-pager.md` and `sprint-notes.md`. Nothing was added that is not in the sources.

> 📝 **Log:** prompt "Read the files in this folder and summarize our team in five bullet points…" · sources: `one-pager.md`, `sprint-notes.md` · version 1.0 · reviewer: Agility Master, Team Signal
