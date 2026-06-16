# content-review

A final read-through for any draft before it ships. Three passes — how it *sounds*, what it *stands on*, and whether the register holds — returning concrete notes, not vibes.

## Why

Two different things sink a draft: it reads like a machine assembled it, or it makes a confident claim that doesn't hold. This skill checks both, separately, because they have different cures — a rhythm problem gets rewritten, a weak argument gets a basis or gets cut.

## What it does

- **Sound pass.** Hunts AI tells — machine rhythm and symmetry first ("not X, but Y" stacked six deep, even section grids, autopilot triads), lexicon second. Yellow flags, not auto-replace: it won't sterilize your voice. Checklist: [AI-TELLS.md](./AI-TELLS.md).
- **Argument pass.** Runs the load-bearing claims through a critical-thinking check — confidence level, visible basis, logical fallacies, your own biases, steelman. Checklist: [ARGUMENT-CHECK.md](./ARGUMENT-CHECK.md).
- **Register pass.** One form of address throughout, every block earning its place, an honest-hook title.

## How to use it

Hand it a draft:

> review this before I post it

If a `SPEAKER-PROFILE.md` or house-style file is in the working directory, it reads against that too. A disputed technical claim is handed off to the `fact-check` skill rather than waved through.

## Install

With [`npx skills`](https://github.com/vercel-labs/skills):

```sh
npx skills add ArchieSA/skills/content-review
```
