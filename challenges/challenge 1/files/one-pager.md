# 📡 Team Signal - Team One-Pager

> Confluence page · ART SmartTransfer · Real-time train data

## Who We Are

Team Signal delivers the real-time backbone of SmartTransfer: live train positions, delays and platform changes, cleaned up and passed on to the other teams within seconds.

## Team

| Name | Role |
|---|---|
| Alex | Product Owner |
| You | Agility Master |
| Member A | Backend developer |
| Member B | Backend developer |
| Member C | Data engineer |
| Member D | Data engineer |
| Member E | Tester |
| Member F | DevOps engineer |

## Events

| Event | When |
|---|---|
| Daily | Every working day, 09:15, 15 minutes |
| Refinement | Wednesday, 13:00, 60 minutes |
| Sprint Review | Every second Thursday, 14:00 |
| Retrospective | Every second Thursday, 15:30 |
| Sprint length | 2 weeks |

## What We Give and What We Need

| Direction | What | Team |
|---|---|---|
| We deliver | Live delay feed for transfer calculations | Switch |
| We deliver | Platform-change events for push notifications | Concourse |
| We need | Streaming platform and monitoring | Depot |

## Current Focus This PI

- **Delay feed v2:** reduce latency from 60 to 15 seconds.
- **Platform-change events** for all major stations.
- **Stable integration tests** with the train data provider.

## How We Work

- All team documents are written in English.
- Messages are short: facts first, then the ask.
- Definition of Done: code reviewed, tests green, documented in the team wiki.

## Open Topics

- Who owns the platform-change events once they are live: Signal or Concourse?
- Flaky integration tests slow down every release.
