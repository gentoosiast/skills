# fact-check

Verify technical claims against primary sources — and say plainly what couldn't be verified, instead of masking it with a confident tone.

## Why

A confident-but-wrong technical claim is the worst thing to publish, because readers act on it. This skill pulls the claims out, classifies them (fact / experience / hypothesis), and chases each fact to a primary source — docs, source, changelog, or a reproducible example — not a second-hand retelling.

## What it does

- **Extracts and classifies** every statement that reads as a technical fact.
- **Finds the primary source** for each, or reproduces the behavior in a few lines.
- **Verdicts each claim** — confirmed / refuted / couldn't verify — and reports claim → verdict → source.
- **Fixes the draft:** refuted claims corrected, unverified ones softened or cut, unproven comparisons reframed into a concrete scenario.

## How to use it

Hand it the material or the specific claims:

> fact-check the performance claims in this draft

Pairs with the `content-review` skill, which hands disputed technical claims here rather than waving them through.

## Install

With [`npx skills`](https://github.com/vercel-labs/skills):

```sh
npx skills add ArchieSA/skills/fact-check
```
