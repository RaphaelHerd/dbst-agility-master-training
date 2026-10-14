# 📚 C07 - Tags and Metadata for the Train's Wiki · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

## 🧾 Metadata Fields

| Field | Values |
|---|---|
| **Type** | decision · meeting notes · how-to · team page · status · retro · playbook |
| **Team** | Signal · Switch · Concourse · Depot · ART |
| **Tags** | 2 to 5 from the tag list below |
| **Owner** | A role, never the name of a team member |
| **Status** | draft · proposed · valid · outdated |
| **Version and last reviewed** | 1.0, 1.1, … and a date |

## 🏷️ Tag List

`test-data` · `feed-v2` · `alerting` · `monitoring` · `platform-change-events` · `pi-planning` · `release-3-2` · `logging` · `estimation` · `dependencies` · `ai-use` · `flaky-tests`

**Rules:** lowercase with hyphens; new tags are agreed in the ART Sync, so the list stays short.

## 🗂️ The 14 Pages, Sorted

| # | Page | Type | Team | Tags | Status | Recommendation |
|---|---|---|---|---|---|---|
| 1 | Team Signal | team page | Signal | none | outdated | Update from the team one-pager: the team has six members, not five |
| 2 | decisions!! | decision | ART | estimation, feed-v2 | draft | Split into one decision record per decision; start with bugs |
| 3 | Notes ART Sync | meeting notes | ART | test-data, dependencies | valid | Keep; turn "release plans two weeks ahead" into a decision record |
| 4 | PI Planning Playbook | playbook | ART | pi-planning | valid | Keep |
| 5 | PI Planning Playbook (old) | playbook | ART | pi-planning | outdated | Archive: three days, top 15 and three working days are all out of date |
| 6 | How to get test data | how-to | Signal | test-data | outdated | Update to "two weeks in advance" and add an owner |
| 7 | Retro Signal Sprint 13 | retro | Signal | test-data, flaky-tests | valid | Keep |
| 8 | Retro notes Signal S13 | retro | Signal | test-data, flaky-tests | outdated | Merge into page 7: it's a duplicate |
| 9 | AI rules | how-to | ART | ai-use | outdated | Replace with the teams' AI working agreements |
| 10 | Alerting: who does what? | how-to | Depot | alerting, monitoring, dependencies | outdated | Contradicts page 11. Clarify in the ART Sync, then update |
| 11 | Monitoring for the delay feed | status | Depot | monitoring, alerting, feed-v2 | valid | Keep and link to page 10 |
| 12 | Platform-change events | decision | ART | platform-change-events, dependencies | draft | Keep as an open decision with an owner and a date |
| 13 | Release 3.2 | status | Concourse | release-3-2, logging | draft | Keep; add an owner and a date |
| 14 | Glossary | how-to | ART | none | draft | Keep and finish |

## 🔍 What the Pages Reveal

- **Decisions hidden in the pages:** feed format v2 frozen until the end of the PI, a demo every sprint for all teams (page 2); teams send Depot their release plans two weeks ahead (page 3); bugs get no estimates, with a question mark (page 2).
- **Pages 10 and 11 contradict each other:** one says Depot defines the alert rules, the other says Depot waits for Signal's alert definitions. That explains the deadlock between Signal and Depot.
- **Page 5 is the old playbook:** all three wrong numbers in C03's answer C are on this page. Outdated pages feed AI answers, too.

> 📝 **Log:** prompts "Read all 14 pages…", then "Propose metadata fields and at most 15 tags…" · sources: `wiki-export.md` · version 1.0 · reviewer: Agility Master, Team Signal
