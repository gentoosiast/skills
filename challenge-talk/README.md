# challenge-talk

Pressure-test a talk's idea before you build it. A friendly skeptic at the framing stage: it states the strongest version of your idea, pushes on whether it's deep enough, whether this audience needs it now, and whether it's even the right room — then calls a verdict: go, reframe, narrow, or drop.

## Why

Most talk prep starts at the outline and assumes the idea is sound. Often it isn't — it's a docs walkthrough, a topic with no angle, or a session pitched at "everyone." Catching that from the stage costs the room's trust; catching it from a program committee costs the slot. This skill catches it while the idea is still a sentence, when reframing is free.

## What it does

- **Steelmans first.** States the best case for the talk before laying a finger on it — no knocking down a strawman of your own idea.
- **Pushes on three axes.** Depth (could they just google it? what's the twist? what would they retell a colleague?), relevance (whose problem, and is the timing right?), and audience (who's actually in the room, and who is this *not* for?).
- **Names the speaker's blind spots.** Sunk cost, hype, curse of knowledge, confirmation — the biases that make it hard to challenge your own idea.
- **Ends on a verdict, not a questionnaire.** Go, reframe, narrow, or drop — with the reason and the next step.

## How to use it

Invoke it and say what you're considering:

> challenge my talk idea: "everything new in React 19" for a senior frontend audience

If you've used `prep-talk`, it reads the audience and level from your speaker profile and the talk's CONTEXT file. If not, it asks about the room, slot, and venue first, then challenges against real answers.

## Working state

The skill ships instructions and the criteria file only — it holds no state. The audience and voice come from the `prep-talk` artifacts; the verdict lands back in the talk's `CONTEXT.md`.

| Path | What |
|------|------|
| [SKILL.md](./SKILL.md) | how to run the challenge and call the verdict |
| [CHALLENGE-CRITERIA.md](./CHALLENGE-CRITERIA.md) | the sharp questions under each axis, and the verdict rubric |

Pairs with [`prep-talk`](../prep-talk) as the gate on the way *in* — `content-review` and `fact-check` are the gate on the way *out*, once a draft exists.

## Install

With [`npx skills`](https://github.com/vercel-labs/skills):

```sh
npx skills add ArchieSA/skills/challenge-talk
```
