# 🚆 ART SmartTransfer - Status Before PI Planning

> Confluence page · collected by Kim from all four teams · Thursday

## 📡 Team Signal · Real-time train data

- **Sprint 14:** goal reached. Delay feed v2 runs in test at 22 seconds (goal: below 30). 4 of 7 items done.
- **Forecast from Tuesday:** the remaining 24 rollout items take 12 weeks with 85 % confidence.
- **New today:** two of six team members won't be available in the next PI. The team chose a plan that fits: outage alerting, peak-hour readiness, platform-change events for Team Concourse and feed v2 in Team Switch's test environment. **The feed v2 rollout to all major stations moves to the following PI.**
- **Decision requested:** escalate the late test data to the train data provider.

## 🔀 Team Switch · Transfer logic

- **Sprint 14:** goal reached. Alternative routes work in test. 3 of 6 items done.
- **Open:** recommendations take 320 ms instead of 200 ms. Feed v2 in Switch's test environment arrives in Sprint 3; Switch starts with walking times instead.
- **Decision requested:** make feed v2 in Switch's test environment a train-level priority. Team Signal has now planned it for Sprint 3.

## 📱 Team Concourse · The passenger app

- **Sprint 14:** goal reached. Push notifications are live for 200 beta users. 3 of 5 items done.
- **Open:** the final notification texts wait for Rail Ops. The release date of app 3.2 is not fixed.
- **Decision requested:** Rail Ops approves a set of text templates once; the team writes new texts within them.

## 🛠️ Team Depot · Platform and operations

- **Sprint 14:** goal not reached. The logging platform runs in test, but only with Team Signal's logs. 2 of 5 items done.
- **Open:** ad-hoc requests take around 40 % of the capacity.
- **Decision requested:** all ad-hoc requests go through the new request form, with incidents as the only exception.

## 🧭 The Train as a Whole

- **Priorities (WSJF):** outage alerting (F2) and peak-hour readiness (F10) are ranks 1 and 2 in every variant. Rank 3 depends on the method; whether F6's legal deadline is confirmed is still open.
- **Dependencies:** 11 between teams or with people outside the train: 3 late, 5 with nothing planned, 1 in the same sprint, 2 fine.
- **Top risks:** the alerting deadlock between Signal and Depot, with a proposal on the table; and the peak-hour load test, planned before its test environment exists and without test data.
