# ⚖️ C11 - WSJF: Note for Kim · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

**Subject:** The top 10, with open eyes

Hi Kim,

All numbers come from `C11-wsjf.xlsx`; Excel calculated them.

## 📊 The Ranking

| Rank | Feature | WSJF (averages) | Biggest disagreement |
|---|---|---|---|
| 1 | F2 Outage alerting for real-time data | 6.53 | Time criticality: 5 to 20 |
| 2 | F10 Peak-hour readiness for the delay feed | 4.04 | Small |
| 3 | F7 Logging migration for all teams | 2.63 | Risk reduction: 3 to 20 |
| 4 | F6 Screen-reader support across the app | 2.58 | Time criticality: 8 to 20 |
| 5 | F8 Self-service request portal | 2.47 | Risk reduction: 2 to 13 |
| 6 | F3 Push notifications for all users | 2.38 | Business value: 3 to 20 |
| 7 | F1 Delay feed v2 at all major stations | 2.28 | Time criticality: 5 to 13 |
| 8 | F9 Platform-change events at all major stations | 1.33 | Business value: 5 to 13 |
| 9 | F5 Walking times for the 50 largest stations | 1.10 | Business value: 3 to 13 |
| 10 | F4 Alternative routes at night | 1.08 | Business value: 2 to 8 |

## 🔍 What the Disagreements Show

Each business owner scores **their own area** highest: Passenger Experience gives F3 the top business value, Platform gives F7 and F8 the top risk reduction, Operations gives F2 the top time criticality. An average of three interests is not a shared view.

## 🔄 What Would Change the Top 3

**Stable in every variant:** F2 and F10 stay at ranks 1 and 2. **Place 3 is open:**

| Assumption | Who is at rank 3 |
|---|---|
| Averages, as today | F7 Logging migration (2.63) |
| Medians instead of averages | F1 Delay feed v2 (2.23) |
| F6's legal deadline counts as a fact: time criticality 20 | F6 Screen-reader support (3.58) |

Ranks 3 to 6 lie within 0.25 points of each other. A small change in the method decides who gets in.

## ❓ Questions for Product Management

1. Is F6's legal deadline confirmed? If yes, its time criticality is a fact, not an opinion.
2. Averages or medians, and why?
3. Could F1 be split into smaller features? WSJF favors small jobs.
4. Should the business owners discuss F3 and F7 together before anyone scores again?

The decision stays with Product Management.

Best regards,
Agility Master, Team Signal

> 📝 **Log:** prompts "Write the Excel formulas… Don't calculate anything yourself.", "Step back first… which single assumption would change the top 3?", "Compare the three business owners…" · sources: `wsjf-scores.csv`, `features.csv`, `C11-wsjf.xlsx` · version 1.0 · reviewer: Agility Master, Team Signal
