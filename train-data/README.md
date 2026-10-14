# 🚆 Train Data: The Rest of the Train

> 🔒 **Trainer material, not for participants.** All groups play the Agility Master of **Team Signal**. This folder holds the data of the other three teams, so that cross-team challenges on Day 2 can stage dependencies and conflicts with prepared files and scenes.

| Team | Works on | Files |
|---|---|---|
| 🔀 Switch | Transfer logic | `switch/` |
| 📱 Concourse | The passenger app | `concourse/` |
| 🛠️ Depot | Platform and operations | `depot/` |

| File | Content |
|---|---|
| `one-pager.md` | Team one-pager: purpose, members (pseudonyms), events, what the team gives and needs |
| `sprint-notes.md` | Sprint 14 Review and Retrospective |
| `dod-agreed.md` | The team's agreed Definition of Done |
| `jira-export.csv` | Sprint 14 items with story points |
| `decision-needed.md` | The PO's decision request for the steering committee |

## 🔗 Dependencies Already in the Story

- **Signal → Switch:** Switch waits for delay feed v2 in its test environment; no date is agreed.
- **Signal ↔ Depot:** Signal's outage alerting waits for Depot's monitoring rules, and Depot's monitoring rules wait for Signal's alert definitions.
- **Signal ↔ Concourse:** nobody knows who owns the platform-change events.
- **Concourse ↔ Depot:** the Concourse log migration was postponed because of app release 3.2.
- **Depot ← all teams:** ad-hoc requests take around 40 % of Depot's capacity.

> ⚠️ Each `jira-export.csv` marks one partly-done item as **Done** (SWI-219, CON-307, DEP-509). That was the C05 trap in the four-team version. Fix the status or reuse the trap on purpose when you copy a file into a challenge.
