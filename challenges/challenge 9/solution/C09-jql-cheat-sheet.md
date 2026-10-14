# 🔎 C09 - JQL Cheat Sheet · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

**Projects:** SIG, SWI, CON, DEP · **Checked against:** `jira-export.csv`, exported on Wednesday, 7 October

## 1️⃣ Which of our stories are blocked right now?

```
project = SIG AND issuetype = Story AND status = Blocked
```

- **In plain words:** stories of Team Signal whose status is "Blocked".
- **Result:** SIG-145, SIG-147.
- **Almost matched:** SIG-157 is blocked too, but it's a task. SWI-216 is a blocked story of another team.
- **Asked Kim:** "Stories only, or all blocked work?" Without `issuetype = Story`, SIG-157 is in the result.

## 2️⃣ What did the whole train finish last week?

```
project in (SIG, SWI, CON, DEP) AND resolution = Done AND resolved >= startOfWeek(-1) AND resolved < startOfWeek()
```

- **In plain words:** items of all four teams, finished (not cancelled) between Monday and Sunday of last week.
- **Result:** SIG-151, SIG-153, SWI-224, CON-312, DEP-510, DEP-511 (6 items).
- **Almost matched:** DEP-512 was closed as "Won't Do". CON-310 was finished on Sunday, 27 September, the week before. SIG-154 was finished on Monday of this week.
- ⚠️ **Check where your week starts.** Depending on the language settings, Jira's week can start on Sunday. Then DEP-511 (Sunday, 4 October) moves into this week and CON-310 into last week.

## 3️⃣ Which bugs have been open for more than 30 days?

```
project in (SIG, SWI, CON, DEP) AND issuetype = Bug AND statusCategory != Done AND created <= -30d
```

- **In plain words:** bugs of all four teams that are not finished and were created at least 30 days ago.
- **Result:** SWI-198, CON-296, DEP-498.
- **Almost matched:** CON-299 is finished. SIG-150 is 27 days old, CON-314 is 21 days old.
- **Note:** `-30d` counts back from the moment you run the query, so the result changes every day.

## 4️⃣ Which open items wait for another team?

```
project in (SIG, SWI, CON, DEP) AND labels = dependency AND statusCategory != Done
```

- **In plain words:** unfinished items with the label "dependency".
- **Result:** SIG-147, SWI-216, CON-313, DEP-504, DEP-507.
- **Almost matched:** SWI-208 is finished. CON-305 and SWI-222 wait for Rail Ops, which has its own label.
- **Limit:** the query is only as good as the labels. A dependency nobody labeled stays invisible.

## 5️⃣ Which stories in the current sprint have no story points?

```
project in (SIG, SWI, CON, DEP) AND sprint in openSprints() AND issuetype = Story AND "Story Points" is EMPTY
```

- **In plain words:** stories in the running sprint whose story-point field is empty.
- **Result:** SIG-158, SWI-225, CON-315, DEP-514.
- **Almost matched:** SIG-150, SWI-198, CON-314 and DEP-498 are bugs, which have no points on purpose. CON-296 is in no sprint.
- **Note:** in some Jira versions, the field is called "Story point estimate".

> 📝 **Log:** prompts "Here are good and bad JQL examples… Write one JQL query for each of Kim's five questions…", "Explain each query…", "Which rows almost match…" · sources: `jql-examples.md`, `kim-questions.md`, `jira-export.csv` · version 1.0 · reviewer: Agility Master, Team Signal
