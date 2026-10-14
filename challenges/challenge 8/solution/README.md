# ✅ C08 - The Number Sascha Will Actually Believe · Sample Solution

> 📘 **Sample solution** for Team Signal &nbsp;|&nbsp; 🤖 **Your results will look different:** AI answers vary from run to run, and a Monte Carlo simulation changes a little every time Excel recalculates. Compare the substance, not the decimals.

## 🧭 How to Use This Solution

1. **Finish the challenge first.** The learning happens while you work with Kiro and Excel, not while you read a solution.
2. **Open the samples** and put them next to your own results.
3. **Compare:** Did you find the same data problems? Do your 50/85/95 % weeks match within about one week?

## 📂 Sample Results

| Deliverable | Sample |
|---|---|
| Data-quality check | [C08-data-quality.md](C08-data-quality.md) |
| Excel model with live formulas | [C08-forecast-model.xlsx](C08-forecast-model.xlsx) |
| Forecast statement for Sascha | [C08-forecast-statement.md](C08-forecast-statement.md) |
| Early-warning signals | [C08-early-warnings.md](C08-early-warnings.md) |

> 💡 Press **F9** in the Excel model: the simulation runs again, and the probabilities move by a percent or two. The weeks at 50, 85 and 95 % stay the same in almost every run.

## 🎯 What a Good Result Looks Like

| Deliverable | Your result is good when … |
|---|---|
| **Data quality** | You found the duplicate, the test ticket, the other team's item, the wrong year and the incomplete week, and you decided on each one |
| **Model** | Excel calculates everything, with no number typed in from the chat; the total of finished items matches the cleaned data (31) |
| **Forecast** | It gives one number with its confidence, both estimates with a probability, the back-test and what the number does not mean |
| **Early warnings** | Each signal was checked in Excel, including the one that turned out not to be real |
| **Your prompts** | The data check proposes but doesn't fix; the plan comes before the formulas; every prompt forbids Kiro to calculate |

## 💬 Sample Prompts

Prompts like these worked well. Yours don't need the same words; compare what they ask for.

| Step | Sample prompt | Why it works |
|---|---|---|
| **Data check** | *"Check every row of jira-export.csv for data-quality problems: duplicates, items from other teams, test tickets, impossible or missing dates, and incomplete weeks. Use the sprint notes and the team calendar as context. Make a table: row, problem, effect on a forecast, proposed fix. Don't fix anything yet."* | Names what to look for, adds context, and leaves the decisions with you |
| **Plan first** | *"We want to know how many weeks the 24 remaining items will take, based on how many items we finished per week. First make a plan: which steps, and which sheets in Excel? Don't calculate anything yet."* | Plan-and-solve: you see the method before any number exists |
| **Formulas** | *"Write the Excel formulas for each step: items finished per week with COUNTIFS, cycle time, work in progress per week, and a Monte Carlo simulation with 1000 runs that draws random weeks from our history with INDEX and RANDBETWEEN. Explain each formula. Don't calculate any results yourself."* | Formulas you can check, and Excel does the math |
| **Back-test** | *"Use only weeks 1 to 6 to forecast how many items we finish in weeks 7 to 12. Give me the formulas for a range with 85 % confidence."* | Tests the method against the past before anyone trusts it |
| **Early warnings** | *"Which signals in this data warn us early that the forecast is getting worse, for example aging items, rising work in progress or longer cycle times? Give me the Excel formula for each."* | Every signal comes with a formula, so you can check whether it's real |

## 🔍 Part 1: The Traps in the Export

| Trap | Why AI and people miss it |
|---|---|
| Duplicate row (SIG-131) | Looks like a normal row unless you compare keys |
| Test ticket (SIG-139) | Easy to spot, but only if someone reads the summaries |
| Other team (SWI-205) | One wrong filter, one extra item |
| Wrong year (SIG-125) | The item silently drops out of the window |
| Incomplete week (5 and 6 October) | The newest data looks the most valuable, but a week that has just begun is not a full week |
| Summer break (week of 10 August) | Not an error! Removing it would make the forecast too optimistic |

## 🧮 Part 2: The Formulas That Matter

```
Items per week     =COUNTIFS(Data!$G:$G,">="&B2,Data!$G:$G,"<"&B2+7)
One random week    =INDEX(Throughput!$C$2:$C$14,RANDBETWEEN(1,13))
Probability        =COUNTIF(<totals after N weeks>,">="&24)/1000
Weeks at 85 %      =INDEX(weeks,MATCH(TRUE,INDEX(probabilities>=0.85,0),0))
```

| Result | Value |
|---|---|
| Finished items in 13 weeks | 31, on average 2.38 per week |
| Weeks needed with 50 / 85 / 95 % confidence | 10 / 12 / 13 |
| Alex's 4 weeks | 0 %: at most 4 items per week can't reach 24 in four weeks |
| Member A's 10 weeks | about 50 % |

> ⚠️ **The classic mistake:** "2.38 items per week, so 24 items take about 10 weeks." That's the average, and it's the 50 % value: a coin flip. Sascha asked for 85 %.

## 🧪 Part 3: The Back-Test

Weeks 1 to 6 forecast **11 to 17** items for weeks 7 to 12, with 85 % confidence for each limit. The team finished **15**. The method passes. If the actual number had been far outside the range, the forecast would not be defensible.

## 💡 What to Take Away

1. **Clean first:** two extra items in the raw export would have made the forecast too optimistic.
2. **AI plans and writes formulas; Excel calculates; you check.** Math in a chat is pattern matching, not arithmetic.
3. **A forecast is a probability, not a promise.** Say so, and say how you tested it.

> 📈 *Twelve weeks with 85 % confidence: tested on the past and calculated in Excel. That's a number Sascha can defend.*
