# 🔀 Decision Needed: Feed v2 in Our Test Environment

> Note from Sam, Product Owner, Team Switch · input for the steering committee paper

## ❓ The Decision

Should providing delay feed v2 in Team Switch's test environment become a train-level priority for the next sprint?

## 📋 Background

- Switching to delay feed v2 (SWI-216) is our top priority, but feed v2 is not yet available in our test environment. There is no agreed date with Team Signal.
- Our recommendations take 320 ms instead of 200 ms (SWI-219). The 200 ms target is at risk if feed v2 arrives late.
- Our transfer recommendations are shown to passengers in the app, which Team Concourse builds.

## ⚖️ Options

| Option | What happens | Consequence |
|---|---|---|
| **A · Train-level priority** | Team Signal provides feed v2 in our test environment in the next sprint | We can switch and work toward the 200 ms target. Team Signal has to plan this work, and other work moves |
| **B · Wait** | We keep working with the current feed until Team Signal is ready | No change for other teams. The 200 ms target may slip to the next PI |
| **C · Simulate** | We build a feed v2 simulator for our tests | Independent of Team Signal. Takes about half a sprint for two developers, and the simulator may behave differently from the real feed |

## ✅ My Recommendation

**Option A.** Feed v2 is the basis for the 200 ms target, and only a train-level priority gets us a date.

Sam
