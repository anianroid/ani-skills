# Voice and style

This is the default house voice deep-write writes in. It is distilled from a
real body of published essays. The rules generalize well, but the voice is meant
to be retuned per author: swap the few-shot examples below for the author's own
published pieces to recalibrate.

## Hard rules

- **No em-dashes. Ever.** Use a comma or a colon where an em-dash would go. This
  is the single most distinctive mechanical tell. Example of the substitution:
  "it hits a limit, token bloat, context overflow, a compaction loop, and the
  session dies." Never introduce `—`.
- **Every claim is hyperlinked to a source, inline.** Specific numbers over
  vague ones (84%, 29%, 2.3M, 40%, $4.6T, 929 seconds).
- **First person, personal stakes.** The author is in the essay, including
  self-deprecation. "I built a calendar scheduling app." "I hit all of this
  running a fleet." "The part I didn't expect."

## Structural moves

- **Concede, then complicate.** Grant the popular claim first, then pivot. "The
  math is real. It's just pointing at the wrong number." "I think the claim is
  true. I also think it misses the point."
- **Declarative section headers.** Each header is a mini-argument, not a label.
  Good: "Making got cheap, and the data backs it up", "Memory is the whole
  game", "What survives contact with production is boring". Bad: "Background",
  "Analysis", "Conclusion".
- **Rhetorical questions as pivots.** "So what is left? Judgment. Taste." "Am I
  reinventing a wheel?"
- **Named authorities as shorthand.** Karpathy, Paul Graham, Ira Glass, Garry
  Tan, Gartner. Borrow credibility economically, one clause each.
- **Aphoristic one-line close**, usually an antithesis or chiasmus.
- **A house through-line across pieces.** Each essay explicitly rhymes with the
  last, building a connected argument rather than standalone posts. The running
  theme in the reference body: execution and tools commoditize, judgment and
  skills and relationships do not.

## Rhythm

Varied sentence length. A longer setup sentence, then a punchy short fragment
for emphasis. "Volume and visibility are not the same thing." "The retainer is
the tell." "Boring is the moat."

## Tone

Analytical but warm. Contrarian but fair. Critique targets are treated with
respect ("Genuinely useful breakdown, and the math works"). Disclosures are
explicit and disarming ("discount the brand name as much as you like").

## Few-shot: openers (concede then complicate)

- "There's a pitch all over my feed right now: build flashy AI agents for small
  businesses, charge a $2,500/mo retainer, stack 8 clients, hit $20k/mo. The
  math works. It's just pointing at the wrong number."
- "Building one that works in a demo is easy now. Keeping a fleet alive for
  months is a completely different discipline, and almost nobody posts about it."

## Few-shot: closers (aphoristic antithesis)

- "Output is free now. Outcomes never were."
- "Agents are easy to start and hard to keep, and the keeping is the moat."
- "The exciting agent gets the screenshot. The boring one gets renewed."
- "Build for the demo, you get churn. Build for Tuesday, you get a business."

## Few-shot: declarative headers from real pieces

- "Making got cheap, and the data backs it up"
- "The one input that doesn't commoditize"
- "We ship faster than our taste can veto"
- "Memory is the whole game"
- "The part I didn't expect: trusting nothing"
- "The alpha was never the harness"

## Formatting conventions

- Blog frontmatter: `title`, `date` (YYYY-MM-DD), `description`, `tags` (array).
  The page renders the frontmatter title as the H1, so do not repeat the title
  in the body.
- Body uses `##` for section heads. Occasional `*italics*` for coined terms and
  quoted phrases. A `---` references line at the bottom when the piece leans on
  many sources.
