# Progress log format

A ledger of covered ground so a session can end and the next resume without re-treading. **One file per topic** — a topic is a whole subject ("solving the Rubik's cube", "React hooks"), not a single concept within it. The file accumulates the concepts mastered inside that topic plus a live pointer to where to pick up.

Lives in `education-progress/` in the working directory, one file per topic, named with an ASCII kebab-case slug of the topic (e.g. `sborka-kubika-rubika.md`, `react-hooks.md`). Content is in the learner's language.

## Structure

```md
# <Topic> — <in progress | completed>

## Covered
- <a concept the learner now owns within this topic> <!-- YYYY-MM-DD -->

## Resume here
- <where we stopped · the next probe to open> <!-- YYYY-MM-DD -->
```

## Rules

- **One file per topic.** A new subject is a new file, not a new section. Within a topic, concepts are bullets under *Covered*.
- **Covered grows append-only.** Add a concept the moment its check passes — quick-check questions *and* the mini explain-back in the learner's own words, per SKILL.md. A concept the learner could answer but not reconstruct isn't covered yet. Don't rewrite or delete past entries — they are the proof of what's solid.
- **Resume here is a single live pointer.** Rewrite it after each concept closes and at session end, so stopping mid-topic loses nothing. Name where you stopped *and* the next probe to open — enough that a cold start picks up without re-asking.
- **Record understanding, not activity.** "Derived that one turn moves 8 pieces at once" is signal; "we talked about turns" is not. The best signal is what the learner *reconstructed* in their own explain-back, not what you told them.
- **Mark the topic completed** in the H1 only after both closing gates pass cleanly — the full explain-back reconstructs the core *and* the targeted questions land (per SKILL.md). Until then it stays *in progress* — that's how the next session knows which file to resume.

This log is the *what* (coverage); the profile is the *how* (learning style) — keep them in separate files.
