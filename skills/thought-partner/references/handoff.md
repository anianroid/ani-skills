# Hand over the brief

The walk's only done-condition. One artifact the user keeps. A build
plan may ride along. It never replaces the brief.

Write it in the conversation. If they want a file, offer a path
(default: `thought-partner-brief.md` in the repo root, or
`~/.gstack/projects/<slug>/` if that directory already exists). Do
not create a project just to store this.

## Brief template

```markdown
# Pre-build brief: {title}

Date: {date}
Mode: Idea | Feature | Builder
Status: DRAFT until they approve
Verdict: do not build | spike first | build this wedge

## Settled ground (known knowns)
- {fact or decision, with citation or "user-stated"}
- Assumptions treated as settled unless overturned:
  - {assumption}

## Decision ledger (known unknowns)
| Question | Answer | Closed by | Why |
|---|---|---|---|
| {question} | {one-line decision} | user / territory / OPEN | {why} |

OPEN items say what unblocks them.

## Extracted (unknown knowns)
- Taste / motivation / tacit constraints that were not in the original
  ask, and what each reshaped.

## Blind spots (unknown unknowns)
Ranked, worst first.

1. **{title}** — evidence: {cite}. Bites because {why}. Changes: {go/no-go/wedge}. Status: decided | OPEN | sharp-edge.

## Premises
1. {statement} — agreed / disagreed / revised to {new}

## Approaches
### A — {narrowest wedge}
Effort / risk / what it learns

### B — {ideal architecture}
Effort / risk / why not first

### C — {lateral, if any}

**Chosen:** {A/B/C} because {one line mapped to their stated goal}.

## Remaining unknowns → cheapest reduction
| Unknown | Resolves by | Cheapest artifact |
|---|---|---|
| {unknown} | research / user / shipping | spike (timebox) / prototype to react to / reference to point at / research pass with a falsifiable claim |

## What we will not build
- {explicit non-goals}

## The assignment
One concrete real-world action. Not "go build it."

Examples that count:
- Talk to {named person} about {named workflow} this week
- Watch {named user} do {task} without helping
- Timebox a {N-hour} spike on {kill assumption}
- Charge {amount} for {wedge} before writing the platform

## Recommendation
What the user should do next, in one short paragraph. This skill
exists to change the next move, not to produce a taxonomy.
```

## What rides along

- A **tweakable plan** is allowed: judgment calls first, with
  alternatives, mechanical work collapsed at the bottom ("I trust you
  on that part").
- A **copyable next message** the user can paste to start the build
  as a separate task, grounded in the chosen wedge and the OPEN items.

## Approval

Ask them to approve, revise, or restart.

- Approve → mark Status: APPROVED. Offer to start the build as a
  new task. Do not start it here.
- Revise → change only the named sections, then re-present.
- Restart → return to mode + settled ground.

If they approve with OPEN kill-assumptions, the verdict cannot be
"build this wedge." It is "spike first" until those close.
