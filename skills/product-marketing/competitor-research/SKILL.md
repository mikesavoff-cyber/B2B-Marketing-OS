---
name: competitor-research
description: >-
  Research one named competitor in depth — positioning, product strengths/weaknesses,
  market sentiment, growth trajectory, paid/organic marketing activity, and AI-answer
  visibility. Use when the task is "research [competitor name]," refreshing stale
  intel on one already-tracked competitor, or adding a competitor to a tracked set
  mid-cycle. Produces a structured per-competitor profile. Does not identify which
  competitors to track (that's `market-competitive-intel-research.md` Step 1) and
  does not write the comparative brief or battlecard (that's the same workflow's
  Steps 3 and 5) — this skill's job is the research on one company, nothing else.
---

# Competitor Research

## When to use this skill

- "Research [company]" as a competitor
- Refreshing research on a competitor already being tracked, outside the weekly-refresh cadence
- A new competitor needs adding mid-cycle (per the expansion trigger: it started appearing in lost-deal data or AI-answer citations)
- Called once per competitor by `market-competitive-intel-research.md` Step 2 — this skill is the thing that step invokes, not a duplicate of it

This skill does **not** decide who to research (Step 1's job), does not compare competitors against each other or against the target (Step 3's job), and does not build a battlecard (Step 5's job). It produces one input those steps consume.

## Required input

Company name, and its confirmed tier (1, 2, or 3) from `market-competitive-intel-research.md` Step 1 — tier controls how much of this skill actually runs. If no tier was given, ask rather than assume Tier 1 depth.

## Step 1 — Tier check

- **Tier 1:** run everything below.
- **Tier 2/3:** run the Marketing lane's mandatory items only (homepage, pricing, Customers/Case Studies) plus the Leadership lane's core items (funding/headcount/status). Skip paid ads, social performance, SEO intelligence, AI-answer visibility, and the blog/changelog pass unless something specific about this competitor gets flagged as worth the extra depth.

## Step 2 — Marketing lane

Fetch live, in this order, never from memory:

1. **Homepage** — positioning/hero language. State the lead positioning angle in exactly one sentence before moving on; if it takes more than one sentence, the positioning hasn't actually been distilled yet.
2. **Pricing page** — tiers, packaging, GTM model inference (sales-led: gated pricing, "Book a Demo" as primary CTA, no self-serve / product-led: visible pricing, self-serve signup, free trial — state which, or hybrid).
3. **Main Product/Platform/Solutions pages** — top-level only, not every feature sub-page.
4. **Customers / Case Studies / Proof / Results — mandatory regardless of tier.** This is where proof of value actually lives, essentially never on the homepage. A competitor's evidence does not get marked "doesn't exist" until this page specifically has been fetched and read. (This requirement exists because an earlier run of this research skipped it and produced a false "no proof" claim — see the parent workflow's standing rules for the full incident.)
5. **Tier 1 only — blog/resources index page.** Title, date, and first paragraph of each recent post — not the full post. Enough to catch a positioning shift or a case-study-shaped post without paying to read every entry in full.
6. **Tier 1 only — changelog/release notes**, if one exists. A shipped feature can directly age out a claim already sitting in this competitor's battlecard.
7. **Tier 1 only — paid search/ad activity and ad copy**, if a tool with this data is available (e.g. Semrush Advertising Research). Note plainly when this isn't reachable rather than guessing at ad spend or messaging.
8. **Tier 1 only — the competitor's own social media presence.** Follower counts, engagement rate, and top-performing content topics/formats, via a tool if available or a direct check of their profiles if not.
9. **Tier 1 only — keyword/SEO/topic intelligence.** What terms they're targeting, ranking-change direction if visible, content-gap signal.
10. **AI-answer visibility** (all tiers, cheap to check): does this competitor show up when an LLM is asked a relevant category question? Note presence/absence and, if present, how they're framed.
11. **G2 / TrustRadius / Trustpilot / Glassdoor** — pull via web search when direct site access is blocked. Sort by recency where the source allows it; a two-year-old review carries less weight than last month's. Capture both praise and complaints, not just the star rating.
12. **Community check** — Reddit, Quora, LinkedIn (posts/discussion, not the company page), Facebook groups, Discord, Slack. Run all of them. An empty result across all of them is itself a real, reportable finding — never skip a source silently or invent chatter that isn't there.

## Step 3 — Product lane

1. Knowledge base / docs / developer portal — feature depth, how it actually works.
2. G2/TrustRadius filtered specifically to feature-level feedback, not general sentiment.
3. A one-time news search as a Google-Alerts substitute (this skill can't configure a live ongoing alert) — say so plainly if the output is later treated as if it were live monitoring.

## Step 4 — Leadership lane

1. Funding, headcount, and status via Crunchbase/PitchBook/Tracxn/press — explicitly a substitute for LinkedIn Premium's Insights tab, which this skill doesn't have access to. Say so.
2. **Jobs page** — what roles they're actively hiring for. Reveals strategic priorities and expansion areas, and postings sometimes name competitors directly ("experience competing against X").
3. Funding rounds, layoffs, acquisitions, executive hires, lawsuits, and **partnership announcements** — check for all of these as distinct event types, not just funding/layoffs.
4. When sources disagree on a hard number (funding total, headcount), report both and flag the discrepancy. Never silently pick one.
5. Check specifically for the two status-changing outcomes: acquired (no longer an independent buying decision) and material distress (large layoff independently reported as business weakness, or a long funding drought) — both outrank any star rating as findings.

## Output

One structured profile per competitor:

- **Positioning** (one-sentence lead angle) + GTM model
- **Buyer** (who they sell to)
- **Market read** (review sentiment, community presence, AI-answer visibility)
- **Product strengths/weaknesses** (feature-level, sourced)
- **Trajectory** (growing / fading / acquired, with the evidence)
- **Marketing activity** (paid, social, SEO — Tier 1 only)
- **Source list** for every claim above

This profile is the input to the parent workflow's Step 3 (comparative synthesis) — it does not itself take a stance on how this competitor compares to the target or to others; that judgment happens one level up, once every tracked competitor's profile exists.

## Constraints

- Never state a fact about this company from memory. Verify live or say "unknown."
- Never conclude "no proof exists" without having actually fetched the Customers/Case Studies page.
- Never treat a tool's absence (no Semrush access, no LinkedIn Premium) as a reason to guess — state the substitute used and the gap plainly instead.

## Related skills

- `market-competitive-intel-research` (workflow) — the orchestrator that invokes this skill once per confirmed competitor, then synthesizes the resulting profiles into a comparative brief. Run that first if the competitor set isn't confirmed yet.
- `pmm-segmentation-icp` — for researching the target's own buyers/customers in depth. This skill's Product/Marketing lanes touch on a competitor's buyer at a surface level only; deep buyer research belongs to that skill, not here.
