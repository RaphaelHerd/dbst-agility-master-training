# 👥 C11 - Three PI Scenarios for Team Signal · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

## 🧮 Capacity

Average velocity 20.75 points × 5 sprints × 4 of 6 people × 85 % (15 % for bugs) = **58.8 points**, calculated in Excel.

## 🔀 The Scenarios

| Scenario | What we do | What moves to a later PI | Load | Share | Fits? |
|---|---|---|---|---|---|
| **A · Everything** | All six items | Nothing, on paper | 81 | 138 % | ❌ |
| **B · Top WSJF and commitments** | Outage alerting (F2), peak-hour readiness (F10), platform-change events for Concourse (F9), feed v2 in Switch's test environment | The feed v2 rollout to the major stations | 52 | 88 % | ✅ |
| **C · Rollout first** | The complete feed v2 rollout (F1), platform-change events (F9), outage alerting (F2) | Peak-hour readiness (F10) | 60 | 102 % | ❌ no buffer |

## ✅ Our Decision: Scenario B

- It **fits** and leaves room for surprises.
- It follows the **WSJF ranking**: F2 and F10 are the top two in every variant.
- It **keeps our commitments**: Team Concourse gets the platform-change events by Sprint 2, and Team Switch gets feed v2 in its test environment.
- Scenario C would put the feed live **without a peak-hour test**, the very risk in our decision paper for the steering committee.

## 🙈 Hidden Assumptions

- **Velocity shrinks in proportion to the people.** If the two missing people hold skills that only they have, the team loses more than a third. The gap map from C10 shows where.
- **15 % for bugs** is our estimate, not a measurement.
- **Five full sprints:** holidays and on-call duties are not included.

## 📣 Who Must Be Told

| Who | What changes for them |
|---|---|
| **Kim and the steering committee** | The feed v2 rollout moves to the following PI |
| **Sascha** | The forecast of 12 weeks assumed six people. It no longer applies and needs to be recalculated |
| **Team Switch** | The rollout moves; feed v2 in their test environment stays in this PI |
| **Team Concourse** | Platform-change events by the end of Sprint 2, as requested |
| **Rail Ops** | Delay information from feed v2 reaches all major stations later |

> 📝 **Log:** prompts "Draft three scenarios for our next PI…", "Which assumptions are hidden in our capacity calculation…" · sources: `capacity-news.md`, `C11-wsjf.xlsx` · version 1.0 · reviewer: Agility Master, Team Signal
