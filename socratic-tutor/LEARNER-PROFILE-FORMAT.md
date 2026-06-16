# LEARNER-PROFILE.md format

A living record of how *this* learner learns — used to calibrate difficulty, pick the right hint, and avoid re-explaining what's already solid. The teaching analogue of the notes you'd keep on a long-running student.

Part of the tutor settings: lives at `tutor-settings/LEARNER-PROFILE.md`, one per working directory. Create it lazily — only once you have a real observation, never on session start.

## Structure

```md
# Learner profile

## Background
- <prior knowledge, role, depth — what NOT to re-explain, and from what level to start>

## How they learn best
- <techniques that landed: mini-checks, tables for asymmetric rules, analogies, …> <!-- YYYY-MM-DD -->

## Watch for
- <recurring failure modes: almost-right summaries, guess-without-checking, vocabulary gaps, …> <!-- YYYY-MM-DD -->
```

## Rules

- **One observation per bullet** — concrete, with a dated `<!-- YYYY-MM-DD -->` comment.
- **Append, never overwrite.** Past entries show how the learner evolved and protect against regressions. A superseded observation gets a new dated bullet, not a deletion.
- **Record signal, not activity.** "Collapsed an asymmetric rule into a symmetric one in their recap" is signal. "Asked about X" is not.
- **No topics here.** What's been covered and what's next belong in the per-topic progress log (`education-progress/`), not the profile. The profile holds only how/what to teach this learner and notes about them — keep curriculum out.
- **Both polarities.** Log what works (so you repeat it) *and* what to watch for (so you catch it earlier next time).
- **Keep it short enough to read at the start of every session.** A profile too long to skim stops getting read.
