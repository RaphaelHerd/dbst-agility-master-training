# 📥 C02 - The Monday Inbox

> 👥 **Group work** &nbsp;|&nbsp; 🗓️ **Day 1** · Story day T-10 &nbsp;|&nbsp; 🛠️ **Kiro:** chat, context, your steering file

## 📖 Context

It's still Monday morning. Five mails are waiting in your inbox, and every sender wants a precise answer **before 10:00**: Kim, Alex (your PO), Member B from your team, Robin from the works council and Sascha from Finance. Sascha's mail is the tricky one: a risk message for the steering committee.

You know the answers. Kiro can write them faster, but only **if you ask precisely**.

## 🎯 Your Goal

- Answer five mails, each in the form its reader needs.
- Use the **7 principles**, **role prompting** and a **defined output**, so that Kiro's drafts need little rework.
- For the risk message, let Kiro draft **two tones**, then choose one and explain why.

## 📂 Your Inputs

| File | What's inside |
|---|---|
| `files/inbox.md` | The five mails |
| `files/one-pager.md` | Your team one-pager from C01 |
| `files/sprint-notes.md` | Your Sprint 14 notes from C01 |

## ✅ Your Tasks

### ✉️ Part 1 - Three Quick Replies

1. Add the `files` folder to the chat (type `#` and choose **Folder**). Your steering file from C01 is active, so Kiro already knows your team.
   > 💡 No steering file yet? Use the sample in `challenge 1/solution/team-context.md`.
2. **Kim's mail.** First, try a lazy prompt and look at what comes back:
   > 💬 *"Answer Kim's mail."*

   Then apply the principles: be concise and clear, give context and specify the output.
   > 💬 *"Answer Kim's mail from inbox.md in one sentence of at most 40 words: did we reach our Sprint 14 goal, and what is our biggest blocker? Use only sprint-notes.md and name the item ID."*
3. **Alex's mail.** Define the output exactly:
   > 💬 *"Answer Alex's mail with three bullets of at most 20 words each: only what we didn't finish in Sprint 14, with item IDs. No introduction."*
4. **Member B's mail.** Use role prompting:
   > 💬 *"You are an experienced Agility Master who explains things to developers without lecturing. Reply to Member B's mail in at most 80 words: friendly, honest and with one concrete example from our sprint notes."*
5. **Check every reply against the files.** Mark everything Kiro states that is not in the sources.

### 🛡️ Part 2 - Two Sensitive Replies

1. **Robin's mail.** Answer both questions in at most 80 words, formal and precise. Write only what is true today, and delete any promise you can't keep.
2. **Sascha's mail.** Let Kiro draft your team's biggest risk in two tones:
   > 💬 *"Draft a reply to Sascha's mail in at most 80 words: the risk, what it affects, and what we need from whom. Write two versions: one calm and reassuring, one direct and urgent. Use only facts and numbers from our files."*
3. **Choose one version** and explain in one sentence why it fits the steering committee. Change it if you need to.
4. Optional: let Kiro play the reader.
   > 💬 *"Act as a member of the steering committee. Read both versions. Which one helps you decide, and what is missing?"*
5. Add the **AI label** and a **log line** to your replies.

> 💡 **Tip:** If an answer misses the mark, don't argue with Kiro. Sharpen the prompt and run it again. That's principle 6: reflect and adapt.

> 📚 **Kiro docs:** [Chat](https://kiro.dev/docs/ide/chat/) covers adding files and folders as context. [Steering](https://kiro.dev/docs/steering/) explains why Kiro already knows your team.

## 📦 Deliverables

| Deliverable | Where it goes |
|---|---|
| `C02-replies.md`: five checked replies, both versions for Sascha and your choice with a reason, with **AI label** and **log line** | Your results folder |
| **One sentence** for the debrief: which principle made the biggest difference? | Debrief |

## 🗣️ Debrief

- What did the lazy prompt produce, and what changed with the precise one?
- Which tone did you choose for Sascha, and why?
- Did Kiro add anything to Robin's reply that you had to delete?

## 🔗 Where This Leads

Today you checked Kiro's answers against your own files. In **C03 · The Near-Miss**, you check AI answers that someone else almost trusted.

> 📥 *A precise prompt is short, gives the right context and defines the output. The more precisely you ask, the less you have to fix.*
