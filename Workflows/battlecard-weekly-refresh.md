# Battlecard Weekly Refresh (automated)

Purpose: keep the battlecards produced by `market-competitive-intel-research.md` (Step 5) current, on a recurring schedule, without a human re-running the whole research workflow from scratch each time.

This is a separate, downstream workflow. It does not identify new competitors, does not replace Step 1's human-confirmed competitor list, and does not run unattended without ever surfacing findings to a human — it's a diff-and-alert process, not a silent auto-editor.

**Input:** the confirmed competitor list and the current battlecard set from the parent workflow. This workflow starts only after that one has produced at least one real battlecard set — it has nothing to refresh otherwise.

**Cadence:** weekly, by default. Immediate items (per the parent workflow's Step 4 definition — acquisitions, funding rounds, major product releases, lawsuits, large layoffs reported as distress) still get surfaced the moment they're found, same as the parent workflow — this schedule is the floor, not a reason to hold major news for the next weekly run.

**Monthly focus competitor:** each run carries a designated focus competitor for the current month — typically whichever of the five has the lowest current win rate, or the most consequential recent status change — set by a human, not chosen by this workflow. The focus doesn't change what gets checked (all five still get the full Step 1 pass every week), but it does change what gets emphasized in the run log and in that period's newsletter lead story, and it's the competitor whose win rate should actually be tracked before and after the month's push. Without a named focus, a month's activity can't be cleanly attributed to a result — this designation is what makes the whole refresh cycle measurable rather than just busy.

## Step 1: Re-check each competitor's online presence

For each competitor already on the confirmed list, re-run the same sources Step 2 of the parent workflow used, scoped to what's changed since the last run:

- Homepage — re-fetch live; diff against the last captured hero/positioning text.
- G2 / TrustRadius / Trustpilot / Glassdoor — check for new reviews or rating shifts since last check.
- Community (Reddit, Quora, LinkedIn, Facebook groups, Discord, Slack) — check for new mentions.
- Funding/news/leadership signal (Crunchbase, PitchBook, Tracxn, press) — check for new events: funding rounds, layoffs, acquisitions, executive hires, lawsuits.
- SEMrush / Gartner Peer Insights, if account access allows — check for material traffic or rating shifts.

Do not re-run Step 0 (homepage positioning) or Step 1 (competitor identification) — those are one-time, not part of this recurring check, unless a competitor's fundamental status changes (e.g. gets acquired by another company — see Step 3 below).

## Step 2: Classify what changed

For each new finding, classify it the same way the parent workflow's Step 4 does:

| Company | Insight | For Team | Channel | Cadence |
|---|---|---|---|---|

Only genuinely new information goes in this table — re-confirming an unchanged fact is not a finding.

## Step 3: Flag status-changing events specifically

Some events don't just update a battlecard, they invalidate its current form — check for these explicitly every run:

- **Acquired** — the competitor is no longer an independent buying decision. Flag for a human decision: retire the card, or replace it with the acquiring company.
- **Major distress** — a large layoff independently reported as business weakness, or a funding drought long enough to be notable. Update the card's trajectory read, don't just append a line.
- **New legal/regulatory action** — flag immediately, regardless of the weekly cadence.

## Step 4: Update the affected battlecard(s)

For any competitor with a genuine new finding, regenerate that specific battlecard's story arc (parent workflow Step 5) using the updated facts — don't hand-patch one line of an old arc if the new fact changes which beat it belongs in (e.g. a new lawsuit usually becomes the new climax, not an addendum to the old one).

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
- Never auto-retire or auto-replace a competitor on the list (Step 3) — flag it, let a human confirm.
- Never regenerate a card without a genuine new finding behind it.
- If a source that worked last run fails this run (blocked, rate-limited, account issue), report that explicitly in the run log — don't silently skip it or fill the gap from memory.
