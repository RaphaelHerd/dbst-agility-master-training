# ✅ C11 - Everyone Rated These Differently · Sample Solution

> 📘 **Sample solution** for Team Signal &nbsp;|&nbsp; 🤖 **Your results will look different:** AI answers vary from run to run. Compare the substance, not the wording.

## 🧭 How to Use This Solution

1. **Finish the challenge first.** The learning happens while you work with Kiro and Excel, not while you read a solution.
2. **Open the samples** and put them next to your own results.
3. **Compare:** Is your ranking the same? Did you find the assumptions that change the top 3?

## 📂 Sample Results

| Deliverable | Sample |
|---|---|
| Excel workbook: scores, WSJF variants and scenarios | [C11-wsjf.xlsx](C11-wsjf.xlsx) |
| Note for Kim | [C11-wsjf-rationale.md](C11-wsjf-rationale.md) |
| Scenario comparison and decision | [C11-scenarios.md](C11-scenarios.md) |

## 🎯 What a Good Result Looks Like

| Deliverable | Your result is good when … |
|---|---|
| **WSJF sheet** | Excel calculates averages, medians, spreads and WSJF; the disagreements are visible next to the ranking |
| **Note for Kim** | It names the stable part of the ranking, the open place, the assumptions that change it, and questions; the decision stays with Product Management |
| **Scenarios** | Three options with load and share of capacity from Excel, a decision by the group, the hidden assumptions and who must be told |
| **Your prompts** | The formula prompt asks for averages, medians and spreads and forbids results; the decision check names principles before it looks at the ranking |

## 💬 Sample Prompts

Prompts like these worked well. Yours don't need the same words; compare what they ask for.

| Step | Sample prompt | Why it works |
|---|---|---|
| **Formulas** | *"For each feature and each WSJF component, we need the average, the median and the spread between the highest and the lowest score. Then WSJF from the averages and from the medians. Write the Excel formulas and explain them. Don't calculate anything yourself."* | Two methods side by side, and the spread keeps the disagreement visible |
| **Step-back decision check** | *"Step back first: which principles should decide the order of features on a release train? Then look at our ranking: which single assumption would change the top 3? Check the notes in features.csv, too."* | Principles first, so the legal deadline in the notes gets noticed |
| **Bias** | *"Compare the three business owners. Does anyone score their own area consistently higher? What does that mean for an average?"* | Asks about the pattern, not about a person's motives |
| **Scenarios** | *"Draft three scenarios for our next PI with two people fewer and the new dependency from Team Concourse. For each one: what we do, what moves to a later PI, and who is affected. Don't calculate the load; we'll do that in Excel."* | A fixed structure for each option, and the math stays in Excel |
| **Hidden assumptions** | *"Which assumptions are hidden in our capacity calculation, and how could they be wrong?"* | A second step back, this time at your own numbers |

## 📊 Part 1: The Decision Check

```
Average per owner score   =AVERAGEIFS(Scores!$C$2:$C$31,Scores!$A$2:$A$31,$A2)
Median                    =AGGREGATE(17,6,Scores!$C$2:$C$31/(Scores!$A$2:$A$31=$A2),2)
Spread                    =AGGREGATE(14,6,…,1)-AGGREGATE(15,6,…,1)
WSJF                      =(BV+TC+RR)/JobSize
```

| Finding | Why it matters |
|---|---|
| **F2 and F10 are stable** at ranks 1 and 2 | That's where the train can commit with confidence |
| **Place 3 depends on the method:** F7 with averages, F1 with medians | The method has to be chosen, and explained |
| **F6's deadline is a fact,** not an opinion | Counted as a fact, F6 jumps to place 3 |
| **Each owner favors their own area** | An average of interests looks objective but isn't |

> 💡 **Step-back prompting** pays off here: Kiro first names the principles (cost of delay, fixed dates, small jobs first) and only then looks at the numbers. That's how the legal deadline in `features.csv` gets noticed.

## 👥 Part 2: The Scenarios

| Scenario | Load | Share of 58.8 points |
|---|---|---|
| A · Everything | 81 | 138 % |
| **B · Top WSJF and commitments** | **52** | **88 %** |
| C · Rollout first | 60 | 102 % |

> ⚠️ **The forecast from C08 no longer holds.** It assumed six people. A good result says so, and tells Sascha.

> 💡 **No reasons needed:** Alex didn't say why two people are missing, and nobody needs to know. Planning works without private details.

## 💡 What to Take Away

1. **Show the spread next to every average.** Disagreement is information.
2. **Step back before deciding:** principles first, numbers second, and ask what would change the result.
3. **Scenarios with Excel, decisions with people,** and tell everyone whose plans change.

> ⚖️ *One transparent ranking and one honest plan: that's what the train needs for PI Planning.*
