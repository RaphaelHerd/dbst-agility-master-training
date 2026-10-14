# 🖋️ Example: `status-update-prompt`

> An example to spark ideas, with a short explanation for each part. Your own instruction will differ. Copy only the instruction itself into your steering file, not the explanations, and don't forget the three lines of front matter at the very top.

| Part of the instruction | Why it helps |
|---|---|
| **Structure:** one-line summary, then *Done*, *Open* and *Next* | Every update looks the same, so readers find things quickly |
| **Reader first:** if I name a reader, adapt length and tone to them. If I don't, ask me who will read it | The same facts need different words for the team, Kim or Rail Ops |
| **Facts only:** use only the files I give you. Mark anything that is unclear as an open question | Prevents invented facts and promises |
| **Numbers:** use numbers exactly as they appear in the source. Never calculate new ones | Language models don't really calculate |
| **People:** never name team members; use pseudonyms (Member A, B …) only where a person is really needed | Data minimization from the start |
| **Length:** at most 120 words, unless I ask for more | Status updates get read when they're short |
| **Label:** end with the line "AI-assisted draft · reviewed by: …" | Readers can see that AI helped and who checked it |

> 💡 **The test:** call the prompt twice with different readers. If the structure holds and only the wording changes, your instruction works.
