# product-psychology-audit

Reviews a live product surface against the Growth.Design / Benson catalog.

It does not design a new flow. It walks information → meaning → time → memory
and reports findings as principle, evidence, risk, fix, severity.

Requires [product-psychology](../product-psychology) as a sibling folder.

## When to reach for it

- "Psychology audit," "dark pattern check," "why do users drop off here"
- Red-teaming a paywall, onboarding, checkout, empty state, or cancel flow

## Install

```bash
ln -s "$PWD/skills/product-psychology" ~/.claude/skills/product-psychology
ln -s "$PWD/skills/product-psychology-audit" ~/.claude/skills/product-psychology-audit
```

Then invoke `/product-psychology-audit`.
