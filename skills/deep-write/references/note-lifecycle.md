# The one-note lifecycle

deep-write writes each piece as a single note that carries its whole lifecycle:
the polished essay on top, and the making-of below a divider. The finished piece
and its research travel together, so the note is both the deliverable and the
record of how it was made.

## Output location (configurable)

- **Default:** `./deep-write-drafts/<slug>.md` relative to the working directory.
- **Obsidian integration:** point it at a vault `Writing/` folder to slot into an
  existing second-brain. If the user works this way, write there instead.
- No paths are hardcoded in the skill. Ask once during intake, or default to
  `./deep-write-drafts/` and mention it.

## Note structure

```markdown
---
type: essay
status: draft
tags: [thoughts, writing, <topic tags>]
---

<!-- polished essay: this mirrors what will publish; keep it wikilink-free so
     it stays easy to sync to a blog repo -->

## <declarative section header>
...the finished essay...

> [!note] One note, whole lifecycle
> Destination: <blog / newsletter / where it will live>
> Status: draft. The workshop below records the making-of.

# 📝 Workshop (below this line)

## Thesis / angle
<one-line thesis, and the prior piece it rhymes with>

## Grounding ledger
<claim → source → job, with confidence flags. See research-playbook.md>

## Outline
<numbered section skeleton>

## Rough draft
<the looser conversational version, kept for reference>

## Raw thoughts / brain dump
<the original dump, verbatim>

## Distribution
<X thread, quote-tweet copy, LinkedIn post, first comment, carousel manifest,
 tagging plan, launch-day sequence>

## Decision log / still open
<title lock + rationale, disclosure comfort, thin claims softened, TODOs>
```

## Naming and status

The filename carries the stage. Start as `<title> (draft)` with `status: draft`.
Do not split a piece into sibling notes. When the human later publishes, they
rename to `<title> (published)`, set `status: published`, and (if it has a blog
post) treat the repo file as canonical while the note's top section stays a
wikilink-free mirror.

## Why wikilink-free on top

The polished section is meant to be copy-pasted into a blog or newsletter with
no edits. Keeping it free of vault-only syntax (wikilinks, embeds) means it syncs
cleanly to wherever it publishes.
