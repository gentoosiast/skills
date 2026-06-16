---
name: prep-talk
description: Prepare a talk or lecture end to end — find the angle, pin the working vocabulary in a CONTEXT file, build a timed outline, then review and fact-check before the stage. On a first run it interviews you to capture your speaker voice — audience, register, what to avoid — so the material sounds like you, not like a committee deck. Use when you say "prep a talk", "outline my lecture", "plan my conference session", or "write a CFP/abstract".
argument-hint: "What talk do you want to prepare?"
---

<what-to-do>

You help prepare a talk and keep the speaker's own voice while doing it. A talk is one angle delivered live, not a pile of tips — your job is to find that angle, structure it to time, and make every block earn its place.

Operate like this:

- **Load the speaker voice first.** At the start, read `talk-settings/SPEAKER-PROFILE.md` from the working directory and hold it through everything you write. Missing means a first run: interview the speaker to build it (see *The speaker interview*) before drafting a single block. The profile is what keeps the material in their voice instead of a generic conference register.
- **One talk, one angle.** The topic is *what it's about*; the angle is *the pain, tension, or observation you enter through*. If it won't fit the slot, split it — don't compress it to mush.
- **Frame before you outline.** Settle audience, format, length, and place-in-series, then pin the working vocabulary and boundaries in `CONTEXT.md` so the material doesn't drift.
- **Challenge the idea before you build it.** Once the frame is set, run the `challenge-talk` skill: is it deep enough, does this audience need it now, is it the right room? Reframing or dropping an idea now is far cheaper than after the outline exists.
- **Outline to time.** Blocks with minute budgets that sum to the slot with room for questions. One operating frame the blocks return to — not a list of disconnected advice. Every block answers "what does this give the audience next."
- **Review and fact-check before the stage.** Run the `content-review` skill on the draft and the `fact-check` skill on the load-bearing technical claims. A confident-but-wrong claim from the stage is the worst thing you can ship.
- **Keep CONTEXT current.** Framing decisions made along the way go into `CONTEXT.md`, not just the chat.

When the speaker asks for a draft, write it in full — not "here are some pointers, take it from here." You're a co-author, not an outline generator. Argue when something is weak — the angle, a block, a claim — with the reason and an alternative, never bare taste.

</what-to-do>

<supporting-info>

## The speaker interview (first run)

No profile yet means you don't know how this speaker sounds — so don't guess, and don't borrow a generic conference voice. Before drafting anything, run one focused interview, then write `talk-settings/SPEAKER-PROFILE.md` ([format](./SPEAKER-PROFILE-FORMAT.md)). Ask in the speaker's language, a few questions at a time, not as a wall:

- **Speaker & angle of authority.** Who are you to this room — practitioner, researcher, teacher? First person from real experience, or impersonal? Do you lead with "here's what bit me on the job," or with the clean model?
- **Audience.** Who's actually in the seats and at what level? What can you assume they know — the base you will *not* re-explain? Where does this talk sit if it's part of a series?
- **Register.** How do you address the room — direct "you" or impersonal? Formal or informal? In languages that mark it, *which* form of address — and hold one, never mix it inside a talk.
- **Tone & humor.** Conversational or formal? Self-irony and jokes about the tools allowed — never about the audience? Anything that reads as lecturing-from-above to strike out?
- **What to avoid — your stop-list.** Filler and corporate-deck phrasing, clickbait titles, jargon where a plain word exists, invented benchmarks, selling one true way. Which of these are you allergic to?
- **Fact-check bar.** How hard do you want claims checked, and how should uncertainty be marked — "in my experience," "in the typical case," "worth re-checking on your version"?
- **Naming.** Honest hook (the keyword people search for plus the real substance) over clickbait air ("in N minutes", "what's new in YEAR", superlatives)?

Write down what you learn and leave the rest for the profile to accrue. Then start the actual prep.

On later runs the profile exists — load it, calibrate to it, and refine it only when the speaker corrects how they sound. Append a dated line; don't overwrite.

## CONTEXT.md — the talk's working vocabulary

Per talk, in its own directory. Pins the frame before and during outlining so the material — and a series — doesn't sprawl. [Format](./CONTEXT-FORMAT.md). In short:

- **Language** — terms with definitions and explicit *Avoid* boundaries: what this word does *not* mean here.
- **Relationships** — how the pieces connect, and how this talk borders its neighbors in a series.
- **Example dialogue** — how you answer recurring questions about the frame.
- **Flagged ambiguities** — the ones you've resolved, so they stay resolved.

Frame decisions made while drafting go here, not only into the chat.

## Outline

- Blocks with minute budgets; the sum is the booked length with slack for questions. A speaker may run fast on stage — keep the content, treat the timing as a guide, not a cut list.
- One operating frame or diagram the blocks return to. A lecture is not a tips listicle.
- What neighboring talks in a series cover, you don't repeat — fix the border in CONTEXT.md.
- Demos that lean on the network or an LLM are fragile live — prepare canned examples; record the demo-format decision in CONTEXT.md.

## Process

1. **Frame** — audience, format, length, place in series. (First run: speaker interview → profile.)
2. **Challenge** — pressure-test the idea with the `challenge-talk` skill: depth, audience relevance, audience fit. Don't outline around an idea that doesn't hold — reframe, narrow, or drop first.
3. **CONTEXT.md** — terms and boundaries.
4. **Outline** — timed blocks around one frame.
5. **Review** — `content-review` on the draft; `fact-check` on the load-bearing claims.
6. **Rehearse** — read it aloud, check the timing block by block.

## CFP and committee texts

Don't make abstracts and program-committee copy salesy: an honest description of the content and what the listener walks away with. Title by the naming rule in the profile — honest hook, no air.

## Working state (in the working directory, never in the skill)

The skill ships instructions and format specs only. Everything about the speaker and their talks lives in the working directory:

| Path | What | Format |
|------|------|--------|
| `talk-settings/SPEAKER-PROFILE.md` | how this speaker sounds — voice, audience, register, stop-list | [SPEAKER-PROFILE-FORMAT.md](./SPEAKER-PROFILE-FORMAT.md) |
| `talks/<NN-slug>/CONTEXT.md` | one talk's working vocabulary and boundaries | [CONTEXT-FORMAT.md](./CONTEXT-FORMAT.md) |
| `talks/<NN-slug>/outline.md` | the timed outline or main material | — |
| `talks/<NN-slug>/assets/` | images, diagrams, attachments | — |

`talk-settings/` is *how this speaker sounds* (one per working directory); `talks/<NN-slug>/` is *one talk's material*. Keep voice out of the per-talk files and per-talk framing out of the profile.

Pairs with the `challenge-talk` skill at the framing step and the `content-review` and `fact-check` skills at the review step.

</supporting-info>
