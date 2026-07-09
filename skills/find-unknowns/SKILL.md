---
name: find-unknowns
description: Map the unknowns in an idea, feature, or plan before (and during, and after) execution — blind-spot pass, quadrant classification, and a decision-changing interview. Use when the user wants to de-risk a decision, find blind spots, stress-test a pivot/plan, or says "run find-unknowns", "blind spot pass", "what am I missing", "unknown unknowns". Based on "A Field Guide to Fable: Finding Your Unknowns" (@trq212).
---

# Find Unknowns

The map (prompts, plans, context) is not the territory (the codebase, the market, reality). The gap between them is unknowns, and work quality is bottlenecked by how well they get clarified. This skill is an iterative pass to surface them cheaply, before they get expensive.

## Inputs

Ingest everything available about the subject before classifying: the user's stated idea/plan, related vault or repo notes, prior research in the conversation, live product surfaces (landing pages, docs), and the user's own context (who they are, what they already know, where they are in their thought process). If the user hasn't said where they are in their thinking, that's the first interview question.

## Step 1 — Quadrant map

Classify what you've ingested into the four quadrants, explicitly, in writing:

- **Known knowns** — what's already stated or established. Compress; don't re-litigate.
- **Known unknowns** — open questions the user is already aware of. List them so they're tracked, note which are answerable by research vs. only by the user vs. only by shipping.
- **Unknown knowns** — things the user knows but hasn't written down: tacit context, taste ("I'll know it when I see it"), real motivations, constraints so obvious they were never stated. You can't list these directly; you extract them by interviewing and by offering concrete options to react to (people recognize what they want faster than they articulate it).
- **Unknown unknowns** — what nobody in the room has considered. This is the blind-spot pass (Step 2).

## Step 2 — Blind-spot pass

Actively hunt unknown unknowns. Techniques, pick what fits:

- **Adversarial framing**: argue the opposite. If the plan assumes demand, look for evidence of absence; if it assumes a capability, check feasibility at the weakest link.
- **Second-order effects**: who else is affected (existing users, brand, pricing, team focus)? What breaks downstream if this succeeds?
- **Feasibility of the critical path**: find the single technical/legal/distribution assumption that, if false, kills the idea. Verify it first, not last.
- **Precedent scan**: who tried this shape before and what happened to them?
- **Timing/absorption**: is a platform or incumbent about to make this a feature?
- **Domain teaching**: if the user is new to the domain, teach the landscape so they can prompt/decide better, don't just decide for them.

Present findings ranked by how much they'd change the decision, not by how interesting they are.

## Step 3 — Interview

Interview the user about the ambiguities that survive Steps 1-2. Rules:

- Prioritize questions where the answer changes the architecture/strategy; skip anything with a conventional default.
- Small batches (use AskUserQuestion, max 4 at a time), concrete options over open-ended prompts — options extract unknown knowns by recognition.
- Include an honest-signal question when the subject is a decision ("what's actually driving this?") — motivation is the most common unknown known.
- Stop interviewing when remaining unknowns are only resolvable by shipping or research; say which is which.

## Step 4 — Reduce the unknowns

For each surviving unknown, propose the cheapest artifact that converts it to a known, choosing from:

- **Brainstorm/prototype** — several disposable variants to react to (for unknown knowns / taste).
- **Reference** — find an existing implementation/product to point at instead of describing.
- **Research pass** — for facts the internet can settle; be specific about the falsifiable claim to check.
- **Spike/feasibility test** — for the critical-path assumption; timebox it.
- **Implementation plan, decisions-first** — lead with the choices most likely to change (data models, interfaces, user-facing behavior); bury mechanical work at the bottom.

## During execution

Keep an `implementation-notes.md` (or equivalent) with a **Deviations** section: when reality forces a change from the plan, take the conservative option, log it, keep going. Deviations are discovered unknowns — feed them back into the next planning pass.

## After execution

- **Pitch/explainer**: package spec + prototype + deviations into one doc a reviewer can absorb cold, leading with the demo.
- **Quiz**: offer the user a short quiz on what was actually done/decided; gaps in their answers are unknowns that survived and need a follow-up pass.

## Output

Always end a run with: (1) the ranked blind-spot list, (2) what the interview resolved, (3) the remaining unknowns each mapped to its cheapest reduction artifact, (4) a recommendation. Keep it decision-oriented — this skill exists to change what the user does next, not to produce a taxonomy.
