# 📈 C08 - Data-Quality Check · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

**Source:** `jira-export.csv`, 41 rows · **Window:** the 13 complete weeks from 6 July to 4 October

## 🔍 Problems and Decisions

| # | Problem | Row | Effect on the forecast | Decision |
|---|---|---|---|---|
| 1 | **Duplicate row** | SIG-131 appears twice | The week of 24 August counts 4 items instead of 3 | Delete one row |
| 2 | **Test ticket** | SIG-139 "TEST please ignore" | One extra item in the week of 7 September | Delete |
| 3 | **Item from another team** | SWI-205 | One extra item in the week of 17 August | Delete: the export filter was wrong |
| 4 | **Impossible date** | SIG-125 resolved in 2025, before it was created | Missing in the week of 10 August; negative cycle time | Fix to 2026-08-14; confirm with the team |
| 5 | **Done, but no resolved date** | SIG-128 | Can't be placed in a week | Leave out of the forecast; ask the team for the date |
| 6 | **No start date** | SIG-136 | No cycle time | Keep for throughput, leave out of cycle time |
| 7 | **Incomplete week** | SIG-154, resolved on Monday 5 October | A week that has just begun pulls the average down | Use complete weeks only |
| 8 | **Very low week** | 1 item in the week of 10 August | Looks like an outlier | Keep: it was the summer break, and holidays will happen again |

## 📊 Before and After

| | Raw export | Cleaned |
|---|---|---|
| Items finished in the 13 weeks | 33 | 31 |
| Average per week | 2.54 | 2.38 |

Two extra items look small. But they are exactly the kind of error that makes a forecast too optimistic, and Sascha would ask about it.

## ❓ Open Questions for the Team

- When was SIG-128 really finished?
- Is 14 August the right date for SIG-125?

> 📝 **Log:** prompt "Check every row of jira-export.csv for data-quality problems…" · sources: `jira-export.csv`, `sprint-notes.md`, `team-calendar.md` · version 1.0 · reviewer: Agility Master, Team Signal
