---
name: content-review
description: Final read-through of any prose before it ships — a sound pass for AI tells and machine rhythm, an argument pass for whether the claims actually hold, and a register/cohesion pass. Returns specific notes — what's not working and how you'd fix it — not vibes. Use when you say "review this", "read it before I publish", "check for AI tells", or hand any draft for a final pass.
argument-hint: "What should I review?"
---

# Content review

Three passes over any draft, plus a format check. The output is a list of concrete notes — what specifically fails (the hook, the structure, a claim, filler, the ending) and "here's how I'd do it instead" — never bare "I don't like it."

If a `SPEAKER-PROFILE.md` or a house-style file is present in the working directory, read against it too: the register, voice, and stop-list it sets are part of the bar.

## Pass 1 — how it sounds (AI tells)

The strongest tell isn't a word, it's rhythm and symmetry. Look there first; lexicon second. Full checklist: [AI-TELLS.md](./AI-TELLS.md).

- **Rhythm and symmetry first.** Balanced antitheses ("not X, but Y") — one or two is a device, six in a row is a machine. Anaphora chains. Even grids of identical sections. Triads on autopilot.
- **Then lexicon.** Filler connectives ("it's worth noting that"), empty intensifiers ("truly", "the very"), nominalized bureaucratese, stock metaphors, summary endings that just restate.
- **Unsupported sweep.** "Everyone / most / often / it's accepted that" with no basis — cut it or mark it as opinion.
- **Don't sterilize.** Author hedges ("in my experience"), one-off qualifiers, apt jargon, and live "was X → became Y" images carry the voice — touch them last. See AI-TELLS.md, "Don't touch."
- **Final filter:** would a person say this out loud?

## Pass 2 — what it stands on (the argument)

Run the load-bearing claims — the strongest first — through the argument check. Full checklist: [ARGUMENT-CHECK.md](./ARGUMENT-CHECK.md).

1. Confidence level marked: fact / experience / hypothesis.
2. Basis visible — and relevant, sufficient, reliable.
3. No logical fallacy (ad populum, false dilemma, hasty generalization, correlation-as-cause, straw man, …).
4. No author bias dressed as fact (confirmation, novelty, survivorship, anchoring).
5. Steelman done if something is being criticized.
6. "Where it breaks" names real limits, not a token disclaimer.
7. No apparent self-contradiction left unexplained (a claim that flips "cheap → not free" must show the scale changed — a unit vs a sum — not the fact).

A found hole gets closed with a basis, softened to a hypothesis, or cut. A disputed technical claim goes to the `fact-check` skill — not a confident tone.

## Pass 3 — register and cohesion

- One register throughout — forms of address not mixed (check against the profile if there is one).
- Every block answers "what does this give next"; name the "so what?" blocks that just hang.
- The title passes the honest-hook test: it promises exactly what the material delivers, no air.

## Format check

If the piece has a format with its own checklist (a post, a talk, a lesson, a video), run it against that. A talk, for example: block timings sum to the booked length; the frame and terms don't contradict the CONTEXT file; nothing repeats a neighboring talk in the series. Keep format rules in the material or its skill, not here — this skill is format-agnostic.
