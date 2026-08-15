# Blind-spot pass

What neither of you knows to ask. Hunt unknown unknowns and rank them
by how much they would change the go / no-go / wedge, not by how clever
they sound.

Inherited from [find-unknowns](../../find-unknowns/SKILL.md), with
gstack's Search Before Building layered on.

## Sweep

State coverage: "this pass covered X" (files, product surfaces, public
precedent, or "idea-only — no codebase"). Do not pretend you read what
you did not.

Hunt for:

- **Landmines** — things that bite silently: a kill assumption, a
  legal/distribution gate, a data shape that is wrong by default, a
  prior attempt at the same job and why it died.
- **Unwritten conventions** — rules the code or the market enforces
  that no doc states.
- **Second-order effects** — who else is affected if this works
  (existing users, brand, pricing, focus).
- **Absorption** — is a platform or incumbent about to ship this as a
  checkbox?
- **Half-built paths** — flags, dead code, reverted PRs. The reason
  they died is usually your landmine.

## Techniques (pick what fits)

- **Adversarial framing** — argue the opposite. If the plan assumes
  demand, look for evidence of absence. If it assumes a capability,
  check the weakest link first.
- **Critical-path kill test** — name the one assumption that, if
  false, kills the idea. Verify it first, not last.
- **Precedent scan** — who tried this shape, and what happened to
  them? Be specific. A named failure is worth more than a vibe.
- **Domain teaching** — if the user is new to the domain, teach the
  landscape so they can decide. Do not decide for them in silence.
- **Search before building** (gstack ethos):
  - Layer 1 — tried and true. Don't reinvent. Question it anyway
    once in a while; that is where brilliance hides.
  - Layer 2 — new and popular. Search, then scrutinize. The crowd
    is often manic.
  - Layer 3 — first principles about *this* problem. Prize these.
  - **Eureka:** Layer 3 contradicts the crowd. Name it: "Everyone
    does X because they assume [Y]. [Evidence from this session]
    suggests that's wrong here. So [implication]."

When searching the public web, use generalized category terms, not
the user's stealth name. If they decline search, proceed on what you
already have and say so.

## How to report a finding

Each finding is a card:

- **Evidence** — file and line, a URL, a named precedent, or "inferred
  — not verified"
- **Why it bites**
- **What it changes** about the idea, the wedge, or the go/no-go

A finding that needs a decision closes like a hard question: lettered
options plus your recommendation. A finding that only needs awareness
goes on the map as a sharp edge.

## Rank

Decision-changing first. Interesting-but-irrelevant last, or cut.

**Done when** the sweep's coverage is stated and every material
finding is on the map: decided, OPEN, or sharp-edge.
