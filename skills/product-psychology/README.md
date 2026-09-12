# product-psychology

Applies the [Growth.Design psychology catalog](https://growth.design/psychology)
(106 cognitive biases and UX principles) when designing any product surface.

Diagnose the user moment into one Benson bucket (information, meaning, time,
memory), load that bucket only, pick 2–4 principles, pass an ethics floor, then
stop. It does not dump the catalog.

## When to reach for it

- Building onboarding, paywalls, checkout, empty states, notifications, habit
  loops, pricing tables, settings, or cancellation
- Users drop off, do not convert, or do not return
- Someone says "nudge," "dark pattern," "aha moment," or "product psychology"

## The walk

1. Ethics floor: true, reversible, informed, wanted, second-order
2. Dominant bucket
3. Design / Audit / Teach
4. Name the dark twin you will not do

## Pairing

- Reviewing a live surface → [product-psychology-audit](../product-psychology-audit)
- Marketing pages / campaigns → `marketing-psychology` (not in this repo)

## Install

```bash
ln -s "$PWD/skills/product-psychology" ~/.claude/skills/product-psychology
```

Then invoke `/product-psychology`, or describe the surface and let the agent
pick it up from the description.
