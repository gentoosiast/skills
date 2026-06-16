---
name: fact-check
description: Verify technical claims against primary sources — docs, source code, changelogs, reproducible examples — and mark what couldn't be verified instead of masking it with a confident tone. Use when you say "fact-check this", "verify these claims", doubt a technical statement, or before shipping material with disputed claims.
argument-hint: "What claims should I verify?"
---

# Fact-check against primary sources

## Procedure

1. Pull every statement that reads as a technical fact: API behavior, numbers, comparisons, versions, limits.
2. Classify each: fact / personal experience / hypothesis. Experience and hypotheses must be marked as such ("in my experience", "seems like") — they can't read as law.
3. For each fact, find a primary source: official docs, source code, changelog, RFC, issue, or a reproducible example. A secondary retelling (a blog, a chat) is a lead to the source, not proof.
4. Verdict per claim: confirmed (with the source) / refuted (and what's actually true) / couldn't verify.
5. Fix: correct what's refuted; soften the unverified to experience or hypothesis, or cut it; reframe an unproven "X is faster than Y" into the logic of a concrete scenario.
6. Report back: claim → verdict → source. Name the unverified plainly — don't mask it with a confident tone.

## What to check with

- **Web:** official docs, the project repository, changelogs, RFCs.
- **Code:** a short reproducible example right here (a REPL, a sandbox) — often faster and more reliable than searching.

## Red flags

- "always / everywhere / in all versions" — often the residue of compression that dropped the reason.
- A pretty claim you'd rather not check — check it first (confirmation bias).
- A number with no measurement method behind it.
- A comparison ("X is cheaper / faster than Y") stated as a general law from a single case.
