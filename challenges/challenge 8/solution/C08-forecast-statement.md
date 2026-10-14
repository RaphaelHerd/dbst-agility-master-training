# 📈 C08 - Forecast Statement for Sascha · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

**Subject:** Re: One number I can defend

Hi Sascha,

**The number:** with **85 % confidence**, the 24 remaining items are done within **12 weeks**.

| Confidence | Weeks needed |
|---|---|
| 50 % | 10 |
| **85 %** | **12** |
| 95 % | 13 |

**The two estimates:**
- **4 weeks:** practically impossible with our pace. Not one of 1000 simulated runs finished 24 items in four weeks.
- **10 weeks:** a coin flip, with about 50 % probability.

**How we got there:** a Monte Carlo simulation in Excel, based on 13 weeks of real data. Team Signal finished 31 items in that time, between 1 and 4 per week. We cleaned the Jira export first: one duplicate, one test ticket, one item from another team and one wrong date.

**How we tested it:** we used only weeks 1 to 6 to forecast weeks 7 to 12. The forecast said 11 to 17 items; the team finished 15.

**What the number does not mean:**
- It is not a promise. It assumes the next weeks look like the last 13.
- It is not a measure of performance. It describes the system the team works in, not individual effort.
- It counts every finished item, bugs included. Bugs that come up during the rollout are not part of the 24 items.

**Risk to watch:** four items have been open far longer than usual, and work in progress has doubled in the last three weeks. If that continues, plan with 13 weeks rather than 12.

Best regards,
Agility Master, Team Signal

> 📝 **Log:** prompts "First make a plan…", "Write the Excel formulas for each step…", "Use only weeks 1 to 6…" · sources: `jira-export.csv` (cleaned), `C08-forecast-model.xlsx` · version 1.0 · reviewer: Agility Master, Team Signal
