# prep-talk

Prepare a talk that sounds like *you*, not like a committee deck. It finds the angle, pins the working vocabulary, builds a timed outline, and reviews and fact-checks the draft before you're on stage — holding your speaker voice the whole way.

## Why

Most talk-prep help hands you a generic conference outline in a generic conference voice. This skill does the opposite: on a first run it interviews you — audience, register, what you refuse to say — and writes that down, so every talk it helps with comes out in your voice and at your audience's level.

## What it does

- **Captures your voice once.** A first run is a short interview — who you are to the room, how you address it, what you won't ship — written to a profile it holds on every later run.
- **One talk, one angle.** Finds the pain or tension you enter through, and splits the talk rather than compressing it to mush when it won't fit the slot.
- **Pins the frame.** A per-talk CONTEXT file fixes the working vocabulary and the borders with neighboring talks, so a series doesn't sprawl.
- **Outlines to time.** Blocks with minute budgets around one operating frame — not a tips listicle — summing to your slot with room for questions.
- **Reviews before the stage.** Runs the companion `content-review` and `fact-check` skills so nothing confident-but-wrong goes out.

## How to use it

Invoke it and say what you're preparing:

> prep my 40-minute talk on React Server Components for a senior audience

On a first run in a working directory it interviews you for your speaker voice before drafting. Later runs load that profile and hold it.

## Working state

The skill ships instructions and format specs only — everything about you and your talks lives in your working directory:

| Path | What | Format |
|------|------|--------|
| `talk-settings/SPEAKER-PROFILE.md` | how you sound — voice, audience, register, stop-list | [SPEAKER-PROFILE-FORMAT.md](./SPEAKER-PROFILE-FORMAT.md) |
| `talks/<NN-slug>/CONTEXT.md` | one talk's working vocabulary and boundaries | [CONTEXT-FORMAT.md](./CONTEXT-FORMAT.md) |
| `talks/<NN-slug>/outline.md` | the timed outline / main material | — |

Pairs with [`challenge-talk`](../challenge-talk) at the framing step, and [`content-review`](../content-review) and [`fact-check`](../fact-check) before the stage. Full behaviour lives in [SKILL.md](./SKILL.md).

## Install

With [`npx skills`](https://github.com/vercel-labs/skills):

```sh
npx skills add ArchieSA/skills/prep-talk
```
