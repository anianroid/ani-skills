# Research playbook

Research is a visible, first-class artifact in every piece, not something hidden
behind the prose. The output of the research stages is a **grounding ledger**
that ships inside the Workshop section of the note.

## The grounding ledger

One bullet per claim. Each bullet maps three things:

`claim  →  primary source (linked)  →  the rhetorical job it does`

...plus a confidence flag. Example, verbatim from a real piece:

> **Context rot** (Chroma 2025): 18 frontier models, all degrade as input grows,
> often far below the cap. [link] → why bloat must be rotated. Confidence: high,
> primary study.

Name the ledger to match the piece. Real pieces used: "Research & sources",
"External grounding used", "Key facts / stats (with confidence flags)" plus a
"Sources" list.

## Confidence flags

Record how solid each claim is, and let the flag dictate the hedging in the
prose:

- **high, primary:** a primary study or first-party data. Use plainly.
- **solid, secondary:** an authoritative summary of a primary source. Fine to
  use; consider finding the primary.
- **single-sourced:** only one source found. Soften the language in prose ("a
  security write-up catalogues...") and leave a TODO to find a second source.
- **contested:** real but disputed, or narrow methodology. Usually do not use
  in the body. Keep it in reserve and note why.

Real example of the discipline: the "95% of gen-AI pilots fail" stat was flagged
"real but CONTESTED (narrow success definition). Did not use; keep in reserve."
Gartner's "40%+ cancelled by 2027" was chosen instead as "solid, primary."

## Choosing the hook number

From the ledger, pick the single strongest stat as the hook the piece and the
social posts lead with. Criteria: high confidence, surprising, and directly
serves the thesis. Reserve weaker or contested stats for the body or not at all.

## Primary over secondary

Prefer primary sources and make the distinction explicit. When a piece cites a
survey, cite the survey and its press release. When leaning on a summary rather
than the original, say so in the ledger.

## First-party evidence is research too

The author's own logs, incidents, and system numbers are strong material. Pull
exact figures: a real stall incident with "929 seconds" and "reaped 1,
escalated 0", a memory graph growing "~1076 to 1109 pages over the week". These
war stories are often the most credible evidence in the piece.

## The competitive / prior-art sweep

Every analytical piece gets an "am I reinventing a wheel?" pass. This is the
core of "deep research" here:

- Who else has argued this or built this?
- Name each neighbor and the one slice it covers.
- Name what they all miss (usually the hard part your piece is about).
- Verify specifics before you assert them. If you will screenshot a GitHub issue
  or quote a competitor, confirm the exact wording and status first. In one real
  piece, only 4 of the cited issues were confirmed closed-as-described; the rest
  were explicitly marked "confirm before screenshotting."

## How research feeds the writing

- The strongest stat becomes the hook number.
- Confidence flags become hedging language in prose.
- The prior-art sweep becomes a dedicated "am I reinventing a wheel?" section.
- First-party incidents become the section that proves the thesis with a story.
- Questions you researched map one-to-one onto essay sections.

## How to run it agentically

- Fan out several web searches in parallel, each on a different sub-question, so
  no single search angle is a bottleneck. Use subagents to keep the reading out
  of the main thread; return structured bullets, not raw pages.
- If the `deep-research` skill is installed, delegate the heavy grounding pass to
  it and fold its cited findings into the ledger.
- Deduplicate and assign confidence before writing anything into prose.
