# 📡 Decision Needed: Test Data for Feed v2

> Note from Alex, Product Owner, Team Signal · input for the steering committee paper

## ❓ The Decision

Should the steering committee escalate the late test data to the train data provider, or accept that delay feed v2 goes live without a peak-hour load test?

## 📋 Background

- Delay feed v2 runs in the test environment at 22 seconds. Our target for this PI is 15 seconds.
- The load test with peak-hour data (SIG-145) could not run: test data from the provider arrived late, for the third sprint in a row.
- Team Switch's transfer calculations use our delay feed.

## ⚖️ Options

| Option | What happens | Consequence |
|---|---|---|
| **A · Escalate** | The steering committee asks the provider to deliver test data two weeks before each sprint | Fixes the cause. Feed v2 goes live after the load test, once the data has arrived |
| **B · Go live without the load test** | Feed v2 goes live after the functional tests | Faster. How the feed behaves at peak hours stays unknown until it happens in production |
| **C · Build our own test data** | Two data engineers create synthetic peak-hour data | Independent of the provider. Takes about one sprint for two data engineers, which the PI focus loses |

## ✅ My Recommendation

**Option A.** It fixes the cause instead of the symptom. Option B is a risk for passengers at peak hours, and option C costs two people a full sprint.

Alex
