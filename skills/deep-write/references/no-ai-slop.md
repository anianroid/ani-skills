# The no-ai-slop check

Source: [petergyang/no-ai-slop](https://github.com/petergyang/no-ai-slop) (MIT). Fetched
`SKILL.md` and `eval.md` directly, not just the README, and condensed into the
patterns that actually recur in this author's drafts. Run this as an explicit
pass at the end of Stage 5 (essay) and Stage 6 (distribution copy), not just a
vibe check. If the external repo changes, re-fetch and re-diff this file rather
than trusting memory of it.

**Author-requested, added 2026-07-26**, after the X thread for "The Bug Was in
the Silence" read as AI-ish. The root cause was not a single bad line, it was
the same "label: dramatic reveal" shape recurring four or five times across one
distribution pack. One instance is a stylistic choice. Three or more is a tell.
Count occurrences of a pattern across the whole draft, not just per-sentence.

## The single highest-value check: colon reveals and plot-twist labels

Watch for a noun phrase, a colon or a bare label, then a punchy reveal:
"The weird part: the strikes came from rotations that succeeded." "The fix: three
flag changes. The real work: redesigning the counter." "Final twist: one
'wedged agent' wasn't wedged at all."

Fix: state the fact directly. "The strikes came from rotations that succeeded."
"Three flag changes fixed it. The real work was redesigning the counter." "One
'wedged agent' wasn't wedged at all."

This is NOT banning colons outright. A colon before a genuine list, a label
("BACKOFF: three strikes and the watchdog stops trying"), or a quote
("the log said: 'manual intervention needed'") is fine and matches this
skill's own declarative-header convention in `voice.md`. The tell is a colon
used as a drumroll before a single dramatic payoff, not a colon used to define
or introduce.

Also cut the explicit "Plot twist:" / "final twist:" / "here's the killer"
family, plain rhetorical drumrolls with no informational content of their own.
State the twist as a fact instead of announcing that a twist is coming.

## Other patterns worth a specific look in this author's drafts

- **Throat-clearing openers.** "Here's the thing," "Here's what nobody tells
  you," "The uncomfortable truth is." Cut and state the point. Note: this
  author's established hooks already avoid these (see `profile/signals.md`,
  2026-07-09 entry on rejecting "here's the part nobody selling you a model
  will tell you"). Treat a fresh instance as a regression, not a new finding.
- **Self-answered rhetorical Q&A as a flattery device** ("Want to know the
  secret? Here it is.") is banned. This is distinct from the rhetorical
  question as pivot that `voice.md` explicitly allows ("So what is left?
  Judgment. Taste."). The house move poses a real question and answers it
  across a section, doing argumentative work. The banned version poses a fake
  question purely to manufacture a curiosity gap before a reveal that could
  have been stated directly. When in doubt, cut the question and state the
  answer as the sentence; if nothing is lost, it was the banned kind.
- **Fake-profound kickers.** Do not rewrite a weak closing line into a better
  metaphor. Delete it and end on the clearest concrete sentence already in the
  draft, or the aphoristic close this skill already asks for in
  `voice.md`.
- **Banned words**: delve, foster, leverage, utilize, facilitate, empower,
  streamline, robust, cutting-edge, paradigm shift, game changer, tapestry,
  realm, beacon, multifaceted, meticulous, intricate, paramount, transformative,
  elevate, embark, supercharge, harness (as a verb), ever-evolving.
- **Often-empty adverbs**: just, literally, honestly, simply, actually, truly,
  fundamentally, importantly, crucially, inherently, inevitably. Cut when they
  add nothing; keep when they carry real emphasis, contrast, or uncertainty.
- **Robotic rhythm.** Repeated sentence shapes across a thread or a set of
  paragraphs (the same "X. Y: Z." structure every beat) reads as generated even
  when no single sentence is individually bad. Vary the shape.
- **Formatting slop.** Emoji in headings, bold sprinkled mid-sentence, bullets
  where two sentences of prose would read better. The 🧵 marker on an X
  thread's first tweet is a genuine platform convention, not slop; a
  numbered-triad tagline the author has reused across multiple published
  pieces (e.g. "rotate, remember, recover") is an established voice signature,
  not slop either. Don't strip house conventions while hunting for AI tells.

## Sentence-structure tells (Kristen Lowe, "Sentences That Sound Like Other Sentences")

Source: [Sentences That Sound Like Other Sentences: Seven Sentence-Level AI
Writing Tells](https://workbravely.substack.com/), pt. 4 of her AI-writing-tells
series. **Author-requested, added 2026-08-18.** These are shape tells, not
vocabulary tells: a sentence can clear every banned-word and colon-reveal check
above and still read as AI because of its structure. Same threshold as
everywhere else in this file: one instance is a stylistic choice, two or more
of the same shape in one draft is a tell.

- **Negative parallelism & correlative conjunctions.** "It's not just X, it's
  Y." "Not only did X, but it also Y." "Neither X nor Y." Legitimate when it
  corrects an assumption the reader actually holds. AI uses it to manufacture
  drama around a premise no one held ("WWII wasn't just a military conflict,
  it was a global event" — nobody thought otherwise). Test: if you can't name
  the specific wrong assumption the sentence is correcting, the negative half
  is doing nothing. Cut it and state the fact plainly.
- **Tricolons with a weak third item.** Three-part lists are a real rhetorical
  tool (this skill uses them deliberately, see `voice.md`), but AI defaults to
  three even when two would do, padding the last slot for rhythm: "the
  experience was fun, relaxing, and rejuvenating" (rejuvenating adds nothing
  relaxing didn't already cover). Test: does the third item survive being cut?
  If the sentence loses no information, the third item was decorative.
- **Dramatic countdowns.** Negative parallelism and a tricolon stacked to fake
  stakes: "It's not the tooling. It's not the staffing. It's the handoff."
  Reads like a game-show elimination when nobody proposed tooling or staffing
  as the cause. Fix: just name the cause. Reserve the countdown shape for when
  the ruled-out options were genuinely on the table.
- **Fragment question, immediate answer.** "The beta results? Transformative."
  A one-to-three-word question with the verb dropped, followed by a punchy
  one-word verdict. Distinct from the self-answered-rhetorical-Q&A pattern
  above (that one poses a full question as a curiosity-gap device); this one
  is a sentence fragment doing a staccato reveal. Near-zero legitimate use in
  this author's register. Cut on sight, state the result as a plain sentence.
- **False ranges.** "From the farmhouse to the boardroom." "From teenagers to
  managing directors." A real range ("from California to the New York
  Island") has an interior you could enumerate. A false range picks two
  endpoints that sound far apart but describe no actual intermediate scope.
  Test: swap one endpoint for an unrelated word (farmers instead of
  teenagers); if the sentence still basically works, the range was decorative.
  Fix: say what's actually broad, plainly, without the endpoints.
- **Participle tails.** A trailing "-ing" clause explaining what the sentence
  you just read was supposed to accomplish: "...underscoring the
  inefficiency," "...reflecting a broader shift," "...highlighting the
  importance of X." If the sentence needs the tail to land, the sentence
  itself wasn't clear enough. Fix the sentence and cut the tail; don't keep
  both.
- **Uniform sentence length and shape.** Sharpens the "robotic rhythm" bullet
  below into a concrete test: read a paragraph and eyeball word counts. AI
  sentences cluster in a narrow band (roughly 15 to 18 words) and repeatedly
  trail off into the same qualifying-clause shape ("..., a signal that X").
  Human paragraphs alternate short punches with long, clause-heavy sentences.
  If every sentence in a paragraph could swap places without changing the
  rhythm, vary it.

## X-specific note: threads can manufacture this pattern

Chopping a continuous story into numbered tweets creates artificial beat
boundaries, and this author's own drafts show a tendency to fill each boundary
with a "label: reveal" tee-up to make the next tweet feel earned. If the author
has X Premium (check `profile/platforms.md` or ask once), default to offering a
single long-form post as an alternative to a numbered thread for narrative
(story-shaped) pieces, and re-run the no-ai-slop check on the merged version,
not just the original thread. See `references/distribution.md`.

## Workflow

1. Read the full draft (essay, then each distribution artifact) before editing.
2. Count instances of each pattern above across the whole draft. Two or more of
   the same "label: reveal" shape is the strongest signal, fix all of them, not
   just the most obvious one.
3. Make the minimum effective edit. Preserve the author's established voice
   signatures (lowercase social copy, dry understatement, specific technical
   nouns repeated on purpose, the aphoristic close). Do not smooth every
   sentence into the same tidy shape.
4. Report a short **What changed** note: which patterns were found, quoted,
   and how they were fixed, plus anything deliberately left alone and why.
