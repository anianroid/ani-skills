# Reddit field notes (opt-in platform pack)

Reddit is not a distribution channel; it is a community you contribute to. The
post is the author sharing what they learned, complete in itself, with nothing
to click. If the piece has no genuine lesson or no community where it fits,
skip Reddit for that piece and say so. A skipped post is always better than a
salesy one.

Researched 2026-07-06 (two research agents, rules via third-party catalogs and
archive APIs; Reddit blocks direct crawls). Re-verify a sub's rules in-app for
60 seconds before posting; automod settings change.

## The one rule that dominates everything

Mid-2026 Reddit punishes AI-LOOKING WRITING harder than AI topics. Ironically,
the Claude subs are the harshest about posts that read like Claude. Symmetric
numbered frameworks, tidy triads, "it's not X, it's Y" constructions, em-dash
cadence, and grammatically perfect prose are all tells (polished posts get ~3x
more downvotes in business subs). The field-notes post must be a war story
that happens to contain the lessons, not a framework with anecdotes attached.
Required: at least one concrete failure, real numbers, a real artifact (an
actual prompt, a before/after), short rough paragraphs, and the author's own
loose register. Never port essay prose.

## Link etiquette (consensus across all subs)

- Full value in the post. Never a teaser.
- No link in the body. On strict subs (r/AI_Agents, r/marketing), no link
  anywhere including comments.
- Do not volunteer "link in comments"; that reads as growth-hack now. If
  someone asks, "I wrote a longer version, happy to share" and reply with it.
- Never post the same text to two subs, and never post two subs the same day.
  Stagger 5 to 7 days, each with its own framing. Simultaneous crossposting is
  itself a spam signal.
- Account should have some comment history in the target sub (mods review
  account history). Engage in comments for hours after posting.

## Target tiers (for AI-workflow / delegation / briefing content)

### Tier 1
- **r/ClaudeAI** (~1M, very active). Workflow posts are the sub's best genre;
  use the "Claude Code Workflow" flair if Code-specific. Contrarian workflow
  titles with a number perform ("After N weeks of X, ...: 6 things"). Mood
  swings around releases and rate limits; avoid launch-drama days.
- **r/agency** (~94k, fast-growing). Best operator fit for briefing/delegation
  content; briefs ARE the agency business. Small sub, gives practitioners the
  benefit of the doubt. Verify current rules in-app (not crawlable).

### Tier 2
- **r/AI_Agents** (~396k). Post-mortems about autonomous runs are the native
  genre and failure threads are unusually honest. Text-only; automod strips
  links; zero links even in comments.
- **r/ClaudeCode** (~342k, flooded; posts bury fast). Same genre as ClaudeAI;
  post the winner of ClaudeAI here a week later. Check for prior similar
  posts first so the post doesn't look derivative; cite or differentiate.
- **r/DigitalMarketing** (~433k). Practitioner Q&A culture; AI workflow is a
  top recurring theme. Tactical how-I-brief framing.
- **r/EntrepreneurRideAlong** (~707k). Journey framing ("N months of
  delegating real deliverables: what broke"). Lightest moderation; diluted
  audience.
- **r/PromptEngineering** (~395k, text-only). Works when the thesis is
  contrarian FOR that sub ("prompting was never my bottleneck").

### Tier 3 (only with careful sub-specific rewrite and full rule-reading)
- **r/startups** (2.1M): mandatory flair, automod technicalities (historically
  required the literal phrase "I will not promote" in the body); discussion
  framing ending on a real question.
- **r/marketing** (2M): zero-tolerance promo enforcement, no own-site links
  ever; drop "AI" from the title, make it about briefing.
- **r/Entrepreneur** (5.2M): ground zero for AI-slop cynicism; "Lessons
  Learned" flair; one shot, lead with a failure.
- **r/SaaS** (745k): survives easily, engagement lottery, audience is largely
  other founders farming. Free secondary crosspost; don't judge quality by it.

### Skip
- **r/Anthropic** (complaint-dominated), **r/productivity** (explicit no-AI-
  content rule), **r/smallbusiness** ("how I use AI" is a recognized
  consultant lead-gen pattern there), **r/ChatGPTPro** (wrong brand room,
  approval-queue black box), **r/aipromptprogramming** (low energy),
  **r/ArtificialInteligence** (generalist; only with a tool-agnostic rewrite).

## Post shape that wins (2025-2026 pattern)

- Title: time-in-trenches + number + payoff, mildly contrarian. "After 6
  months of X, here's what actually works."
- 400-900 words. Bold mini-headers or a loose numbered list. Short paragraphs.
- First person, specific stakes, at least one thing that went wrong.
- One real artifact: an actual prompt snippet, a real before/after.
- End by asking what others do, and mean it.

## Sequencing template for a piece

1. Tier-1 sub with the best content fit, native framing.
2. 5-7 days later: second community, rewritten (different lead story, different
   angle), not a crosspost.
3. Optional tier-2/3 only if the first two landed and the author wants more.
Log each post and its reception in the piece's Workshop for the next run.
