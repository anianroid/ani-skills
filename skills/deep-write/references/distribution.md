# Distribution playbook (X + LinkedIn), 2026

This is the research-backed spec for spinning an essay into social distribution.
Produce an X thread and a native LinkedIn post for every piece, plus an optional
PDF carousel for higher LinkedIn reach.

## The link rule (most important thing on this page)

Links suppress reach. Handle them per platform:

- **LinkedIn:** a link in the post body costs roughly 60% of reach. Write a post
  that is complete without the click, then put the link in the **first comment**,
  which you post yourself immediately. A repackaged PDF carousel or a LinkedIn
  Article also sidesteps the penalty. (Recent updates also trim reach on detected
  "bridge" posts, so the post must stand on its own.)
- **X:** a link in the first tweet costs 30 to 50%+ of reach. Keep tweet 1
  link-free. Put the URL in the **final tweet or a self-reply**. Replies are
  weighted far above likes, so the whole game is conversation.

## The provocative-hook variant (occasional, both platforms)

Once in a while, deliberately run an engagement-farming hook instead of the
standard evidence-first open. This is a documented outperformer: the author's
best post ever (34.6k impressions, 55 comments in 4 days, vs a typical essay
post) led with the target's own provocative words, verbatim, as the entire
hook, with a native video clip of the target attached.

The recipe, when a piece answers a named take:
- **Hook = the target's exact quote, in quotation marks, no setup.** Borrow
  their authority and invite the fight in line one.
- **Media = a native clip of the target saying it** (video beats card links
  and text on both platforms).
- **Structure = direct rebuttal**, concede-then-turn, so disagreement lands in
  the comments instead of scrolling past.
- **Ship the aggressive cut.** Draft a measured cut too, but the sharp one is
  the one that travels.

Guardrails: this is a spice, not the default. Use it at most one post in a
handful, only when the substance can survive the heat (a real named take, a
defensible counter-argument), and never manufacture outrage the essay doesn't
actually contain. Offer it as an option at Stage 6 when the piece has a named
target; skip it for pure-thesis pieces.

## Execution conventions

- **The first 60 to 90 minutes on LinkedIn, 30 to 60 on X, is the ranking
  window.** Reply to every comment and reply immediately. Rally teammates for
  substantive comments, not bare reactions.
- **End every post on a question** to pull comments.
- **Media on the hook lifts reach.** A diagram on X tweet 1, a carousel on
  LinkedIn.
- **Two tagging mechanisms, kept strictly separate:**
  1. **In-thread @ = genuine attribution only.** Research authors, and the
     ecosystem frameworks you actually serve. Never a forced cc. Never tag the
     person or genre you are critiquing.
  2. **Quote-tweets = separate standalone posts,** spaced across launch day.
     This is where reposts come from. The single highest-leverage move is to QT
     the exact post you are rebutting and borrow its audience, in your own
     respectful words.

**QT targets must be real, found, and linked (never buck-passed).** Do not write
"find a fresh post about X and QT it." That is homework, not a deliverable. Go
find the actual post: web-search for it, get the `x.com/<user>/status/<id>` URL,
curl it to confirm it resolves and is recent, and drop it into the copy with the
QT text already written against that specific post. Only leave a target as a TODO
when it is genuinely unfetchable (the author's own private-timeline links, or a
handle whose recent posts you cannot see), and then say so explicitly and note
what you checked. See SKILL.md operating principle 7b.

## Launch-day sequence

- Morning (Tue to Thu, roughly 9 to 11am audience time): post the X thread, then
  self-reply with the link, then engage.
- Same morning: post the LinkedIn native post, add the first-comment link, then
  engage.
- Midday and afternoon: spaced quote-tweets.
- Next day: reshare or post the carousel.

## X format: numbered thread vs single long-form post

Default is a numbered thread (below). If the author has X Premium, offer a
single flowing long-form post instead, especially for narrative/story-shaped
pieces (a debugging postmortem, a founder story). Numbered tweets create
artificial beat boundaries, and this author's drafts specifically show a
tendency to fill each boundary with a "label: reveal" tee-up (see
`references/no-ai-slop.md`) to make the next tweet feel earned. The same story
told as continuous prose usually needs none of those tee-ups and reads less
AI-ish, not more, despite being longer. Keep the same hook-first opening,
link-at-the-end rule, and aphoristic close either way. Run the no-ai-slop check
on whichever version ships.

## X thread shape

Link-free hook tweet leading with the contrarian number and a 🧵. One idea per
numbered tweet, mirroring the essay sections. Genuine @-attribution inline.
Disclosure inline if relevant. Link only in the final tweet. Aphoristic closer.
No hashtags on X.

### Few-shot: verbatim X thread ("The Real Alpha Is Boring")

```
1/ Everyone's selling the same play right now: build flashy Claude agents for small businesses, charge a $2.5k/mo retainer, stack 8 clients, $20k/mo.
The math is real. It's just pointing at the wrong number.
The real alpha in agents-for-business is boring. 🧵

2/ The demo is the easy part now. The agent that wows in a 2-min Loom is the first to break in production.
Gartner: 40%+ of agentic projects cancelled by 2027.
That retainer isn't a feature. It's the tell, you're being paid to keep a fragile thing alive.

3/ The agents still running in month six aren't the dazzling ones. They're invoicing. Reconciliation. Ticket triage. Lead routing.
Narrow, repeatable, unglamorous. Nobody films a Loom about an accounts-receivable agent. Which is exactly why it's still billing in month six.

4/ Why does boring survive and flashy die?
@garrytan + Steve Yegge's "thin harness, fat skills": push judgment up into skills, execution down into deterministic tooling.
A model can seat 8 at a dinner table. Ask it to seat 800 and it hallucinates a confident, wrong chart.

5/ Reliability is the product.
@FoundationCap sizes "service-as-software" at $4.6T and nails the line: buyers don't purchase software, they purchase outcomes.
An SMB isn't buying an agent. They're buying an invoice that goes out on its own, every time. Boring = dependable.

6/ Then the decision the pitch skips entirely: build your own harness, or rent it?
Build is catnip. OpenClaw (@steipete) and Hermes (@Teknium) are spectacular, full control, data sovereignty, open weights.
But you become the thing you maintain.

7/ OpenClaw's first months: a critical RCE, 100k+ instances exposed, ~12% of community skills malicious. No security team, it's brilliant OSS, not a vendor.
Multiply across a client roster and each one's a snowflake server you patch at 2am. You bought yourself a sysadmin job.

8/ For ~90% of cases you should rent, not build. Hand-roll a harness only when it's your core IP, and a dentist's invoicing isn't core IP.
Managed platforms (I work on @duet) own hosting, integrations, guardrails, patching. You bring the skill and the client, not the plumbing.

9/ The harness is a commodity. Anthropic literally shipped Claude Code's source to npm by accident.
Your skills and client relationships are the only things that don't.
Build for the demo, you get churn. Build for Tuesday, you get a business.
ani.computer/writings/boring-agents
```

Highest-leverage quote-tweet copy (rebut the exact post, respectfully):

> Genuinely useful breakdown, and the math works. One push-back: it points at
> the wrong number. The agents that survive production are boring, and the margin
> is in renting your harness, not building it. The case: [link]

## LinkedIn post shape

Native long-form text, complete without a click. Hook in the first two lines
(roughly 210 characters before the "See more" fold), leading with the contrarian
number. Short one-to-three-sentence paragraphs with whitespace between them.
Broetry is dead: lead with expertise, not one-word lines. A single 👇 plus a
closing question. Five trailing hashtags. Link in the first comment. One sparing
tag of your own company page (it reshares). Higher-reach variant: an 8 to 10
slide PDF carousel in 4:5 portrait, editorial style, link on the final slide.

### Few-shot: verbatim LinkedIn post ("The Real Alpha Is Boring")

```
There's a pitch all over my feed right now: build flashy AI agents for small businesses, charge a $2,500/mo retainer, stack 8 clients, hit $20k/mo.

The math works. It's just pointing at the wrong number.

Everyone's running the same play. Wire up n8n and the Claude API, film a 2-minute Loom of a lead form turning into a CRM update, sell it on retainer.

But the demo is the easy part now. The agent that wows in a Loom is the first one to break in production. Gartner expects 40%+ of agentic AI projects to be cancelled by 2027, mostly on cost, unclear value, and weak reliability.

So that retainer isn't a feature. It's the tell. You're not being paid to build. You're being paid to stand between a fragile system and the client who'll notice the second it breaks.

Here's what the Loom never shows: the agents still running in month six are the boring ones. Invoicing. Reconciliation. Ticket triage. Lead routing. Nobody films a Loom about an accounts-receivable agent, which is exactly why it's still billing.

Boring isn't the consolation prize. Boring is the moat.

And there's a second mistake hiding under the first: building your own harness. OpenClaw and Hermes are spectacular tools, but the day you self-host them across a roster of clients, you've bought yourself a sysadmin job, patching snowflake servers at 2am. For ~90% of cases you should rent the infrastructure, not build it. Hand-roll a harness only when it's your core IP, and a dentist's invoicing isn't core IP.

The harness is a commodity. The only things that don't commoditize are your skills and your client relationships.

Build for the demo, you get a great Loom and a churn problem. Build for Tuesday morning, the reconciliation that has to run whether or not anyone's watching, and you get a business.

(Disclosure: I work on Duet, a managed agent platform, so I have a horse in the build-vs-buy race. The argument holds without it.)

What's the most boring agent you'd actually pay to keep running? 👇

#AIagents #automation #SMB #AItools #founders
```

First comment (posted by the author immediately):

> Full essay, with the data and the build-vs-buy math: [link] short version: the
> boring agent nobody demos is the one still running in month six.

## The tagging plan (write one per piece)

- **Attribution @s (in-thread):** list the research authors and frameworks you
  cite and genuinely serve.
- **Quote-tweet targets (standalone posts):** the exact post(s) you are
  rebutting or building on. Spaced across the day. Draft the QT copy.
- **Do not tag:** the person or genre you are critiquing, in-thread.
