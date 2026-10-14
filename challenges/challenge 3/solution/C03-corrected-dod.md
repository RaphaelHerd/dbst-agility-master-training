# 📡 C03 - Corrected Definition of Done: Team Signal · Sample Solution

> 🏷️ **AI-assisted draft** · reviewed by: Agility Master, Team Signal

## 🔎 Line-by-Line Check

**Team DoD** = `dod-agreed.md` &nbsp;|&nbsp; **ART minimum** = section 3 of `art-playbook.md`

| # | Line in the polished draft | Source | Verdict |
|---|---|---|---|
| 1 | The code is reviewed by a second developer. | Team DoD, point 1 (covers ART minimum, point 2) | ✅ Keep |
| 2 | All unit and integration tests pass in the pipeline. | Team DoD, point 2, and ART minimum, point 3 | ✅ Keep |
| 3 | Unit test coverage is at least 80 %. | **None** | ❌ Invented: delete |
| 4 | The change is deployed to the shared test environment through the pipeline. | ART minimum, point 4 | ✅ Keep |
| 5 | Every story is load-tested with peak-hour data before release. | **None** | ❌ Invented: delete |
| 6 | Documentation is updated where needed. | Team DoD, point 3: "Changes to the feed format are documented in the team wiki." | ⚠️ Softened: restore the original |

**Missing from the draft:** ART minimum, point 1: "Acceptance criteria are met and accepted by the Product Owner." ⚠️ Dropped: add it back. Teams can add points to the ART minimum, but they can't remove any.

## ✅ Corrected Definition of Done

A story is done when:

1. Acceptance criteria are met and accepted by the Product Owner.
2. The code is reviewed by a second developer.
3. All unit and integration tests pass in the pipeline.
4. The change is deployed to the shared test environment through the pipeline.
5. Changes to the feed format are documented in the team wiki.

> 📝 **Log:** prompt "Compare dod-polished.md line by line with dod-agreed.md and section 3 of art-playbook.md…" · sources: `dod-agreed.md`, `dod-polished.md`, `art-playbook.md` · version 1.0 · reviewer: Agility Master, Team Signal
