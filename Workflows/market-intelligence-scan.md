# Market Intelligence Scan

Purpose: track the industry/category level, not any named competitor. This is a different job from `market-competitive-intel-research.md` — that file answers "what are these five companies doing," this one answers "what's happening in the category itself" (regulation, funding climate, category-wide narrative shifts). Genuinely separate, feeds the same brief, doesn't replace or duplicate the competitor-specific work.

**Why this exists as its own file rather than a step inside the competitor workflow:** a question like "what's happening in the AI-hiring-assessment category broadly" is a valid, standalone thing to ask, independent of any specific competitor list — bolting it onto a competitor-named file would blur two different jobs.

## The "subscribe to publications" problem, and how it's actually solved here

The source guidance behind this file says to subscribe to industry publications for ongoing coverage. This skill can't literally hold a subscription or receive a live feed — there's no persistent inbox here. The real substitute:

1. **Build a fixed, named watchlist once, confirmed by a human** — not "whatever search turns up this time." For the target's category, identify 3-5 real, specific, ongoing sources: trade publications, category-specific newsletters, and the relevant analyst firms (Gartner, Forrester, IDC, or category-specific equivalents). Name them explicitly and keep the list stable across cycles — this is what makes it comparable to a subscription rather than a fresh unbounded search every time.
2. **"Subscribing" becomes a scoped, repeatable search against that named watchlist**, run on this file's cadence — e.g. `site:[publication domain]` search plus checking the publication's own latest-articles/archive page directly, not a generic category search. A generic search re-discovers different results each time and isn't comparable across cycles; a scoped search against a fixed list is.
3. **State the watchlist explicitly in every output** — which sources were actually checked this cycle — so a gap (a publication whose site is unreachable, or that published nothing new) is visible rather than silently absorbed into "no findings."

## Step 1 — Build or confirm the watchlist

If no watchlist exists yet for this category: search for the real trade publications, newsletters, and analyst firms that actually cover it, propose 3-5, and get human confirmation before treating it as the standing list. If a watchlist already exists, use it as-is; don't rebuild it each cycle.

## Step 2 — Scoped scan, one source at a time

For each watchlisted source: check its latest content (archive/latest-articles page, or a `site:`-scoped search) for anything published since the last scan. Capture: headline, date, one-sentence summary, and why it matters to the target's category — not the full article.

## Step 3 — Structured lenses (apply only when doing a fuller quarterly pass, not every scan)

- **PESTLE** — Political, Economic, Social, Technological, Legal, Environmental factors relevant to the category. Most B2B software categories will only have live signal in 2-3 of these; don't force all six every time.
- **Porter's Five Forces** — competitive rivalry, threat of new entrants, supplier power, buyer power, threat of substitutes. Useful specifically for the Market Context section of the comparative brief; skip for a routine monthly scan.

## Step 4 — Output

A short market-intelligence note: watchlist sources actually checked this cycle, what's new, why it matters to the target's category, and — if anything found here changes how a specific tracked competitor should be read — a flag back to that competitor's profile (produced by the `competitor-research` skill) rather than duplicating the finding in two places.

## Cadence

Monthly by default — same rhythm as the competitor-specific newsletter, but run and reported separately, since it's a different question. A full PESTLE/Five Forces pass (Step 3) runs quarterly, alongside whatever quarterly competitor deep-passes are already scheduled.

## Constraints

- Never state an industry trend or regulatory fact from memory. Verify against the actual watchlist source, or say "unknown."
- Never expand the watchlist without human confirmation — an unconfirmed source added silently breaks the cycle-to-cycle comparability this whole approach depends on.
- Report a source that returned nothing new as "checked, nothing new," not silently omitted — the difference between "we checked and found nothing" and "we didn't check" has to stay visible.

## Related

- `market-competitive-intel-research.md` — the competitor-specific workflow this feeds. Findings here that bear on a specific tracked competitor get flagged there, not duplicated.
- `skills/product-marketing/competitor-research/SKILL.md` — the per-company research unit this file is explicitly *not* a substitute for.
