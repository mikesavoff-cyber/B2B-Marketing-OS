# Tool Reference for Competitive Intelligence

Every tool named in `Product Marketing/Competitive Intel/`, organized by tier. This file replaces any
generic tool-mapping — if a named tool isn't available in a given session, say so plainly and use the
next-best resource in the same tier; don't guess at data a missing tool would have provided.

## Contents
- Tier 1: Free & Affordable Tools
- Page Checklist
- Tier 2: Paid & Enterprise Tools
- Win/Loss Tools
- Content & Distribution Tools
- Displacement Campaign Tools
- Recommended Sequences
- Named Gotchas

---

## Tier 1: Free & Affordable Tools

Source: *Gathering Insights: Startups & Mid-Market*.

- **Company homepage** — read positioning/messaging directly. No filters needed, just the page itself.
- **G2 / TrustRadius** — "Yelp for B2B software." Filter to 1-3 star reviews, search by keyword, sort
  by most recent. Also filterable by company size, user role, category, industry, region.
- **Social communities** (Reddit, Quora, Facebook groups, Discord, Slack) — search `[competitor name]
  reddit` (or the relevant platform) directly. No incentive bias, unlike review sites.
- **Competitor's own customer knowledge center** — FAQs, UI screenshots, walkthroughs (product-lane
  research, not homepage).
- **Google Alerts** — free, keyword-based. Try a few keyword combinations (e.g. `[competitor] CRM`,
  `[competitor] press release`). Customize frequency, source, language, region, delivery email under
  "Show Options."
- **LinkedIn Premium — Insights tab** — employee headcount trend over ~18 months, as a revenue-health
  proxy for privately held competitors.

*Not from the course. Imported from `competitor-profiling` or added after the Skillvue run, 2026-09-23:*
- **Sitemap + robots.txt** — free site map. Read `/robots.txt` for `Sitemap:` lines, else try
  `/sitemap.xml` and `/sitemap_index.xml`; follow nested sitemaps. Save the URL list to
  `scrapes/_sitemap-urls.txt`. Page counts per section (blog, resources, "vs" pages) are the Tier 1
  stand-in for search footprint.
- **Capterra** — third review source after G2 and TrustRadius. Also used in the findability check:
  search the company name and note name collisions.
- **Company help centers** — the public help center or support site (often `help.`, `support.`, or a
  Zendesk domain). Some are candidate-only; say so rather than treating that as the customer knowledge
  base.

---

## Page Checklist

*Imported from `competitor-profiling` Phase 1; added after the Skillvue run, 2026-09-23.* Map the site
first (sitemap above), then read these pages. Mark each "checked" or "not found" in the profile's Raw
Data Sources.

| Page | Answers which audience question | Why |
|---|---|---|
| Homepage | Perceived | Positioning, headline claims |
| Pricing | Perceived + used | Tiers, packaging, billing model |
| Product / solutions pages | Used | What it actually covers; required before claiming a competitor lacks X |
| Integrations page | Used | What it plugs into |
| Customers / case studies | Perceived | Where proof lives; homepages rarely carry it |
| Help center / knowledge base | Used | How it really works: billing, setup, validation, limits |
| About / company | Trending | Founding, team, offices, funding |
| Press / news page | Trending | Launches, partnerships, rounds |
| Blog index + changelog | Trending | Content cadence and product direction |

## Tier 2: Paid & Enterprise Tools

Source: *Gathering Insights: Enterprise*. Use once Tier 1 is proven out or budget allows.

- **Crayon / Clue** — aggregates a competitor's full digital footprint (Reddit/Quora mentions, social,
  site changes, content, news/PR, reviews) into one filterable feed; alerts to inbox or Slack; native
  battlecard filters.
- **Chorus.ai** — conversation intelligence. Tracks/analyzes sales calls and emails, flags competitor
  mentions, builds keyword playlists across calls. Reveals how often sellers actually face a
  competitor and how they currently pitch against them.
- **SEMrush** — competitor website traffic, traffic source, estimated market size. Owned primarily by
  SEO/SEM teams — partner with them.
- **Analyst relations (Forrester, Gartner)** — paid access to industry reports and 1:1 analyst
  inquiries.
- **Network consultants (GLG)** — anonymous consultations with a target competitor's former executives.

## Win/Loss Tools

Source: *Win/Loss, parts 1-2*.

- **Google Forms** — simple/affordable survey tool; lacks conditional logic and design flexibility.
- **GetFeedback** — more customizable survey tool, when Google Forms' limits are a real constraint.
- **Zoom's native call recorder** — pragmatic default for interviews, especially if the org already
  uses Zoom.
- **Chorus.ai** (also listed under Tier 2) — highest transcription accuracy for interviews; keyword
  playlists across a batch of interviews (e.g. every mention of "expensive" across closed-lost calls).
- **Calendly** — scheduling, removes the back-and-forth of finding a mutual time.

## Content & Distribution Tools

Source: *Building Battlecards*, *Competitive Newsletters*.

- **Canva** — battlecard design; upload brand colors, use a template, don't over-design.
- **Crayon / Clue** (also Tier 2) — native battlecard filters synced to the tracked-competitor feed.
- **Drive, Dropbox, Box** — simple collateral storage.
- **Highspot, Seismic, Showpad** — content management platforms for sales/marketing collateral.
- **Salesforce** — some teams push collateral directly here.
- **Grammarly** — free Chrome extension, catches typos/grammar, works in any browser-based editor.
- **Hemingway** — flags overly long/complex sentences, adverbs, passive voice.
- **MailChimp** — newsletter writing/distribution: preview text, audience list management, open/click
  tracking.

## Displacement Campaign Tools

Source: *Organizing a Competitive Marketing Campaign*.

- **CRM** — opportunity/account notes, if sales reliably fills them in.
- **LinkedIn** — engagement on a competitor's posts as a customer-list proxy.
- **ZoomInfo** ("Reach" Chrome extension) — pulls contact/account info from a LinkedIn search, profile,
  CRM, or corporate website; can filter by "technologies installed" (32,000+ tracked) to find accounts
  actually running a competitor's product.
- **A named lower-cost alternative to ZoomInfo** — has a similar Chrome-extension flow but no
  technologies-installed filter. (The instructor's exact name for this tool is garbled/unclear in the
  transcript — don't guess a specific product name; note that a cheaper alternative exists and verify
  the actual name before recommending one.)
- **SEM/SEO teams** — branded-keyword bidding; comparison-intent landing pages.

---

## Recommended Sequences

### Standing up Tier 1 research (default, per competitor)
```
0. Baseline → if researching for a named company, run steps 1-8 on it first
1. Sitemap → map the site, save _sitemap-urls.txt, note page counts per section
2. Page checklist → read the pages for each audience question (Page Checklist above)
3. G2/TrustRadius → filter 1-3 star, keyword search, sort recent; record the newest review's date
   (if blocked: TrustRadius → Capterra; never solve a CAPTCHA; ask the user if critical)
4. Findability → review-site presence + category per site, name collisions, "vs" page count
5. Social communities → search "[competitor] reddit" or equivalent
6. Competitor's own knowledge center → product-lane detail
7. News → funding, M&A, launches; subscribe: Google Alerts on 2-3 keyword combinations
8. LinkedIn Premium Insights (if available) → headcount trend
```

### Upgrading to Tier 2 (once proven out / budget allows)
```
1. Set up Crayon or Clue → one aggregated feed, replaces manual per-source checking
2. Connect Chorus.ai (or equivalent) → track live sales-call mentions
3. Pull SEMrush traffic/market-size data
4. Establish analyst relations / GLG only for specific deep questions, not routine tracking
```

### Standing up the full program (Build Order, from *Pushing "Go"*)
```
1. Insight cataloging log (spreadsheet)
2. Battlecards + newsletter, for the capped 5 tracked competitors
3. Win/loss program, scoped only to deals against those 5
4. Proactive displacement campaigns
```

---

## Named Gotchas

| Issue | What the source says to do |
|---|---|
| Review-site ratings can be incentivized (gift-card-for-review campaigns) | Still use G2/TrustRadius — just expect some minimalist low-signal reviews mixed in |
| Google Alerts overwhelms past ~10 tracked competitors | Move to Crayon/Clue instead of adding more alerts |
| Sales team doesn't reliably fill in CRM competitor notes | Don't rely on CRM data alone for displacement-campaign lists — use LinkedIn engagement as a fallback |
| Closed-lost accounts respond to win/loss outreach at a lower rate | Over-invite closed-lost accounts — send more invites than there are interview slots |
| Interview timing too far past deal close | Reach out within ~3 weeks; beyond that, recall degrades — filter by opportunity-closed date |
| Newsletter item runs long | Cap at under 1000 characters — length intimidates the reader and hides the "so what" |
| Battlecard overloaded with detail | Quick dismiss (2-3 sentences) goes first — that's what 95% of readers actually want |

*Added after the Skillvue run, 2026-09-23 (not from the course):*

| Issue | What to do |
|---|---|
| Review site shows a CAPTCHA / "verification required" mid-run | Don't solve it. Save a "blocked" note, fall back G2 → TrustRadius → Capterra, ask the user to pass the check if the source is critical |
| Reddit blocks scrapers and API calls | Save search-result snippets labeled as leads, not read threads; say the threads weren't opened |
| Review base is stale (e.g. HireVue on TrustRadius: newest review Dec 2023) | Cite the newest review's date next to every rating; flag it as stale if more than 12 months old |
| Sitemap `lastmod` dates look uniform (e.g. TestGorilla regenerates daily) | Don't read them as publishing cadence; use page counts instead |
| Obvious domain is parked or wrong (e.g. talentware.com vs talentware.ai) | Confirm the real domain via search before scraping; record the wrong one as a finding |
