---
name: competitor-research
description: >-
  Competitive intelligence — researching competitors, building a competitive
  intelligence program, cataloging insights for internal teams, and producing
  battlecards, competitive newsletters, and win/loss programs. Use whenever
  the task involves "competitive intelligence," "competitor research,"
  "gathering competitive insights," "who are our competitors," "competitive
  landscape," "battlecard," "competitive newsletter," "win/loss program," or
  "track our competitors." Built entirely from the 10-lesson Competitive
  Intel course in `Product Marketing/Competitive Intel/` — every rule in this
  file traces to a specific lesson quote. Nothing here comes from outside
  that source.
metadata:
  version: 1.0.0
---

# Competitive Intelligence

Competitive intelligence is "researching and discovering insights relating to competitors in your
industry" — the more of it you have, "the more clearly you'll be able to differentiate from those
competitors to your ideal customers" (*What is Competitive Intelligence...*).

## Initial Assessment

Different internal audiences ask fundamentally different competitive questions — "each of these
departments will ask different competitive questions" (*Gathering Insights: Startups & Mid-Market*).
Before researching, confirm:

1. **Which audience is this for?** Sales/marketing (how competitors are *perceived*), product (how
   competitors are *used*), or leadership (how competitors are *trending*)? Each has a different
   question and a different resource set (Research Process below).
2. **How many competitors are being tracked, and is the list capped?** "Only start by tracking and
   informing your sales, product and leadership teams on the most vital few competitors... if you
   reduce that number down to a max of five competitors, you'll find that you can keep up very well"
   (*Pushing "Go"...*). Don't proceed against an uncapped list without flagging this.
3. **What's the budget tier?** Free/affordable resources only (Tier 1), or is there budget for paid
   tools — Crayon/Clue, Chorus.ai, SEMrush, analyst relations, GLG (Tier 2)? "If you've proven out
   your competitive program... or if you work for an organization with a decent budget" is when Tier 2
   applies (*Gathering Insights: Enterprise*).
4. **One-off research, or an ongoing program?** An ongoing program needs the insight-cataloging system
   below; a one-off doesn't.

## Core Principles

1. **Treat internal teams as an audience.** "Thinking of your internal teams as an audience, as your
   customers... If you're going to interrupt their day with competitive insights, it needs to be
   relevant for them as well as written and delivered thoughtfully. Otherwise, your messages will go
   unread or unresponded to" (*Understanding Your Audience*).
2. **Outsider perspective beats internal bias.** "So often we get wrapped into our own bias narrative
   of what our products do and how our company looks. Win loss programs help us experience an
   outsider's perspective while revealing unique competitor value props" (*Win/Loss, part 1*).
3. **Every insight earns its place by relating back to the company.** Before including any finding,
   apply the three-question filter: "How does this relate to my company? Is there a bigger story to
   this? What questions do I have after learning about this?" (*Competitive Newsletters*).
4. **Consistency compounds.** "These are all practices that, when compounded over time, will
   dramatically help your company crush your competitors" (*Pushing "Go"...*).
5. **Cap scope to stay sustainable.** Max 5 tracked competitors — "you'll find that you can keep up
   very well for that small group of competitors... Once you establish a system for those five
   competitors, you can slowly add more" (*Pushing "Go"...*). The list only grows once the system for
   five is demonstrably working, never in anticipation of needing to.

## Insight Cataloging (the persistence layer)

Every finding gets logged, not just used once and discarded — "the idea is moving forward, you'll add
more and more insights" (*Understanding Your Audience*).

- **Tool:** a shared spreadsheet — "we're going to keep things really kindergarten... I'm going to use
  Google Sheets. The reason we're using Google Sheets is because everyone has access to it," and the
  format ports to "essentially any other note taking tool."
- **Columns:** link to the insight; "in your own words, write a 1 to 2 sentence summary"; the team(s)
  it benefits — "sales, marketing, product, C-suite, or another team."
- **Cadence:** monthly by default — "that's the sweet spot because it's enough time for a decent
  number of changes to occur, but not so long that you appear to be MIA." Explicit exception:
  "large competitive updates like acquisitions, funding rounds, new major product releases... try to
  report on them as they occur," not held for the monthly batch.
- **Re-confirm what each team actually cares about every few months**, not just once at setup —
  "every few months reach back out to them and confirm what they're interested in."

## Saving Raw Data

*Imported from `competitor-profiling`, not the course — the course describes the insight-ledger
spreadsheet above, but nothing about persisting raw source material. Added after a real failure: a
research pass cited G2/Trustpilot/Capterra ratings pulled from a search-result snippet instead of
actually navigating to each review site and reading filtered review content, and the finished profile
looked equally polished either way — the formatting hid that the research step had been shortcut.
This section exists specifically so that can't happen invisibly again.*

**The rule: no citation without a corresponding raw file.** Every source actually used in a deliverable
must be saved to disk before that deliverable is written — not summarized from memory, not typed
straight into a template field. If a raw file for a source doesn't exist, that source cannot be cited;
the deliverable must say "not collected this run" instead.

**Directory layout** (relative to project root):

```
competitor-profiles/
├── raw/
│   └── <competitor-slug>/
│       └── <YYYY-MM-DD>/
│           ├── scrapes/    # homepage.md, pricing.md, product.md, ...
│           ├── reviews/    # g2.md, trustradius.md, capterra.md, ... — the actual filtered/quoted
│           │                 review text, not just a star rating
│           └── community/  # reddit.md, quora.md, ... — actual quoted threads, or an explicit
│                              "no results found" note if a platform search came up empty
├── <competitor-slug>.md    # the finished Competitor Profile / battlecard / newsletter item / etc.
└── _summary.md             # cross-competitor summary, when more than one is profiled
```

**Specifically for the G2/TrustRadius technique** (Core Principle territory, *Gathering Insights:
Startups & Mid-Market*): `reviews/g2.md` must contain the actual review text pulled after filtering to
1-3 stars and searching by a relevant keyword, with reviewer/date where shown — not an aggregate rating
copied from a search snippet. A star rating alone does not satisfy this file's purpose.

**Never create the date folder retroactively to make a shortcut look compliant** — if the raw file
doesn't already exist when the deliverable is being written, the research wasn't actually done yet; go
do it, or mark the source as not collected.

## Research Process

### Tier 1 — Free & affordable resources (default)

**Marketing/Sales question — how is this competitor *perceived*?**
- **Homepage** — read positioning directly from the copy (worked example: HubSpot's "learn and grow"
  copy reads as "a growth tool primarily for startups or small businesses").
- **G2 / TrustRadius** — "like Yelp for B2B software." Technique: "filter down to only 1 to 3 star
  reviews... The search bar can also be used to find reviews that include specific keywords," sorted
  by most recent. Named caveat: review incentives ("$10 Amazon gift cards") produce a share of
  minimalist, low-signal reviews — still worth using, just don't treat every review as equally honest.
- **Social communities** — Reddit, Quora, Facebook groups, Discord, Slack: "just Google your
  competitor's name and add Reddit." Higher signal than review sites because "these are channels
  where folks are just hanging out. They had zero obligation to be there."

**Product question — how is this competitor *used*?**
- **The competitor's own customer knowledge center** (not the homepage) — FAQs, UI screenshots,
  walkthroughs.
- **G2/TrustRadius, filtered to feature-specific feedback** rather than general sentiment.
- **Google Alerts** — free, keyword-based: "type in a few keywords... Google will automatically
  populate a preview." Customizable by frequency, source, language, region, and delivery email.

**Leadership question — how is this competitor *trending*?**
- **LinkedIn Premium's Insights tab** — "employee headcount trends over the past year and a half...
  a pretty good proxy for when a company is on a hiring spree" (or, if declining, business weakness).
  Named reason it matters: most competitors are "privately held companies that don't share their
  annual revenue."

### Tier 2 — Paid & enterprise resources (once Tier 1 is proven out, or budget allows)

Why upgrade: Google Alerts breaks down once tracking grows — "tracking 9 or 10 vendors... becomes
25, 35, 40... a recipe for disaster... your inbox is going to be bombarded" (*Gathering Insights:
Enterprise*).

- **Crayon / Clue** — aggregate a competitor's entire digital footprint (Reddit/Quora, social, site
  changes, content, news/PR, reviews) into one filterable, alertable feed; both also have native
  battlecard filters synced to the feed.
- **Chorus.ai** — conversation intelligence: tracks and flags competitor mentions in real sales calls
  and emails, with keyword playlists across calls (worked example: a playlist on "expensive" pulling
  15 of 20 closed-lost calls surfaces a trend fast). This is the resource that reveals how *often* a
  competitor actually comes up in real deals and how sellers currently talk about them. Worked story:
  rising Chorus mention frequency for a small competitor led to discovering they were bidding on
  branded keywords via SEM, which led to new seller talk tracks.
- **SEMrush** — competitor website traffic, traffic source, estimated market size. "Partner with your
  SEO and SEM teams for competitive Intel. They have access to a lot of great under the radar
  information."
- **Analyst relations (Forrester, Gartner)** — paid access to industry reports and 1:1 analyst
  inquiries; "industry experts['] non-biased opinion" on where the company differentiates.
- **Network consultants (GLG)** — anonymous consultations with former executives of a target
  competitor; best source for real GTM strategy, pricing, and product detail a public site won't show.

### Synthesis

Route every finding through the Insight Cataloging log above, filtered by the three-question test
(Core Principle 3) before it earns a place in any downstream deliverable.

## Output Formats

Different deliverables for different audiences and different moments — not one template. Full
ready-to-use versions of each are in `references/templates.md`; tool-by-tool execution detail is in
`references/tool-reference.md`.

- **Competitor profile** *(imported from `competitor-profiling`, not the course — see
  `references/templates.md`)* — the default for a plain "research/profile [company]" request that
  isn't scoped to one of the audience-specific deliverables below. Quick scan by default; deep profile
  only if requested or 3 or fewer competitors are in scope.
- **Summary document** *(same import)* — after profiling more than one competitor. `references/templates.md` also carries the rest of that skill's output format: the page-by-page extraction table, Quick Scan, side-by-side comparison, positioning map, Competitive SWOT, and Change Log.
- **Insight ledger** — the always-on running log (columns above).
- **Battlecard** (sales/marketing) — quick dismiss first, then email template, then everything else.
- **Newsletter** (product/C-suite) — table-of-contents first, per-item structure, three-question filter.
- **Win/loss survey** (quantitative) — ≤10 questions, under 5 minutes.
- **Win/loss interview guide** (qualitative) — reused from the survey, opened up for follow-up.
- **Displacement campaign plan** — audience selection, contact list build, SEM/SEO plays.

**Never generate all of these preemptively for a single research request.** Build them in the order
given below, only when actually asked for.

## Build Order (standing up a program, not a one-off)

"Start building out battlecards and newsletters that focus on their strategic updates... Then start
your win loss program and focus only on competitive deals where you've won or lost against one of
those five vendors. And lastly, start collaborating with your marketing team on proactive, competitive
email campaigns and SEM SEO" (*Pushing "Go"...*). In order: insight cataloging → battlecards +
newsletter → win/loss program → displacement campaigns.

## Cadence

"Update your Battlecards every 45 to 60 days. Don't skip a month with your newsletter. Don't let six
months go by without speaking to a closed loss or closed won account" (*Pushing "Go"...*). Immediate
exception, not held for a batch: acquisitions, funding rounds, major product releases (Insight
Cataloging above).

## The Goal (not the deliverable count)

"Your goal should never be to just create an arbitrary number of battlecards or newsletters, or to
interview a certain number of people... the goal should drive back to a business critical metric like
revenue or win rate" (*Pushing "Go"...*). Competitive win rate = won competitive deals ÷ (won + lost)
within a time frame, tracked overall **and per competitor** — a low per-competitor rate on one of the
tracked five is the direct signal for where to focus next, not a guess.

## Win/Loss and Displacement Campaigns — a structural limit

Both require the target company's own CRM and direct access to its real prospects/customers — "the
main point of contact at the account" for interviews, or "your CRM data" and outbound infrastructure
for displacement. **Mark N/A for arm's-length external research** (researching a company from outside,
for interview prep or a positioning exercise) and say so plainly — don't attempt a workaround. Full
methodology is in `references/templates.md` and `references/tool-reference.md`, ready the moment this
skill runs from inside the company rather than researching it.

## Constraints

- **No citation without a corresponding raw file** (see Saving Raw Data above). This is the primary
  constraint in this file — everything else assumes it holds.
- Never state a fact from memory. Verify live or say "unknown."
- Never treat a missing tool (no Semrush, no LinkedIn Premium, no Chorus.ai) as a reason to guess —
  state the substitute used and the gap plainly. Some Tier 2 resources are structurally unavailable in
  a given session (no paid account, no standing relationship) — that's a real ceiling, not something a
  better prompt fixes; say so rather than faking the data.
- Never ship the maximal deliverable set when a smaller one was asked for.

## Task-Specific Questions

Only ask if not already answered:

1. Which competitor(s) or market are we researching, and is the list capped at 5?
2. Which internal audience is this for — sales/marketing, product, or leadership?
3. Tier 1 (free) only, or is Tier 2 (paid/enterprise) available?
4. Is this a one-off profile, or does it need to enter the ongoing insight ledger?

## Related

- `references/templates.md` and `references/tool-reference.md` in this same skill carry the
  deliverable-specific and tool-specific depth — read them when the task calls for that specific
  artifact, not by default on every run.
- `Workflows/market-intelligence-scan.md` — a genuinely separate, ongoing category-level watchlist job
  (regulation, funding climate, category narrative), not a substitute for this skill or vice versa.
- `Workflows/battlecard-weekly-refresh.md` — keeps this skill's battlecards current between full
  research passes.
