# 📈 C08 - Early-Warning Signals · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

Kiro proposed three signals. Each one was checked in Excel. Two are real, one is not.

| Signal | Excel check | Result | Real? |
|---|---|---|---|
| **Aging items:** open longer than 85 % of all finished items | Age = export date minus start date; compare with `=PERCENTILE.INC(Data!H:H,0.85)`, which is 9 days | SIG-138: 71 days · SIG-147: 25 · SIG-145: 22 · SIG-150: 21 · SIG-152: 8, so watch it | ✅ Yes |
| **Rising work in progress** | `=COUNTIFS(...)` per week end: started, but not yet finished | 1 to 4 items per week until mid-September, **6** in each of the last three weeks | ✅ Yes |
| **Longer cycle times** | Median of the last four weeks compared with the median of all 13 weeks | 6 days recently, 7 days overall | ❌ Not visible in this data |

## 🚦 What It Means

- **SIG-138** (archive old feed v1 data) has been in progress for 71 days. Finish it or stop it.
- **SIG-145** and **SIG-147** are blocked by test data and by the deadlock with Depot. They are the reason work in progress is rising.
- **Check weekly:** if more than 6 items are in progress or a new item crosses 9 days, look again at the forecast.

> 📝 **Log:** prompt "Which signals in this data warn us early…? Give me the Excel formula for each." · sources: `C08-forecast-model.xlsx` · version 1.0 · reviewer: Agility Master, Team Signal
