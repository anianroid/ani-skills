# Hard questions

Ask **one at a time**. Push until the answer is specific and evidenced.
Smart-skip any question already answered with a name, a number, or a
behavior. After each answer, take a position and state what evidence
would change it.

These are adapted from Garry Tan's gstack `/office-hours` (Idea / Builder)
and `/plan-ceo-review` (Feature). Do not paste gstack's YC pitch, telemetry,
or design-doc machinery. The questions are the inheritance.

---

## Idea mode (new product or company)

Route by stage. You do not always need all six.

- Pre-product → Q1, Q2, Q3
- Has users, not paying → Q2, Q4, Q5
- Has paying customers → Q4, Q5, Q6
- Internal / intrapreneur → Q4 becomes "smallest demo that gets the
  sponsor to greenlight"; Q6 becomes "does this survive a reorg, or die
  when the champion leaves?"

### Q1 — Demand reality

"What's the strongest evidence someone actually wants this — not
'interested,' not a waitlist, but would be upset if it disappeared
tomorrow?"

Push until you hear behavior: paying, expanding usage, building a
workflow around it, scrambling if it vanished.

Red flags: "people say it's interesting," waitlist signups, "VCs like
the space."

After the first answer, check framing before continuing:

1. Undefined terms ("AI space," "seamless," "better platform") — make
   them measurable.
2. Hidden assumptions ("I need to raise," "the market needs this") —
   name one and ask if it is verified.
3. Real vs hypothetical — "I think developers would want" is a thought
   experiment. "Three people at my last company spent 10 hours a week
   on this" is real.

If the framing is wrong, restate: "I think you're actually building
[reframe]. Closer?" Then continue with the corrected framing. Sixty
seconds, not ten minutes.

### Q2 — Status quo

"What are they doing right now to solve this, even badly? What does
that workaround cost them?"

Push until you hear a workflow, hours, dollars, duct-taped tools, or a
human hired to do it manually.

Red flag: "Nothing — that's why the opportunity is so big." If no one
is doing anything, the pain is probably not sharp enough.

### Q3 — Desperate specificity

"Name the actual human who needs this most. Title? What gets them
promoted, fired, or kept up at night?"

Push until you hear a name, a role, a consequence. Ideally something
heard from that person's mouth.

Red flags: "healthcare enterprises," "SMBs," "marketing teams." You
cannot email a category.

Match the consequence to the domain: B2B = career; consumer = daily
pain or social moment; hobby = the weekend project that gets unblocked.
Never accept "users."

### Q4 — Narrowest wedge

"What's the smallest version someone would pay real money for this
week — not after you build the platform?"

Push until you hear one feature or one workflow, shippable in days.

Red flags: "we need the full platform first," "stripped down it
wouldn't be differentiated." That is attachment to architecture, not
value.

Bonus: "What if they got value with no login, no integration, no
setup. What does that look like?"

### Q5 — Observation and surprise

"Have you watched someone use this without helping them? What did they
do that surprised you?"

Push until you hear a specific surprise. Users doing something the
product was not designed for is often the real product.

Red flags: surveys, demo calls, "nothing surprising, going as
expected." Surveys lie. Demos are theater. "As expected" means filtered
through existing assumptions.

### Q6 — Future-fit

"If the world looks different in 3 years — and it will — does this
become more essential or less?"

Push until you hear a specific claim about how the user's world
changes and why that change makes this more valuable. Not "AI gets
better so we get better." Every competitor can say that.

Red flags: market CAGR, rising-tide arguments.

---

## Feature mode (big change to something that exists)

Ask these one at a time. Highest architectural blast radius first.

### F1 — Right problem vs proxy

"Is this the right problem? What user or business outcome are we
actually after, and is this the most direct path — or a proxy?"

Push until the outcome is observable (a user sees, waits, loses, or
gains something). "Make X more seamless" is a feeling, not a feature.
Name the step that drops people and the rate, if it exists.

### F2 — Do nothing

"What happens if we ship nothing? Who hurts, in what workflow, by
when?"

If the honest answer is "nobody this quarter," the feature is a
want, not a need. Say so.

### F3 — Existing leverage

"What already partially solves this in the codebase or the product?
Are we rebuilding a parallel path?"

Go read before asking. Show the found answer. Rebuilding needs a
why that beats refactoring.

### F4 — Kill assumption

"What is the single technical, legal, or distribution assumption that,
if false, kills this feature? Why aren't we verifying that first?"

### F5 — Second-order effects

"If this succeeds, what breaks: existing users, pricing, brand, team
focus, a downstream system?"

### F6 — What we will not do

"Name the three things we are explicitly not building. If you cannot,
the feature does not have a wedge."

### F7 — 12-month dream state

Sketch:

```
CURRENT STATE  -->  THIS FEATURE  -->  12-MONTH IDEAL
```

Does this walk toward the ideal or sideways? If sideways, say so and
offer the path that walks toward it.

### F8 — Motivation (unknown known)

"What's actually driving this — a user, a deadline, a competitor, a
bored builder, a metric that stopped meaning anything?"

Motivation is the most common unstated constraint. It changes the
architecture.

---

## Builder mode (side project, hack, learning)

Generative, not interrogative — but still hunt landmines. One at a
time.

1. "What's the coolest version of this? What would make someone say
   whoa?"
2. "Who would you show it to, and what would make them care?"
3. "What's the fastest path to something you can use or share?"
4. "What existing thing is closest, and how is yours different?"
5. "What's the one assumption that, if false, makes this not worth
   a weekend?"

If they upgrade to "this could be a company," switch to Idea mode
and say so.

---

## Pushback patterns (use these, do not go soft)

**Vague market → force a name**
- Soft: "That's a big market. What kind of tool?"
- Hard: "There are 10,000 of these. What specific task does a
  specific person waste 2+ hours a week on? Name the person."

**Social proof → demand test**
- Soft: "That's encouraging. Who have you talked to?"
- Hard: "Loving an idea is free. Has anyone offered to pay, asked
  when it ships, or gotten angry when a prototype broke?"

**Platform vision → wedge**
- Soft: "What would a stripped-down version look like?"
- Hard: "If no one gets value from a smaller version, the value
  isn't clear yet. What would someone pay for this week?"

**Growth stat → thesis**
- Soft: "Strong tailwind. How do you capture it?"
- Hard: "Every competitor cites that stat. What's your thesis about
  how the world changes in a way that makes *this* essential?"

**Undefined term → measure**
- Soft: "What does onboarding look like today?"
- Hard: "'Seamless' is a feeling. Which step drops people? What's
  the rate? Have you watched someone go through it?"

---

## Escape hatch

Impatient once: ask the two highest-blast-radius remaining questions
for the mode, then move to premises.

Impatient twice: jump to premises + alternatives.

Full skip of this file only if they already gave names, evidenced
demand or usage, and a wedge. Premises and alternatives still run.
