# 📡 C05 - Decision Paper: Team Signal · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

> 📘 The content of `C05-decision-paper.docx`. In Word, it fits on one page.

## 🧭 Decision Needed

Should the steering committee escalate the late test data to the train data provider, or accept that delay feed v2 goes live without a peak-hour load test?

## 📋 Background

- Delay feed v2 runs in the test environment at 22 seconds. The target for this PI is 15 seconds.
- The load test with peak-hour data could not run: the provider's test data arrived late for the third sprint in a row.
- Team Switch's transfer calculations use this feed.

## ⚖️ Options

| Option | Consequence |
|---|---|
| **A · Escalate:** the provider delivers test data two weeks before each sprint | Fixes the cause. Feed v2 goes live after the load test, once the data has arrived |
| **B · Go live without the load test** | Faster. How the feed behaves at peak hours stays unknown until it happens in production |
| **C · Build our own test data** | Independent of the provider. Takes about one sprint for two data engineers, which the PI focus loses |

## ✅ Recommendation of the Product Owner

**Option A.** It fixes the cause instead of the symptom. Option B is a risk for passengers at peak hours, and option C costs two people a full sprint.

## ⏳ If No Decision Is Made

The load test stays blocked, and it remains open whether feed v2 can handle peak hours.

## 🤝 Who Is Affected

Team Switch, whose transfer calculations use this feed, and passengers at peak hours. Team Switch is not on the steering committee, so its PO gets this paper before the meeting.

> 📝 **Log:** prompt "You write for a steering committee that has five minutes for this topic. First, give me only the skeleton…" · sources: `decision-needed.md`, `sprint-notes.md` · version 1.1 · reviewer: Agility Master, Team Signal
