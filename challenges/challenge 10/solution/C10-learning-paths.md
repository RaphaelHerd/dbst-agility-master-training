# 🌱 C10 - Learning Paths for the Next PI · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

> SharePoint page · Team Signal · team level only: based on the self-assessment, without statements about individual members

## 🗺️ Where the Team Needs to Grow

| Skill | People at level 2 or higher | Needed | Gap | Someone in the team can teach |
|---|---|---|---|---|
| Load and performance testing | 0 | 2 | **2** | No |
| Observability and alerting | 1 | 2 | **1** | No |
| Test automation | 2 | 3 | **1** | Yes |
| Cloud and Kubernetes | 1 | 2 | **1** | Yes |
| Stream processing, backend, data modelling, rail data domain | enough | | 0 | |

## 🧪 Load and Performance Testing

- **Steps:** two volunteers take a course **[DB placeholder: internal training catalogue]** → pair with Team Switch on their performance measurements → run the peak-hour load test (SIG-145) together once the test data arrives → show the results in a team demo.
- **Who can help:** Team Switch, which works on the speed of its recommendations.
- **How we'll know:** two people at level 2 in the next self-assessment, and the load test run by the team.
- **Goals to choose from:**
  - "By the end of the next PI, I can design and run a load test with peak-hour data on my own."
  - "By the end of the next PI, I can read load-test results and explain the bottlenecks to the team."

## 🚨 Observability and Alerting

- **Steps:** pair with Team Depot's site reliability engineers on the monitoring rules for the delay feed → write our alert definitions together. This also breaks the deadlock between the two teams.
- **Who can help:** Team Depot.
- **How we'll know:** alerting for feed outages (SIG-147) is live, and two people can maintain it.
- **Goals to choose from:**
  - "By the end of the next PI, I can write alert definitions for our services and agree on them with Team Depot."
  - "By the end of the next PI, I can find the cause of a feed outage with our dashboards and logs."

## ✅ Test Automation

- **Steps:** pair with the colleague at level 3 while the team fixes two flaky tests per sprint, the action from the retro.
- **Who can help:** someone in the team at level 3.
- **How we'll know:** three people at level 2, and 7 of 7 integration tests stable.
- **Goals to choose from:**
  - "By the end of the next PI, I can write stable integration tests for the feed on my own."
  - "By the end of the next PI, I can find and fix the cause of a flaky test."

## ☁️ Cloud and Kubernetes

- **Steps:** shadow the colleague at level 3 during deployments → take over one deployment per sprint with support → do it alone.
- **Who can help:** someone in the team at level 3.
- **How we'll know:** two people can deploy and roll back on their own, so the skill no longer depends on one person.
- **Goals to choose from:**
  - "By the end of the next PI, I can deploy and roll back our services on my own."
  - "By the end of the next PI, I can explain our cluster setup to a new team member."

> 💡 Every team member chooses their own goals in their development talk. Nobody is assigned a goal from this page.

> 📝 **Log:** prompts "First make a plan…", "First give me only the skeleton of a learning-path page…", "For each skill with a gap, write two development goals…" · sources: `skill-matrix.csv` (team level), `pi-needs.md`, `C10-skill-gap-map.xlsx` · version 1.0 · reviewer: Agility Master, Team Signal
