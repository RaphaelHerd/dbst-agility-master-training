# 🔎 JQL Examples

> Confluence page · ART SmartTransfer · collected by the Agility Masters · our projects: SIG, SWI, CON, DEP

## ✅ Good Examples

| Question | JQL |
|---|---|
| Which Signal items are in progress? | `project = SIG AND status = "In Progress"` |
| What did Team Signal finish yesterday? | `project = SIG AND resolution = Done AND resolved >= startOfDay(-1) AND resolved < startOfDay()` |
| Which Switch bugs are not done yet? | `project = SWI AND issuetype = Bug AND statusCategory != Done` |

## ❌ Looks Right, Isn't

| Question | Wrong JQL | Why it's wrong | Better |
|---|---|---|---|
| What did we finish last week? | `project = SIG AND status = Done AND updated >= -7d` | `updated` changes with every comment, and `-7d` means the last seven days, not last week | `project = SIG AND resolution = Done AND resolved >= startOfWeek(-1) AND resolved < startOfWeek()` |
| Which items were created more than 30 days ago? | `project = SIG AND created < 30d` | `30d` without a minus lies in the future, so this finds every item | `project = SIG AND created <= -30d` |
| Which stories have no story points? | `project = SIG AND sprint = "Sprint 15" AND "Story Points" = 0` | An empty field is not 0, and a fixed sprint name breaks next sprint | `project = SIG AND sprint in openSprints() AND "Story Points" is EMPTY` |

## 🏷️ Our Labels

- `dependency`: the item waits for another team on the train
- `rail-ops`: the item waits for Rail Ops
- `test-data`, `feed-v2`, `flaky-tests`: topics
