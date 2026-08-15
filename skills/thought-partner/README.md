# thought-partner

A pre-build thought partner. It maps unknowns, hunts blind spots, and
asks the hard questions before you (or any builder) start building.

It does not write code. It does not scaffold a repo. It ends with a
brief: a verdict (do not build / spike first / build this wedge), a
four-quadrant map, ranked landmines, forced alternatives, and one
concrete assignment that is not "go build it."

## When to reach for it

- A new product idea, before the first file exists
- A big feature in something that already ships
- "Is this worth building?"
- "What am I missing?"
- You want someone in the room who will not flatter the pitch

## What it inherits

- **[find-unknowns](../find-unknowns)** — quadrant map, blind-spot
  pass, decision-changing interview, cheapest-artifact reduction.
  Originally from ["A Field Guide to Fable: Finding Your
  Unknowns"](https://x.com/trq212) by [@trq212](https://x.com/trq212).
- **[gstack](https://github.com/garrytan/gstack)** by Garry Tan —
  `/office-hours` forcing questions (demand, status quo, specificity,
  wedge, observation, future-fit), anti-sycophancy, premise challenge,
  mandatory alternatives, Search Before Building. This skill does not
  require gstack to be installed.

## The walk

0. Mode: idea, feature, or side project
1. Settled ground (known knowns)
2. Blind-spot pass (unknown unknowns)
3. Hard questions, one at a time, push twice
4. Premises + 2–3 alternatives (narrowest wedge vs ideal)
5. The brief

## Install

Symlink (recommended):

```bash
ln -s "$PWD/skills/thought-partner" ~/.claude/skills/thought-partner
```

Cursor / Codex / other hosts: point the same folder at that host's
skills directory, or copy it.

Then invoke `/thought-partner`, or describe the idea and let the
agent pick it up from the description.

## Pairing

Run this *before* a spec or an implementation skill. If the build
later discovers deviations, run [find-unknowns](../find-unknowns)
again and fold them back into the map. If you have gstack installed,
the approved brief can feed `/plan-eng-review` or `/plan-ceo-review`.
