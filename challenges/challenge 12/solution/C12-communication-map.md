# 📞 C12 - Communication Map: The Alerting Deadlock · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

**Top dependency:** Signal's outage alerting (SIG-P3) needs Depot's monitoring rules (DEP-P2), and those need alert definitions that no item delivers.

## 🗺️ Who Talks to Whom

```
Member A (Signal) ------ alert definitions, rules ------> Depot's site reliability engineers
Alex (PO Signal) ------- scope, sprint, who does what --> Charlie (PO Depot)
Agility Master Signal -- prepare the joint session -----> Agility Master Depot
        |
        +-- no agreement by the ART Sync? --> Kim (RTE) --> PI Planning
Informed: Team Switch, Team Concourse, Rail Ops
```

| Who | With whom | About what | How | By when |
|---|---|---|---|---|
| Member A, dev lead Signal | Depot's site reliability engineers | Alert definitions and monitoring rules | Joint working session | Sprint 1 |
| Alex, PO Signal | Charlie, PO Depot | Scope, sprint and who does what | Direct conversation | Before PI Planning |
| Agility Master Signal | Agility Master Depot | Prepare and facilitate the joint session | Short call | Tomorrow |
| Kim, RTE | Both POs | Who owns alert rules on the train; one version of wiki pages 10 and 11 | ART Sync | Tomorrow |
| Team Switch and Team Concourse | Informed | They use the feed: outages will be detected automatically | ART Sync notes | After the agreement |
| Rail Ops | Informed | Outages of delay information will be noticed sooner | Short note, plain language | When the alerting is live |

## 🪜 If They Can't Agree

1. **Alex and Charlie** agree directly.
2. **Kim** decides ownership in tomorrow's ART Sync.
3. Still open? It goes on the risk list for **PI Planning**.

> 📝 **Log:** prompt "For this dependency, map who needs to talk to whom…" · sources: `train-backlog.csv`, `wiki-alerting.md` · version 1.0 · reviewer: Agility Master, Team Signal
