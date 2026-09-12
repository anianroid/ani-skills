---
name: product-psychology
description: >-
  Applies the Growth.Design / Buster Benson product-psychology catalog (106
  biases and UX principles across information, meaning, time, and memory) when
  designing or reviewing any product surface. Use when building or auditing
  onboarding, paywalls, checkout, empty states, notifications, habit loops,
  pricing tables, settings, or cancellation; when the user mentions cognitive
  bias, nudge, dark pattern, Hick's law, peak-end, social proof, aha moment,
  or product psychology; or when users drop off, do not convert, or do not
  return. For marketing-page copy and campaigns, prefer marketing-psychology.
  For signup CRO, onboarding CRO, or page CRO, use those skills and layer this
  on top.
metadata:
  version: 1.0.0
  source: https://growth.design/psychology
---

# Product Psychology

Use this on **every product**, not one repo. Diagnose the user moment, pick a
few principles, apply them ethically, then stop. Do not dump the catalog.

If `.agents/product-marketing-context.md` exists, read it first.

## Ethics floor

Every recommendation must pass all five:

1. **True** — no fake scarcity, fake social proof, fake progress, fake “most popular.”
2. **Reversible** — agent writes need undo; money writes need a clear exit.
3. **Informed** — feedforward before commit (price, emails, who sees this).
4. **Wanted** — persuasion helps a job the user already has; coercion does not.
5. **Second-order** — name the likely side effect (notification fatigue, streak hostage, zombie subscription).

If a tactic fails the floor, say so and offer the honest version.

Nir Eyal test: would I use this, and does it materially help the user?

## Diagnose first

Every interaction hits Benson’s four problems. Pick the **dominant** one:

| User is… | Bucket | Job |
|---|---|---|
| Overwhelmed, skipping, blind to the CTA | Information | Filter |
| Confused, inventing a story, unsure what this is | Meaning | Make sense |
| Rushing, defaulting, buying/quitting on impulse | Time | Act fast |
| Forgetting, judging the whole by one moment | Memory | Keep a few bits |

Then load **only** the matching reference:

- Information → [information.md](information.md)
- Meaning → [meaning.md](meaning.md)
- Time → [time.md](time.md)
- Memory → [memory.md](memory.md)

Always skim [traps.md](traps.md) before citing a slogan (Miller 7±2, Spark, backfire, ego depletion).

Full one-line index: [catalog.md](catalog.md). Books behind the catalog: [resources.md](resources.md).

## Modes

### Design (building a flow)

1. Name the job-to-be-done and the one success action.
2. Name the bucket and 2–4 principles max.
3. For each: what changes on the screen, and which ethics-floor check it satisfies.
4. Name one thing you will **not** do (the dark twin).

### Audit (reviewing a live surface)

Walk the four buckets in order. For each finding:

- **Principle** — name it
- **Evidence** — what is on the screen
- **Risk** — ethics-floor miss, or user cost
- **Fix** — one concrete change

Severity: blocker (deceptive or irreversible) / should-fix / polish.

Do not grade principles that are not in play. Silence is correct.

### Teach (quiz / explain)

Correct the Growth.Design one-liner if it is sloppy (see traps). Cite the study, not the slogan.

## Common jobs → principles

| Job | Reach for | Not |
|---|---|---|
| First-run / aha | Progressive disclosure, Spark (ability), Reciprocity, Aha moment | Feature tour dump |
| Pricing table | Anchoring, Decoy, Centre-stage, Framing, Social proof | Fake “most popular” |
| Checkout / pay | Default, Loss aversion, Cashless, Feedforward, Fitts | Hidden total, trap exit |
| Habit / return | Hook loop, Variable reward, Investment, Internal trigger, Exit points | Streak hostage |
| Empty / first write | Signifiers, Feedforward, Endowment, IKEA, Chunking | “Nothing here” shame |
| Cancel / offboard | Reactance, Peak-end, Noble edge, Default | Hidden cancel, confirmshaming |
| Notify / re-engage | External vs self-initiated trigger, Reactance | Spray pushes |
| Research / test | Hawthorne, Observer-expectancy, Survey bias, Survivorship | Dogfooding as “users” |

## Output shape

**done**
- Principle → change

**avoid**
- Dark twin you refused

**open**
- What you need from a human (aha definition, constraint, brand rule)

Keep it short. One idea per line.

## Sister skills

- Marketing pages / campaigns → `marketing-psychology`
- Homepage / landing CRO → `page-cro`
- Signup → `signup-flow-cro`
- Post-signup activation → `onboarding-cro`
- Forms / popups / paywall → `form-cro` / `popup-cro` / `paywall-upgrade-cro`
- Visual UI rules → `web-design-guidelines`

This skill is the psychology layer. Those skills are the channel playbooks. Use both when both apply.
