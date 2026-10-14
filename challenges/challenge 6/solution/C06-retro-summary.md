# 🔄 C06 - Retro Board Summary: Team Signal · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

> Confluence page · Team Signal · input for the next Retrospective · 40 anonymous notes, 79 dot votes · team level only

## 🗂️ Topics

| Topic | Notes | Votes | 😊 | 😐 | 😟 | In short |
|---|---|---|---|---|---|---|
| Test data | 8 | 22 | 1 | 2 | 5 | Late test data costs days every sprint, and nobody owns the topic |
| Meetings and focus time | 7 | 18 | 1 | 2 | 4 | Wednesdays leave no time for focused work |
| Flaky tests and pipeline | 6 | 13 | 1 | 1 | 4 | Flaky tests and a red pipeline cost hours; testing gets squeezed at the end of the sprint |
| Dependencies on other teams | 6 | 12 | 1 | 2 | 3 | Waiting for Depot, an open question with Concourse, no date for Switch |
| Teamwork and learning | 7 | 9 | 5 | 1 | 1 | Strong pairing and help; knowledge of the feed sits with few people |
| Working with Kiro | 3 | 3 | 1 | 1 | 1 | Useful, but people want clarity on what goes in and what is monitored |
| Visibility and recognition | 3 | 2 | 2 | 0 | 1 | Good feedback from Kim and Rail Ops; the work is invisible until something breaks |
| **Total** | **40** | **79** | **12** | **9** | **19** | |

## 🔁 Patterns

- **Test data** is a top topic for the **fourth retro in a row** (Sprints 12, 13, 14 and now). The earlier actions had no owner.
- **Meetings on Wednesdays** came up in Sprints 12 and 14 and now again. "Move Refinement to Tuesday" is still not done.
- **Flaky tests** came up in Sprint 13. Progress is visible (3 of 7 tests stable), but the topic is back.
- The old board got fewer notes each time (31, 27, 22, 18). The anonymous board got **40**.

## ⚖️ Bias Check

- **Not just negative:** 12 of 40 notes are positive. Positive notes get few votes, so a summary built on votes alone looks gloomier than the team is.
- **Mood labels are judgments:** "meeting hell" and "I would love one meeting-free afternoon" ask for the same thing. Several notes are borderline, for example notes 5, 12 and 32.
- **Who is missing:** no notes about the work with the PO, about Rail Ops or about passengers. Silence is not proof that all is well.
- **No pointers to people:** two notes mention a role that only one person has. The summary keeps the topic and drops the role.

## ✅ Three Actions

| Action | Owner | Measure | Review |
|---|---|---|---|
| Ask the provider for test data two weeks before each sprint, with the steering committee's backing | Alex | Test data arrives at least 10 working days before the sprint starts | Sprint 16 retro |
| Move Refinement to Tuesday and keep Wednesday afternoons free of team meetings | Agility Master, with Alex | No team meetings on Wednesday afternoons in Sprints 16 and 17 | Sprint 17 retro |
| Fix two flaky integration tests per sprint before new feature work | Member A | 7 of 7 integration tests stable by the end of Sprint 16 | Every retro until done |

**Parked for the ART Sync:** the deadlock with Depot (12 votes for the topic). We can start by sending our alert definitions first.

> 📝 **Log:** prompt "Cluster these 40 anonymous notes into at most seven topics…", counts checked in Excel · sources: `retro-board.csv`, `retro-history.md` · version 1.0 · reviewer: Agility Master, Team Signal
