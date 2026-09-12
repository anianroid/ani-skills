---
name: product-psychology-audit
description: >-
  Audits an existing product surface against the Growth.Design / Benson
  psychology catalog (information, meaning, time, memory). Use when the user
  asks to review, critique, or red-team a flow, screen, paywall, onboarding,
  checkout, empty state, notification, or cancellation; or says "psychology
  audit," "dark pattern check," "why do users drop off here," or "what's wrong
  with this UX." For designing a new flow, use product-psychology. For visual
  UI rules, use web-design-guidelines.
metadata:
  version: 1.0.0
---

# Product Psychology Audit

Read [../product-psychology/SKILL.md](../product-psychology/SKILL.md) and run **Audit** mode.

Then load, in order, only what the surface needs:

1. [../product-psychology/traps.md](../product-psychology/traps.md)
2. The dominant bucket file(s) under `../product-psychology/`
3. [../product-psychology/catalog.md](../product-psychology/catalog.md) if you need a name

## Walk order

1. **Information** — can they see the next step, or is it drowned / ad-shaped / tiny?
2. **Meaning** — what story will they invent if a label is missing?
3. **Time** — what will a rushed person click, and is that in their interest?
4. **Memory** — what peak and ending will they take home?

## Finding format

- **Principle**
- **Evidence** (on-screen)
- **Risk** (ethics floor or user cost)
- **Fix** (one change)
- **Severity**: blocker / should-fix / polish

Blockers = deceptive, irreversible, or hidden money/exit.

Do not invent issues to fill all four buckets. If a bucket is clean, say so in one line.
