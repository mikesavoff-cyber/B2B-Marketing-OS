# Battlecard Weekly Refresh (automated)

Purpose: keep battlecards for the tracked competitor set current, on a recurring schedule, without a human re-running the full research skill (`skills/product-marketing/competitor-research/SKILL.md`) from scratch each time.

This is a separate, downstream workflow. It does not identify new competitors, does not replace the human-confirmed tracked list, and does not run unattended without ever surfacing findings to a human — it's a diff-and-alert process, not a silent auto-editor.

**Input:** the confirmed competitor list and the current battlecard set from the parent workflow. This workflow starts only after that one has produced at least one real battlecard set — it has nothing to refresh otherwise.

**Cadence is two-speed, to keep this affordable — depth follows tier, not a flat schedule:**
- **Weekly (all competitors, every tier):** the cheap pass only — Step 1a's new-page detection (sitemap/nav diff) plus a lightweight check for anything already flagged as likely-changed. This is a signal scan, not a full re-read.
- **Monthly (Tier 1 only):** the full bounded-checklist deep pass — Step 1b in full, every page category, same depth as the parent workflow's original Step 2 research.
- **Quarterly (Tier 2/3):** the same full deep pass, just less often, since they're lower-priority by definition.
- Immediate items (per the parent workflow's Step 4 definition — acquisitions, funding rounds, major product releases, lawsuits, large layoffs reported as distress) still get surfaced the moment they're found, regardless of tier or which cadence is currently due — this schedule is a floor, never a reason to hold major news.

**Monthly focus competitor:** each run carries a designated focus competitor for the current month — typically whichever of the five has the lowest current win rate, or the most consequential recent status change — set by a human, not chosen by this workflow. The focus doesn't change what gets checked (all five still get the full Step 1 pass every week), but it does change what gets emphasized in the run log and in that period's newsletter lead story, and it's the competitor whose win rate should actually be tracked before and after the month's push. Without a named focus, a month's activity can't be cleanly attributed to a result — this designation is what makes the whole refresh cycle measurable rather than just busy.

## Step 1: Re-check each competitor's online presence

This is the actual purpose of the whole workflow, stated plainly: track every move a competitor makes on their own website, not just a handful of named pages. Positioning changes, new product pages, new landing pages, new blog/resource content, new case studies, pricing page changes, and feature releases/changelog entries are all in scope — each one is a real signal about what the competitor is doing, and each one gets missed entirely by a check that only revisits the same few pages every week.

**1a. Detect new pages, not just changes to known ones.** Before diffing anything, check whether the site's structure itself has grown: pull the sitemap.xml if one exists, or re-walk the nav/footer, and compare the URL list against what was captured last run. A brand-new landing page, product page, or case study won't show up in a diff of already-known pages — it has to be noticed as a new URL first. This step is what actually catches "new landing page" and "new product page" as change types; skipping it means the check only ever sees updates to pages it already knew about.

**1b. On the monthly (Tier 1) or quarterly (Tier 2/3) deep-pass run only — re-fetch and diff every page in scope, category by category:**
- **Homepage** — positioning/hero language drift.
- **Product/platform pages** — new capabilities, reworded claims, new pages covering a use case that didn't have one before.
- **Pricing page** — tier changes, new packaging, a price that moved. Pricing changes are strategically significant on their own and should never get folded silently into a generic "product update" line.
- **Customers / Case Studies / Proof / Results** — new logos, new named case studies, new quantified claims. This is the category that caused the original miss in the parent workflow; it does not get treated as lower-priority than the others here.
- **Blog / Resources / content hub** — new posts, especially anything naming a competitor (including the target), a category claim, or a customer story that didn't get its own dedicated case-study page.
- **Changelog / release notes / "what's new"** — new feature releases. A shipped feature can directly age out a claim already sitting in that competitor's battlecard ("they don't have X" stops being true the day they ship X), so this page matters as much as any review site.
- **Landing pages** discovered via 1a — treat as their own category; a new landing page targeting a specific segment or use case is itself a positioning/GTM signal, not just content.

**1c. Off-site sources, same as before:**
- G2 / TrustRadius / Trustpilot / Glassdoor — check for new reviews or rating shifts since last check.
- Community (Reddit, Quora, LinkedIn, Facebook groups, Discord, Slack) — check for new mentions.
- Funding/news/leadership signal (Crunchbase, PitchBook, Tracxn, press) — check for new events: funding rounds, layoffs, acquisitions, executive hires, lawsuits.
- SEMrush / Gartner Peer Insights, if account access allows — check for material traffic or rating shifts.

Do not re-run Step 0 (homepage positioning) or Step 1 (competitor identification) — those are one-time, not part of this recurring check, unless a competitor's fundamental status changes (e.g. gets acquired by another company — see Step 3 below).

## Step 2: Classify what changed

For each new finding, classify it the same way the parent workflow's Step 4 does, plus the change-type category from Step 1:

| Company | Change Type | Insight | For Team | Channel | Cadence |
|---|---|---|---|---|---|

Change Type is one of: Positioning, New Product Page, New Landing Page, New Content, New Case Study, Pricing Change, Feature/Changelog Release, Review/Rating Shift, Community Mention, Funding/Leadership Event. This category is what lets the run log and the newsletter actually say what kind of move a competitor made, not just that something changed.

Only genuinely new information goes in this table — re-confirming an unchanged fact is not a finding.

## Step 3: Flag status-changing events specifically

Some events don't just update a battlecard, they invalidate its current form — check for these explicitly every run:

- **Acquired** — the competitor is no longer an independent buying decision. Flag for a human decision: retire the card, or replace it with the acquiring company.
- **Major distress** — a large layoff independently reported as business weakness, or a funding drought long enough to be notable. Update the card's trajectory read, don't just append a line.
- **New legal/regulatory action** — flag immediately, regardless of the weekly cadence.

## Step 4: Update the affected battlecard(s)

For any competitor with a genuine new finding, regenerate that specific battlecard's story arc (parent workflow Step 5) using the updated facts — don't hand-patch one line of an old arc if the new fact changes which beat it belongs in (e.g. a new lawsuit usually becomes the new climax, not an addendum to the old one).

The change type from Step 2 shapes what actually needs updating, not just whether something does:
- **Feature/Changelog Release** — check whether it directly ages out an existing claim in the card (a stated weakness that's now fixed, a gap that's now closed). This is the change type most likely to make an existing arc actively wrong, not just stale, and gets priority over the others.
- **Pricing Change** — update any pricing-related line in the card; flag for the newsletter even if the battlecard itself doesn't otherwise need regenerating.
- **New Case Study / New Content** — check whether it undercuts a "no proof" or "thin proof" claim already sitting in the card; if so, that claim has to go, not just get a caveat added next to it.
- **New Product Page / New Landing Page** — signals a new segment or use case being targeted; note it even if it doesn't change the card's core arc, since it's relevant to whether this competitor is entering the target's own segment.
- **Positioning** — re-run the diff against Step 0's original read for that competitor; if the shift is significant, treat it the same as a status-changing event even though it isn't on the Step 3 list below.

Cards with no new findings that week are left untouched — don't regenerate a card just because the schedule fired.

## Step 5: Report the run, every time

Every run — even one with no changes — produces a short run log:

- Which competitors were checked.
- What changed, if anything (link to the Step 2 table for that run).
- Which cards were regenerated, if any.
- Any status-changing flags from Step 3, surfaced explicitly for a human decision — never auto-resolved.
- This month's focus competitor, and the current win-rate read against them if that data exists — the one number this whole cycle should be moving.

Publish the run log and any updated cards to the same Notion location as the parent workflow's output. Never let a scheduled run silently pass with no visible record.

## Standing rules — same as the parent workflow, restated because this runs unattended

- Never state a company or product fact from memory. Verify live on every run, even for a competitor checked last week.
- Never judge a competitor's proof or capabilities from its homepage alone. The weekly run is a cheap signal scan by design (Step 1a) — the full bounded-checklist deep pass (Step 1b, including Customers/Case Studies) runs monthly for Tier 1 and quarterly for Tier 2/3, not every week. Don't skip the deep pass entirely just because the weekly scan found nothing; the two run on different schedules for cost reasons, not because the deep pass is optional.
- Never auto-retire or auto-replace a competitor on the list (Step 3) — flag it, let a human confirm.
- Never regenerate a card without a genuine new finding behind it.
- If a source that worked last run fails this run (blocked, rate-limited, account issue), report that explicitly in the run log — don't silently skip it or fill the gap from memory.
