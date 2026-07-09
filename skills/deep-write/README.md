# deep-write

A Claude Code / Agent skill that turns a raw thought dump into a publish-ready
essay plus its social distribution (an X thread and a LinkedIn post), with deep
research at every stage.

It is fully agentic: it researches, drafts, and writes the distribution copy,
pausing at three review gates. It stops at ready-to-ship drafts. It does not
publish a blog, run git, or post to any platform. A human ships.

## What it produces

For one input (a brain dump, a voice-memo transcript, a link, or a one-liner):

- A publish-ready essay with SEO frontmatter.
- An X thread, plus quote-tweet copy for launch day.
- A native LinkedIn post, plus its first-comment link and an optional carousel
  manifest.

All of it lands in a single "one note, whole lifecycle" file: the polished piece
on top, the research ledger, outline, rough draft, and distribution plan below.

## The pipeline

1. **Intake:** gather the raw material, ask at most three clarifying questions.
2. **Angle:** sharpen to a one-line thesis and title options. `Gate 1`
3. **Deep research:** build a grounding ledger with confidence flags and a
   prior-art sweep. `Gate 2`
4. **Outline:** a numbered skeleton with declarative headers.
5. **Draft:** the full essay in the house voice.
6. **Polish:** publish-ready, sourced, no em-dashes. `Gate 3`
7. **Distribution:** X thread + LinkedIn post + launch plan.

## Install

Copy this folder to your skills directory:

```
~/.claude/skills/deep-write/
```

Then invoke it in Claude Code with `/deep-write`, or just describe the task
("turn this dump into an essay and social posts") and it will trigger.

## Layout

```
deep-write/
  SKILL.md                      the orchestrator: pipeline + gates + quality bar
  references/
    research-playbook.md        the grounding ledger, confidence flags, prior-art sweep
    voice.md                    voice rules + few-shot examples (retune per author)
    distribution.md             X + LinkedIn conventions, verbatim examples, tagging plan
    note-lifecycle.md           the one-note output structure (configurable location)
    evolution.md                the self-evolution engine (Apply, Observe, Log, Distill)
  templates/
    essay.md
    x-thread.md
    linkedin-post.md
  profile/                      the personal learning layer (data files gitignored)
    README.md                   what the layer is (tracked, ships)
    LEARNED.md, signals.md, CHANGELOG.md   per-author, gitignored
```

## Self-evolution

deep-write sharpens as you use it. Two layers keep this clean:

- **Shareable core** (`references/`, `templates/`) is generic and ships to
  everyone.
- **Personal profile** (`profile/`, gitignored) is where learning accumulates
  for one author.

On every run it **applies** your learned profile, **observes** how you react
(edits, feedback, which hook you pick) and behave (what you actually post,
cadence, topics, stages you skip), **logs** real signals, and **distills** the
recurring ones into rules. A signal stated as a rule or seen across two pieces
graduates into your profile automatically and reversibly (audited in a
CHANGELOG); anything that belongs in the shareable core is proposed for your
approval first, so the shared artifact never drifts silently. When open-sourced,
the engine travels but your data stays private and each new user grows their own
profile from empty.

## Customizing the voice

The default voice is distilled into general principles (concede-then-complicate,
cite everything, no em-dashes, aphoristic close) plus few-shot examples. To
retune for a different author, swap the examples in `references/voice.md` for
that author's own published pieces.

## License

TODO before open-sourcing.
