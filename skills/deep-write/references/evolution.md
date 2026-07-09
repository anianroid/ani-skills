# How deep-write evolves

Every run of deep-write is also a chance to tune deep-write. The skill watches
how the author reacts (explicit feedback, edits, approvals) and how they behave
(what they actually ship, their cadence and topics, which stages they skip),
logs those signals, and graduates the recurring ones into a personal profile
that overrides the defaults. The shareable core stays clean; the personal layer
is where learning accumulates.

## Two layers

- **Shareable core** (`references/`, `templates/`): the defaults. Ships to
  everyone. Edited only deliberately, through an approval gate.
- **Personal profile** (`profile/`, gitignored): the living, per-author layer.
  - `LEARNED.md`: the active, graduated rules the skill applies every run.
  - `signals.md`: the raw journal of observations.
  - `CHANGELOG.md`: the audit trail of what evolved, when, and why.

When deep-write is open-sourced, `profile/` is gitignored, so new users start
with an empty profile and grow their own. The engine (this file) travels; the
data does not. If the `profile/` files do not exist on a run, create them from
the structures below.

## The loop: Apply, Observe, Log, Distill

### 1. Apply (at intake)

Read `profile/LEARNED.md` if it exists and layer it over the `references/`
defaults. On conflict, LEARNED wins: it is the personalized layer. If there is
no profile yet, use the pure defaults.

### 2. Observe (at each gate and after the piece ships)

Watch for signals in two buckets:

- **Reactions (explicit):** feedback at gates ("too hedged", "punchier", "I hate
  that opener"), the edits the author makes to your drafts (what they cut, swap,
  restructure), approvals and rejections, which title or hook they pick.
- **Behavior (implicit):** what they actually post versus what you drafted
  (hashtag changes, cut tweets, reworded hooks), cadence and topics over time,
  which gates or stages they consistently skip or expand, how much research they
  tolerate, tone drift.

### 3. Log (append to `signals.md`)

One entry per signal. Fields: date, piece slug, category (`voice` | `research` |
`distribution` | `process` | `topic`), the observation, a verbatim quote if
there was one, and a status of `candidate`. Log only real, observed signals.
Never invent a signal to fill the journal.

### 4. Distill (end of each run, or on demand via "deep-write evolve")

Review `signals.md` and promote using the same confidence model as the research
playbook:

- **Stated as a rule** by the author ("always do X", "never do Y") → graduate
  immediately (high confidence).
- **Observed across two or more pieces** → graduate.
- **Seen once, not stated** → stays a `candidate`. Leave it logged; do not act.

When graduating a signal:

1. Write or update the rule in `LEARNED.md` (keep it to the active rule set).
2. Add a `CHANGELOG.md` entry: date, the rule, and the signals that justify it,
   so it is reversible.

If a graduated rule is core enough to belong in the shareable defaults
(`voice.md`, `distribution.md`, etc.), **do not silently edit the core.** Propose
the edit at a gate and let the author approve. Approved edits update the
reference file and get a CHANGELOG note.

## Guardrails

- Personal-profile updates are automatic, low-risk, logged, and reversible.
- Shareable-core edits require explicit approval.
- Everything is auditable in the CHANGELOG; any graduation can be reverted.
- Do not overfit: one data point is a candidate, never a rule.
- Keep `LEARNED.md` tight. It is the active rule set, not the journal. When a new
  signal contradicts an old rule, update the rule and note it; do not just append
  a contradiction.

## File formats

`LEARNED.md`, grouped by category, one rule per line with a confidence tag and a
date:

```markdown
## Voice
- [graduated 2026-07-15] Prefer plain verbs over "leverage"/"utilize"; he swaps these out every time.

## Distribution
- [stated 2026-07-15] Never lead an X hook with a rhetorical question; open on the number.
```

`signals.md`, reverse-chronological:

```markdown
### 2026-07-15 · <slug> · voice · candidate
Observation: cut every instance of "it's worth noting" from the draft.
Quote: "stop hedging, just say it"
```

`CHANGELOG.md`, reverse-chronological, one entry per graduation or core edit.
