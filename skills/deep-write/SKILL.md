---
name: deep-write
description: >-
  Turn a raw thought dump into a publish-ready essay plus an X thread and a
  LinkedIn post, with deep research at every stage. Use when someone has a brain
  dump, voice-memo transcript, rough idea, or link and wants a finished essay
  and its social distribution. Trigger phrases: "deep-write this", "turn this
  into an essay", "essay + X post + LinkedIn post", "write and distribute",
  "make a blog post from these notes", "thought dump to essay". Fully agentic:
  it researches, drafts, and writes the distribution copy, pausing at three
  review gates. It stops at ready-to-ship drafts; it does not publish or post.
---

# deep-write

A staged pipeline that takes a rough thought and returns three artifacts: a
publish-ready essay, an X thread, and a LinkedIn post. Research is a first-class
step at every stage, not an afterthought. Everything lands in a single "one
note, whole lifecycle" file so the making-of travels with the finished piece.

## Operating principles

1. **Research before you write, at every stage.** Never assert a number or a
   claim you have not grounded. Fan out real web research with subagents. See
   `references/research-playbook.md`.
2. **One connected body of work.** Each piece should rhyme with the author's
   prior essays around a house through-line, not read as a standalone hot take.
3. **Concede, then complicate.** Grant the popular claim first, then turn it.
4. **Cite everything, flag what is thin.** Every claim gets a source; single
   sourced or contested claims get softened language and a flag.
5. **Land the plane on one line.** Close on a single aphoristic sentence.
6. **No em-dashes.** Use commas or colons instead, in the copy and in these
   drafts. This is a hard rule. See `references/voice.md`.
6b. **Run the no-ai-slop check before every gate.** Colon-reveals ("the weird
   part: X"), plot-twist labels ("final twist:"), throat-clearing openers,
   fake-profound kickers, and banned filler words are cut on sight, in the
   essay and in every distribution artifact. Two or more of the same tee-up
   shape across one piece is the strongest tell; fix all instances, not just
   the obvious one. See `references/no-ai-slop.md`.
7. **You draft, the human ships.** Produce ready-to-post drafts. Do not push
   git, publish a blog, or post to social.
7b. **Do the work, never pass the buck.** Do not hand the author a task you could
   do yourself. If the copy needs a quote-tweet target, a link, a stat, a handle,
   or an asset, go find the real one, verify it (curl the URL, confirm the post is
   real and recent), and put it in with the link and drafted copy. "Find a tweet to
   QT" is not a deliverable; a specific, verified, linked post with the QT copy
   already written is. Leave a TODO for the author only when it genuinely requires
   access or judgment you do not have (a private link not in the vault, a
   subjective brand call), and when you do, say exactly why it is blocked and what
   you already tried. Ship the most finished thing you can, not homework.
8. **The skill tunes itself to you.** Every run, apply what you have learned
   about this author and log how they react and behave, so the skill sharpens
   over time. See `references/evolution.md` and the Self-evolution section below.

## What this does and does not do

- **Does:** intake, thesis, deep research, outline, draft, polish, and
  distribution copy (X thread + LinkedIn post + optional carousel manifest),
  written into a one-note lifecycle.
- **Does not:** publish to a blog, run git, or post to any platform. It ends at
  drafts a human can copy, paste, and ship.

## Intake (do this first)

First, **apply the personal profile:** read `profile/LEARNED.md` if it exists and
layer its rules over the defaults for the rest of the run. On conflict, the
profile wins. If there is no profile yet, use the pure defaults. See the
Self-evolution section.

Gather the raw material: a pasted dump, a file path, a link, or a one-liner.
Then ask only what is genuinely missing, at most three questions:

- The core claim or angle, if it is not already clear from the dump.
- The audience and where it will live (personal blog, company blog, newsletter).
- Any prior piece it should rhyme with (the house through-line).
- Output location. Default is `./deep-write-drafts/<slug>.md`. It can point at an
  Obsidian `Writing/` folder instead. See `references/note-lifecycle.md`.

If the dump is already rich, infer the rest and proceed. Do not stall on
questions you can answer yourself.

## The pipeline

Run the stages in order. Pause only at the three gates marked 🚦. Between gates,
keep momentum. Delegate research to subagents so the heavy reading stays out of
the main thread.

### Stage 1: Angle (thesis and title)

- Distill the dump to a one-line thesis. Sharpen it until it is contrarian but
  fair, and specific rather than vague.
- Do a quick prior-art scan: has this been argued before, by whom, and what is
  the strongest counterargument? This sharpens the angle and surfaces who to
  cite or rebut later.
- Identify 2 to 3 candidate "hook numbers": the single strongest stat the piece
  could lead with. Note which you still need to verify.
- Draft 2 to 3 title options as declarative mini-arguments, plus a slug.

🚦 **Gate 1:** Present the thesis, the title options, and the candidate hook
numbers. Get a nod (or a redirect) before spending on deep research.

### Stage 2: Deep research and the grounding ledger

- Fan out web research (parallel subagents; use the `deep-research` skill if it
  is installed). Build a **grounding ledger**: one bullet per claim, mapping
  claim to primary source to the rhetorical job it does, with a confidence flag.
- Prefer primary sources. Record when you are leaning on a secondary summary.
- Run the "am I reinventing a wheel?" sweep: the competitive or prior-art
  landscape. Name the neighbors and what each misses.
- First-party evidence counts: the author's own logs, incidents, and numbers are
  strong material. Pull exact figures.
- Full method in `references/research-playbook.md`.

🚦 **Gate 2:** Present the ledger. The human flags what to cut, soften, reserve,
or dig deeper on. This is where thin claims get caught before they reach prose.

### Stage 3: Outline

- Write a numbered section skeleton. Every header is a declarative mini-argument,
  not a label ("Making got cheap, and the data backs it up", not "Background").
- Open with the concede-then-complicate move. Plan the aphoristic close.
- Add a comparison table if the piece hinges on a build-vs-buy or A-vs-B choice.

### Stage 4: Draft

- Write the full essay in the house voice: first person, personal stakes,
  varied rhythm with punchy fragments for emphasis, named authorities as
  shorthand, every claim hyperlinked inline. See `references/voice.md`.
- Keep the through-line explicit so it rhymes with the prior piece.

### Stage 5: Polish to publish-ready

- Tighten to the published register. Run the self-check below.
- Run the no-ai-slop check (`references/no-ai-slop.md`) on the full essay.
- Verify there are zero em-dashes. Verify every claim carries a source and every
  single-sourced claim is softened and flagged.
- **Verify every link resolves.** Curl each URL and flag any 404 (a real break,
  fix it). Treat 403 as a likely bot-block that still works in a browser (e.g.
  Bloomberg, Bain), not a break. Never ship a draft with a dead link.
  Research-sourced URLs are the usual culprits, and a dead host can 404 or
  redirect, so check them, do not trust them.
- Sharpen the section headers and the closing line.
- Produce SEO frontmatter: `title`, `date`, `description`, `tags`.

🚦 **Gate 3:** Present the finished essay before spinning up distribution.

### Stage 6: Distribution

**Platform packs.** Distribution is modular. X and LinkedIn are the core pack,
always produced. Extra platforms (Reddit field notes, and future packs) are
opt-in per author, recorded in `profile/platforms.md`. Read that file first and
draft only the enabled platforms. If it does not exist, this is a new author:
ask once which extra platforms to enable (a one-question onboarding), write
their answer to `profile/platforms.md`, and proceed. The author can change the
lineup any time by saying "deep-write platforms" (add/remove platforms
conversationally; update the file). Each extra platform has its own reference
playbook (e.g. `references/reddit-field-notes.md`) and its own voice: never
port the X/LinkedIn copy to another platform unedited.

Produce the core pack, following `references/distribution.md`:

- **X thread (or single long-form post for X Premium authors):** default is a
  link-free hook tweet leading with the contrarian number, one idea per
  numbered tweet mirroring the essay sections, genuine @-attribution inline,
  disclosure inline if relevant, link only in the final tweet. If the author
  has X Premium (check `profile/platforms.md`, ask once if unknown, and cache
  the answer there), offer a single flowing long-form post as the alternative
  for narrative/story-shaped pieces: numbered tweet-boundaries tend to
  manufacture colon-reveal tee-ups (see `references/no-ai-slop.md`), and a
  continuous story often reads less AI-ish than the same beats chopped into a
  thread. Either way, include 1 to 2 quote-tweet posts for launch day (QT the
  exact post you are rebutting).
- **Run the no-ai-slop check** (`references/no-ai-slop.md`) on every
  distribution artifact before presenting it, not just the essay. Count
  repeated tee-up shapes across the whole pack, not per-sentence.
- **LinkedIn post:** native long-form, complete without a click, hook in the
  first two lines before the fold, short paragraphs with whitespace, close on a
  question, 5 trailing hashtags, and the link in a first comment you post
  yourself.
- **Carousel: ask, don't assume.** Ask the author whether to generate the
  LinkedIn carousel as an actual PDF (8 to 10 slides, 4:5 portrait, editorial
  style matching the blog aesthetic) for higher LinkedIn reach. If yes, build
  and render it (custom HTML printed via headless Chrome gives exact 4:5
  sizing, which letter/A4 markdown-to-PDF tools cannot); if no, offer the
  slide manifest only.
- **Launch plan:** the tagging plan (attribution vs quote-tweets, kept
  separate) and the launch-day sequence.

If enabled in `profile/platforms.md`, also produce:

- **Reddit field notes:** a standalone text post per target community,
  following `references/reddit-field-notes.md`. This is NOT distribution copy:
  no links in the body, no mention of the essay unless asked in comments, no
  marketing voice. It is the author sharing what they learned, rewritten from
  scratch in community register. Skip entirely (and say so) when the piece has
  no genuine lesson to share or no community where it fits; a skipped Reddit
  post is always better than a salesy one.

## Output

Write one note per piece to the output location, in the "polished on top,
Workshop below" structure. Full spec in `references/note-lifecycle.md`. Order:

1. Frontmatter (`type`, `status: draft`, `tags`).
2. The polished essay.
3. A callout noting intended destination and status.
4. `# 📝 Workshop (below this line)`.
5. Thesis and angle, grounding ledger, outline, rough draft, distribution block,
   and a decision log of open calls (title lock, disclosure comfort, thin
   claims softened).

Filename carries the stage: start as `<title> (draft)` with `status: draft`.

## Self-evolution (learn from every run)

deep-write improves as this author uses it. Full engine in
`references/evolution.md`. The loop, each run:

- **Apply** the personal profile at intake (above).
- **Observe** at each gate and after the piece ships: how the author reacts
  (feedback, the edits they make to your drafts, what title or hook they pick)
  and how they behave (what they actually post vs what you drafted, cadence,
  topics, which stages they skip or expand).
- **Log** each real signal to `profile/signals.md` as a `candidate`. Never invent
  a signal.
- **Distill** at the end (or on "deep-write evolve"): promote signals that were
  stated as a rule, or seen across two or more pieces, into `profile/LEARNED.md`,
  with a `profile/CHANGELOG.md` entry. If a rule belongs in the shareable core
  (`references/`), propose that edit at a gate rather than editing it silently.

Personal-profile updates are automatic and reversible. Shareable-core edits need
the author's approval. If the `profile/` files do not exist, create them first.

## Self-check before every gate

- [ ] No em-dashes anywhere.
- [ ] Every claim has a source; single-sourced claims softened and flagged.
- [ ] Every link resolves (404 = fix it; 403 = bot-block, valid in a browser).
- [ ] Opening concedes then complicates.
- [ ] Close is one aphoristic line.
- [ ] Section headers are arguments, not labels.
- [ ] Specific numbers over vague ones.
- [ ] X hook tweet is link-free; LinkedIn link is in the first comment.
- [ ] Both social posts end on a question.
- [ ] Attribution @s are genuine; the critique target is never cold-tagged.
- [ ] Every quote-tweet target, link, stat, and asset is a real, verified, linked
      thing (curl-checked), not a "go find one" instruction handed to the author.
      Any remaining TODO says exactly why it is blocked and what you already tried.
- [ ] Essay and every distribution artifact pass the no-ai-slop check
      (`references/no-ai-slop.md`): no colon-reveals, plot-twist labels,
      throat-clearing openers, fake-profound kickers, banned filler words, or
      off-shape sentence structures (negative parallelism, dramatic
      countdowns, weak-third tricolons, fragment-question-answers, false
      ranges, participle tails). A repeated tee-up shape across the pack is
      fixed everywhere it appears.

## Optional accelerators

deep-write is self-contained and needs none of these. If they are installed you
may delegate sub-steps: `deep-research` (Stage 2), `social-content` (Stage 6),
`copy-editing` (Stage 5), `seo-audit` or `ai-seo` (frontmatter and titles).
