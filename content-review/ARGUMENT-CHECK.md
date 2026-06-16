# Argument check: what the text stands on

The companion to [AI-TELLS.md](./AI-TELLS.md). That file is about how the prose *sounds*; this one is about whether the *thinking* holds — the anatomy of an argument, the quality of the evidence, the common reasoning errors, and your own biases. In the spirit of Tom Chatfield's *Critical Thinking*.

Why it matters: technical content gets carried into real projects. A strong claim with no foundation is the worst thing to publish. Hold this bar both when reviewing and when proposing a claim yourself.

## 1. Levels of confidence

Separate what you **know**, what you **believe**, and what you **assume** — and make it visible in the text.

- **fact** — a checkable statement (API behavior, a number from a primary source);
- **experience** — "this is how it played out for me in production";
- **hypothesis** — "seems like it's because…".

Mark it honestly: "in my experience", "in the typical case", "worth re-checking on your version". Don't pass experience off as universal law.

## 2. Anatomy of an argument: claim → grounds → inference

Every argument is a conclusion plus premises plus the step between them. Before asserting, lay it out: what's the conclusion, what does it rest on, does the step hold?

Rule for any piece: every strong claim has a **visible basis** — an example, a number, an observation, or a link. No basis means it's taste, not a claim — cut it or mark it as opinion.

## 3. Evidence quality

Not every "basis" works. Check three axes:

- **relevance** — does the support bear on the claim? (a JSON-parsing benchmark says nothing about render speed);
- **sufficiency** — one case is not a law; "worked on my side project" doesn't settle it for production;
- **reliability** — a primary source (docs, source, changelog, a reproducible example) beats "heard it in a chat" and second-hand retellings.

Don't invent benchmarks or numbers. No proof, no claim.

## 4. Logical fallacies

- **appeal to the crowd (ad populum):** "everyone moved to X" — backed by what, and does it matter to the argument?
- **appeal to authority:** "the framework's core team recommends it" — relevant expertise is a reason, not a proof; tell expertise apart from a name-drop;
- **false dilemma:** "either X or pain" — there's almost always a middle;
- **straw man:** arguing against a weaker claim than the one actually made;
- **hasty generalization:** "tried it on one project → no good for anyone";
- **correlation ≠ cause:** "rewrote it in Rust and it got faster" — did the algorithm change too?
- **ad hominem:** attacking the author of an approach instead of the approach;
- **slippery slope:** "one `any` and you slide back to untyped everything";
- **circular / "obviously":** the claim justifies itself or hides behind "everyone knows".

## 5. Your own biases

The author's and reviewer's, not the reader's:

- **confirmation** — hunting only for the upsides of a favored tool;
- **novelty / hype** — new looks better just for being new;
- **survivorship** — you see the successful migrations, not the abandoned ones;
- **anchoring** — the first benchmark number sticks and drags the conclusions;
- **sunk cost** — "we already invested in X, so X is good".

## 6. Steelman the other side

Before hitting a tool or approach, state the **best** case for it — not the easiest one to knock down. If you can't state the strong version, you don't understand it yet, and it's too early to criticize.

## 7. Rhetoric vs argument

Moves that persuade around the reasoning: a confident tone in place of proof, rhythm and triads, crowd pressure, emotion, a pretty metaphor over a hole in the logic. If a claim holds only on delivery, that's rhetoric — and it belongs in AI-TELLS.md. Delivery is fine as packaging for a sound argument, never as its replacement.

## 8. Good questions (the Socratic check)

- how do I know this?
- what would have to be true for the claim to hold?
- under what conditions does it break?
- who is this **not** for, and why?
- what do I *want* to be true — and am I bending the conclusion toward it?

## The checklist (on review)

Run it on the key claims, the strongest first:

1. Confidence level set? (fact / experience / hypothesis)
2. Visible basis? Is it relevant, sufficient, reliable?
3. No fallacy from section 4?
4. No bias from section 5?
5. Steelman done, if criticizing someone?
6. Does "where it breaks" name real limits, not a fig-leaf disclaimer?
7. No apparent self-contradiction: if a claim flips ("cheap" → "not free"), is it shown that the *scale* changed (a unit vs a sum, a rare case vs frequency), not the fact itself?

Close a found hole with a basis, soften it to a hypothesis, or cut it. A confident tone over an unverified claim is not allowed.
