# Competitive Intelligence Templates

Ready-to-use templates for every deliverable this skill produces. Six of these (Insight Ledger,
Battlecard, Newsletter, Win/Loss Survey, Win/Loss Interview Guide, Displacement Campaign Plan) trace to
a specific lesson in `Product Marketing/Competitive Intel/`. The Competitor Profile and Summary
Document templates are a deliberate import from the `competitor-profiling` skill — the 10-lesson course
never describes a single synthesized profile document, only audience-specific deliverables, and a
one-off "research this company" request needs a profile shape those six don't provide. Marked clearly
below so provenance stays honest. Pick the template that matches what was actually asked for — don't
produce more than one deliverable unless asked.

## Contents
- Competitor Profile *(imported from `competitor-profiling`)*
- Summary Document *(imported from `competitor-profiling`)*
- Insight Ledger
- Battlecard
- Newsletter
- Win/Loss Survey
- Win/Loss Interview Guide
- Displacement Campaign Plan

---

## Competitor Profile

*Source: imported from the `competitor-profiling` skill (`~/.agents/skills/competitor-profiling/`),
not the Competitive Intel course. Use for "research this competitor" / "profile [company]" requests
that don't map to a specific audience deliverable below.*

```markdown
# [Competitor Name] — Competitor Profile

**URL**: [website]
**Generated**: [date]
**Depth**: [quick scan / deep profile]

---

## At a Glance

| Metric | Value |
|--------|-------|
| Tagline | [from homepage] |
| Founded | [year] |
| Headquarters | [location] |
| Team size | [estimate] |
| Funding | [if known] |
| Domain rank | [from whatever SEO tool is available this session] |
| Est. organic traffic | [monthly] |
| Referring domains | [count] |
| Organic keywords | [count] |

---

## Positioning & Messaging

**Primary value proposition**: [headline + subheadline from homepage]

**Target audience**: [who they're speaking to, based on copy analysis]

**Positioning angle**: [how they position — e.g., "simplicity-first," "enterprise-grade," "all-in-one"]

**Key messaging themes**:
- [theme 1 — with source page]
- [theme 2]
- [theme 3]

---

## Product & Features

### Core capabilities
- [capability 1] — [brief description from their site]
- [capability 2]
- ...

### Notable differentiators
- [what they emphasize as unique]

### Integrations
- [count] integrations
- Key: [list top 5-10]

### Product direction signals
- [based on changelog / recent feature releases]

---

## Pricing

| Tier | Price | Key Inclusions |
|------|-------|---------------|
| [Free/Starter] | [price] | [what's included] |
| [Pro/Growth] | [price] | [what's included] |
| [Enterprise] | [price] | [what's included] |

**Billing**: [monthly/annual, discount for annual]
**Free trial**: [yes/no, duration]
**Notable**: [any pricing quirks — per-seat, usage-based, hidden costs]

---

## Customers & Social Proof

**Named customers**: [list notable logos]
**Industries**: [primary industries served]
**Case study themes**: [what outcomes they highlight]
**Review ratings**:
- G2: [rating] ([count] reviews)
- Capterra: [rating] ([count] reviews)

---

## SEO & Content Strategy

**Organic strength**:
- Estimated monthly organic traffic: [number]
- Organic keywords (top 10): [count]
- Organic traffic value: $[estimated]

**Top organic pages** (by estimated traffic):
1. [page URL] — [keyword] — [est. traffic]
2. [page URL] — [keyword] — [est. traffic]
3. [page URL] — [keyword] — [est. traffic]

**Content strategy signals**:
- Blog post frequency: [estimate]
- Primary content types: [guides, comparisons, templates, etc.]
- Content focus areas: [topics they invest in]

**Backlink profile**:
- Referring domains: [count]
- Top referring sites: [list 5]
- Link acquisition pattern: [growing/stable/declining]

---

## Strengths & Weaknesses

### Strengths
- [strength 1 — with evidence source]
- [strength 2]
- [strength 3]

### Weaknesses
- [weakness 1 — with evidence source]
- [weakness 2]
- [weakness 3]

---

## Competitive Implications for [Your Product]

**Where they're strong vs. us**: [areas where this competitor has an advantage]

**Where we're strong vs. them**: [areas where you have an advantage]

**Opportunities**: [gaps in their offering or positioning we can exploit]

**Threats**: [areas where they're improving or gaining ground]

---

## Raw Data Sources

- Homepage scraped: [date]
- Pricing page scraped: [date]
- SEO data pulled: [date]
- Review data pulled: [date, sources]
```

**Depth default:** quick scan (At a Glance + Positioning + Pricing + SEO summary only) unless deep
profiling is requested or 3 or fewer competitors are in scope — matches this skill's own Tier
1/Tier 2 depth split. Fields with no data available this session should say so plainly (e.g. "not
collected — [tool] unavailable this session"), never left as an unfilled placeholder pretending to be
checked.

---

## Summary Document

*Source: imported from `competitor-profiling`. Use after profiling more than one competitor.*

After profiling all competitors, produce a summary covering:

1. **Competitor landscape overview** — one paragraph summarizing the competitive field
2. **Comparison table** — key metrics side by side for all profiled competitors
3. **Positioning map** — where each competitor sits (e.g., simple↔complex, cheap↔premium)
4. **Key takeaways** — 3-5 strategic observations from the research
5. **Gaps and opportunities** — where the market is underserved

---

## Insight Ledger

Source: *Understanding Your Audience*. The always-on running log every other deliverable draws from.

```markdown
| Link | Summary (1-2 sentences, your own words) | Team(s) it benefits | Date | Urgent? |
|------|------------------------------------------|----------------------|------|---------|
| [url] | [summary] | Sales / Marketing / Product / C-suite / Other | [date] | Yes (acquisition/funding/major release) / No (monthly batch) |
```

Re-confirm what each team actually wants updated on every few months — this log's shape doesn't
change, but which rows get surfaced to which team should be re-checked as the company evolves.

---

## Battlecard

Source: *Building Battlecards for Sales & Marketing Teams*. "95% of the time" the reader just wants to
get the competitor out of the conversation fast — structure reflects that, in this exact order.

```markdown
# [Competitor Name] — Battlecard

## Quick Dismiss
[2-3 sentences. Their biggest weakness, our unique strength, or a mix of both. This is the section
that actually gets read on a live call — everything below is support material.]

## Email Template
[A longer written explanation of why we're better — for follow-up in writing, not live.]

## Everything Else
### Product Comparison
[...]
### Strengths & Weaknesses
[...]
### Pricing Information
[...]
```

**Design:** in-house design or a Canva license (upload brand colors, pick a template, don't over-design
— this needs to be scanned in seconds). Crayon/Clue if available: native battlecard filters synced to
the tracked-competitor feed.

**Distribution:** publish wherever the team's collateral already lives (Drive/Dropbox/Box, or a CMS
like Highspot/Seismic/Showpad, or directly in Salesforce) — never a new location. Announce it in an
existing recurring venue (a standing stand-up), 3-5 minutes. Revisit the same team ~4 weeks later with
a visibly improved version, after asking for feedback on how well the quick dismisses actually land.

---

## Newsletter

Source: *Competitive Newsletters for Product & the C-Suite*. Different audience and different depth
than the battlecard — this is where real analysis belongs, not a shallow dismiss.

```markdown
# [Company] Competitive Update — [Month Year]

**Subject line + preview text:** [write this last — preview text drives up to 24% of open decisions]

## Table of Contents
1. [Most important item — one-line teaser, not just a title]
2. [...]

## [Competitor Name]
**[Less-than-10-word subheader summarizing the insight]**

[Body, under ~1000 characters. Passed through the three-question filter before inclusion: how does
this relate to us, is there a bigger story here, what question does it raise — and answer that
question, don't leave it open.]

## Who's Growing
[Headcount-trend signal, from LinkedIn Premium tracking]

## Who Customers/Prospects Are Mentioning
[Community-mention signal, e.g. from Reddit/Quora or Chorus.ai call-mention tracking]
```

**Content types:** M&A activity, funding rounds, partnerships, major product releases, positioning/
messaging shifts. Never paste a press release — the work is in the "so what."

**Tools:** Grammarly (grammar/typos, inline wherever it's drafted), Hemingway (flags long/complex
sentences, adverbs, passive voice), MailChimp (preview text, audience lists, open/click tracking).

**Cadence:** monthly, never skip a month. Announce ahead of time, ask for feedback after.

---

## Win/Loss Survey

Source: *Win/Loss, part 1*. Quantitative — reach and speed, at the cost of depth.

```markdown
## Survey: [Closed-Won / Closed-Lost]

Target length: under 5 minutes, 10 questions or fewer. Anchor to the consideration/decision stages.

1. Which vendors did you consider?
2. How did you evaluate providers?
3. What were [competitor]'s strengths and weaknesses?
4. What was the primary reason behind your final selection?
5. If price wasn't a factor, would your decision have changed?
[+ a segmenting question if a cross-segment pattern matters, e.g. "How many employees does your
company have?"]
```

**Invite email** (under 200 characters, both tracks):
- **Closed-won:** thank them for being a customer, ask to learn from their evaluation process. No
  incentive by default — they're already in good standing.
- **Closed-lost:** thank them for evaluating the company (not for being a customer). Incentive
  explicit and visible — without one, response rate likely won't be high enough to see a pattern.

**Tools:** Google Forms (simple/affordable, no conditional logic); GetFeedback (more customizable).

---

## Win/Loss Interview Guide

Source: *Win/Loss, part 2*. Qualitative — context a survey can't capture.

```markdown
## Interview Guide — [Closed-Won / Closed-Lost]

Reused from the survey questions above, opened up for follow-up. Target 15-20 minutes.
Need at least 10 *related* interviews (matched on industry, product evaluated, or company size)
before trusting a pattern.

Stay alert to what's actually said over what's scripted — ask the off-script follow-up, dig into a
pause or an odd word choice.
```

**Sourcing — two gotchas:**
1. Closed-lost accounts respond at a lower rate — over-invite them, don't just accept a smaller sample.
2. Reach out within ~3 weeks of close — beyond that, recall degrades. Filter by opportunity-closed date.

**Tools:** Zoom's native recorder (pragmatic default) or Chorus.ai (higher transcription accuracy,
cross-call keyword playlists); Calendly for scheduling.

**Reporting — combine with the survey results, answer two questions before presenting anything:**
1. What needs to happen to act on this? (cost, timeline, owner — not just the raw finding)
2. Who needs to see this? (loop in every real stakeholder, not just leadership)

Deliverable: an official slide deck linking to the raw survey spreadsheet + interview data.

---

## Displacement Campaign Plan

Source: *Organizing a Competitive Marketing Campaign*. Proactive — targeting a competitor's own
customer base. Check first whether a campaign already exists; partner with it rather than duplicate it.

```markdown
## Displacement Campaign: [Competitor Name]

**Audience:** [a competitor we have a strong win rate against, whose base we're targeting — OR a
legacy vendor in a market just entered]

**Contact list — build method:**
- Free: CRM opportunity/account notes (if sales reliably fills them in) + LinkedIn engagement on the
  competitor's posts as a customer proxy
- Paid: contact-enrichment tool (e.g. ZoomInfo's Reach extension) to convert LinkedIn engagement into
  real contact info, or filter by "technologies installed" to find accounts actually running the
  competitor's product

**Parallel plays:**
- SEM: bid on the competitor's branded keywords (budget-dependent)
- SEO: landing pages addressing what someone would search to compare the two companies (works
  regardless of budget)
```

Requires real outbound infrastructure and consent/compliance handling — a recommendation to hand to
whoever owns demand gen, not something this skill executes itself.
