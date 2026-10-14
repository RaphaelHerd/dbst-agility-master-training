# ⚙️ Changing Jira Automation on the Train

> Confluence page · ART SmartTransfer · Owner: Kim, Release Train Engineer · applies to every automation rule in the shared Jira

> ⚠️ **[DB placeholder: company rules for change management and for automation in Jira]**

## 🔁 The Steps

| # | Step | Who |
|---|---|---|
| 1 | **Change request:** what, why, trigger, condition, action, risk and how to switch the rule off | Whoever wants the rule |
| 2 | **Approval** by the Release Train Engineer and the Jira administrator | Kim and the Jira administrator in Team Depot |
| 3 | **Test** in the sandbox project `SANDBOX` with test issues, never on a live project first | Whoever wants the rule |
| 4 | **Go-live** with a named rule owner and the rule's audit log switched on | Jira administrator |
| 5 | **Log:** one line in the change log with date, rule, version and approver | Rule owner |
| 6 | **Review** after four weeks: does the rule still do what it should? | Rule owner |

## 🚫 Never

- Rules that monitor or compare individual people.
- Rules that send messages to large groups without a review.
