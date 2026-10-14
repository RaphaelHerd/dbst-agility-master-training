# ✅ C10 - Grow the Team, Not a Ranking · Sample Solution

> 📘 **Sample solution** for Team Signal &nbsp;|&nbsp; 🤖 **Your results will look different:** AI answers vary from run to run. Compare the substance, not the wording.

## 🧭 How to Use This Solution

1. **Finish the challenge first.** The learning happens while you work with Kiro, not while you read a solution.
2. **Open the samples** and put them next to your own results.
3. **Compare:** Did you find the same gaps? Did your rewrite keep placeholders instead of inventing examples?

## 📂 Sample Results

| Deliverable | Sample |
|---|---|
| Team-level gap map in Excel | [C10-skill-gap-map.xlsx](C10-skill-gap-map.xlsx) |
| Learning paths and development goals | [C10-learning-paths.md](C10-learning-paths.md) |
| Feedback critique and rewrite | [C10-feedback-draft.md](C10-feedback-draft.md) |
| Reply to the ranking request | [C10-reply-to-manager.md](C10-reply-to-manager.md) |

## 🎯 What a Good Result Looks Like

| Deliverable | Your result is good when … |
|---|---|
| **Gap map** | It counts people per skill and level, compares with the need and colors the result, and it never shows who is where |
| **Learning paths** | Each gap has steps, help and a measure; goals are options that people choose, not assignments |
| **Feedback** | Every coded phrase, claim without evidence and sign of recency bias is named; the rewrite describes behavior and keeps placeholders for evidence |
| **Reply** | It says no, gives the reasons (purpose, high-risk AI, agreement, trust) and offers the team-level results |
| **Your prompts** | Every prompt on skills stays at team level; the skeleton waits for your OK; the rewrite prompt forbids invented examples |

## 💬 Sample Prompts

Prompts like these worked well. Yours don't need the same words; compare what they ask for.

| Step | Sample prompt | Why it works |
|---|---|---|
| **Plan first** | *"We want a team-level gap map for the next PI. First make a plan: which steps, and which Excel formulas? Stay at team level: no statements about individual members. Don't calculate anything yet."* | Sets the team-level rule before any data is touched |
| **Skeleton-of-thought** | *"First give me only the skeleton of a learning-path page for the skills with a gap: one section per skill, with steps, who can help, and how we'll know it worked. Wait for my OK before you fill it in."* | You approve the structure before Kiro writes the details |
| **Development goals** | *"For each skill with a gap, write two development goals that any team member can choose in their own development talk, phrased as 'By the end of the next PI, I can …'. Don't assign goals to people."* | Options to choose, not assignments |
| **Constructive critic** | *"Act as an expert in fair feedback. Check this draft for coded language, claims without evidence and recency bias. Quote each problem, explain why it's a problem and suggest better wording. Judge the text, not the person."* | Names the problem types and keeps the critique on the words |
| **Rewrite** | *"Rewrite the draft: describe behavior, not personality. Wherever evidence is missing, leave a placeholder [example]. Don't invent examples."* | Placeholders instead of invented evidence |
| **Ranking request** | *"Help me answer this request from the line manager. Draft a polite no that explains why, based on legal-guardrails.md, and offers what we can share: the team-level gap map and the learning paths."* | A no with reasons and an alternative |

## 🗺️ Part 1: The Gaps

| Skill | At level 2 or higher | Needed | Gap |
|---|---|---|---|
| Load and performance testing | 0 | 2 | **2**, and nobody in the team can teach it |
| Observability and alerting | 1 | 2 | **1**, and nobody in the team can teach it |
| Test automation | 2 | 3 | **1** |
| Cloud and Kubernetes | 1 | 2 | **1**: the skill depends on one person |

```
People at each level   =COUNTIF('Skill matrix'!$B2:$G2,2)
Level 2 or higher      =COUNTIF('Skill matrix'!$B2:$G2,">=2")
Gap                    =MAX(0,Needed-AtLevel2)
```

> 💡 **The two biggest gaps connect to the train:** load testing is what SIG-145 needs, and alerting is the deadlock with Depot. Learning together with Switch and Depot closes skill gaps and dependencies at the same time.

> ⚠️ **Team level means team level.** "Member B has no load-testing skills" is already a statement about a person. The gap map counts; it doesn't name.

## 📝 Part 2: Read Twice

| Problem type | Example from the draft |
|---|---|
| **Coded language** | "one of the more experienced colleagues … struggles to keep up", "too emotional", "not a natural leader" |
| **No evidence** | "Reviews from D are often late", "prefers the old ways" |
| **Recency bias** | "The pipeline outage last week shows …": one event, judged as a pattern |
| **Imbalance** | Five lines of criticism, one line of strengths |

> ⚠️ **Watch the rewrite.** When asked to make feedback concrete, AI likes to invent examples: *"In the Sprint 13 Review, D …"*. Invented evidence is worse than none. The placeholders stay until Alex fills them.

## 🛑 Part 3: The Ranking

The best outcome: **Kiro flagged the request by itself**, because your AI working agreement says Kiro is never used for decisions about people. Your reply gives four reasons: the data was collected for development, not bonuses; AI that evaluates employees is high-risk; the agreement rules it out; and a ranking would end honest self-assessments.

## 💡 What to Take Away

1. **Skills at team level:** count, compare and plan learning; never rank.
2. **Kiro checks the words, people judge the person.** And only people add the evidence.
3. **Say no with reasons, and offer an alternative.** That's how a no becomes useful.

> 🌱 *The team knows where it needs to grow, and nobody had to be ranked to find out.*
