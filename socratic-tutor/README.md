# socratic-tutor

A tutor that refuses to hand you the answer. It teaches a technical topic by making *you* reason it out — probing questions one at a time, escalating hints, docs-reading practice — so the understanding is one you built and can keep, not one you were handed and will forget.

## Why

A concept you reconstruct yourself sticks; a concept explained *at* you evaporates. So this skill is deliberately anti-spoonfeed: ask "just write the code" or "just give me the answer" and it refuses — warmly, with a hint or a question instead. That refusal is the feature, not a failure of it.

## What it does

- **Never hands over the solution.** Leads you to it with questions, not lectures.
- **One probe at a time.** Asks, waits, and treats a wrong answer as a window into the mental model that produced it — then dismantles *that*, not just the surface error.
- **Escalating hints.** When you're stuck it climbs a ladder — rephrase → analogy → point at a doc → a few illustrative lines — only as far as it must, never to the working answer.
- **Trains docs-reading.** "Is X possible?" gets you sent to the source to report back, not an answer from memory — building the "go read" reflex.
- **Explain-back test.** The core check: you reconstruct the idea in your own words, as if teaching someone who's never seen it. Questions can be passed on recognition; explaining the thing unprompted can't. This is what tells "got through the lessons" apart from "actually understands it" — run as a mini check per concept and a full one before a topic is closed.

## How to use it

Invoke it explicitly and say what you want to understand:

> teach me how DNS resolution works — no spoilers

On a first run in a working directory it agrees on a **tone** with you (gentle and encouraging ↔ blunt and demanding) before teaching. Tone changes *how* it talks to you; it never relaxes the no-answers contract.

## Session state

The skill ships instructions only — everything about *you* lives in your working directory, so sessions can stop and resume cleanly:

| Path | What | Format |
|------|------|--------|
| `tutor-settings/TUTOR-STYLE.md` | the agreed tone | [TUTOR-STYLE-FORMAT.md](./TUTOR-STYLE-FORMAT.md) |
| `tutor-settings/LEARNER-PROFILE.md` | how you learn — traits and teaching notes | [LEARNER-PROFILE-FORMAT.md](./LEARNER-PROFILE-FORMAT.md) |
| `education-progress/<topic>.md` | one file per topic: covered concepts + a resume pointer | [PROGRESS-LOG-FORMAT.md](./PROGRESS-LOG-FORMAT.md) |

`tutor-settings/` is *how to teach you*; `education-progress/` is *what's been covered*. Full behaviour lives in [SKILL.md](./SKILL.md).

## Install

With [`npx skills`](https://github.com/vercel-labs/skills):

```sh
npx skills add ArchieSA/skills/socratic-tutor
```
