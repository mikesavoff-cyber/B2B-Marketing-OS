---
name: account-scoring
description: >-
  Turn an ICP into a 0-100 fit score for every account in the market, tier
  accounts A/B/C/D, match GTM effort and spend to each tier, design "1 message,
  1 audience, 1 offer" plays, and report progress with a Pipeline Weather
  Report and TAM penetration view. Use whenever the task involves "score our
  accounts," "account scoring," "ICP scoring model," "fit score," "tier our
  accounts," "A/B/C/D tiers," "target account list," "ABM tiers," "where
  should we spend," "TAM/SAM mapping," "pipeline weather report," or "TAM
  penetration." Built from Keyplay's ICP modeling workshop in
  `Product Marketing/ICP and Personas/`.
allowed-tools: Read Write Edit Bash WebSearch WebFetch
metadata:
  version: 1.0.0
---

# Account Scoring

"The easiest way to squander marketing budgets is to target the wrong accounts" (Keyplay, *Model and
target a data-driven ICP*). "None of this is a messaging problem. It's a targeting problem."

## The two failure points this solves

From *Model and target a data-driven ICP*:
1. **A vague definition.** PartnerStack's original ICP read as a "standard SaaS ICP": so broad that
   pulling "every single company that fits this description" would mean mostly waste.
2. **The translation gap.** "You can have a really good definition of exactly who your ICP is," and
   still never turn it into the account lists, ad targeting, and outbound lists you actually run.

Method: **Define → Translate → Test → Improve**, run across three parts:
**Account Selection → Account Engagement → Account Measurement**.

## Inputs

- **`icp-definition` output.** Its signal table ("better if..." / "avoid if...") and ICP definition
  sentence are the model's starting point. If it's missing, run the signal map here: best
  customers vs. DQ leads, per `references/methodology.md`.
- **`competitor-research` output.** Technographic fit, such as whether an account uses a competitor
  today, can be a signal.
- **CRM data:** best customers, DQ leads, opportunity stages, and pipeline. Needed to test the model
  and for all of Measurement.
- **The SAM list:** the accounts to score. "Be careful" defining it.

## Process

Full steps and examples: `references/methodology.md`. Templates: `references/templates.md`.

### Part 1 — Account Selection (build and test the model)

1. **Signals.** Start from the signal table. Enrich both lists with:
   - size
   - sub-industry
   - sales motion
   - team structure
   - tech stack
   - growth indicators

   The key is contrast: a trait both best customers and DQ leads share is not a signal.
2. **Weight the signals** into a model that gives every account a 0-100 fit score. "Depending on
   your situation, you'll weigh different models differently." The source doesn't prescribe
   weights. Set them from the signal strength in your own data and state the reasoning.
3. **Use AI for the hard signals.** These are signals databases can't easily see, like "does it
   have an existing partner program" or "rate their level of ABM sophistication on a scale of one
   to ten." AI can read an account's website and score them.
4. **Test.** Run best customers and DQ leads through the model. "What you want to see is that your
   DQ leads are scoring mostly C and D" and top customers score high. If not, re-weight. "If you
   really want to get buy-in... you need to be able to test it."
5. **Score the SAM** and tier it A/B/C/D. The source doesn't give numeric cutoffs. Set them from
   where the test separated best customers from DQ leads, and state them.

### Part 2 — Account Engagement (match effort to tier)

| Tier | GTM effort | Spend |
|---|---|---|
| A | Full activation: 1:1 or 1:few ABM, sales + marketing + partnerships | High CAC, justified by high ACV |
| B | Targeted campaigns, signal-qualified outreach, 1:few or vertical plays | Medium CAC |
| C | Passive only: SEO, inbound, PLG, nurture | No targeted spend |
| D | Inbound only | Zero paid, zero outbound, zero ABM |

- **Fit beats size.** An enterprise account "that score[s] low in your model because they don't have
  a strong business need... we should cut waste by not sending on the Cs."
- **Always-on brand, plus coordinated plays.** Brand runs to the whole market. Plays are
  **1 message, 1 audience, 1 offer**. Thoropass: audience = companies with multiple compliance
  frameworks, message = "Experiencing death by audits?", offer = a next step that solves that pain.
- **Cut waste.** For C and D tiers, list the channels, plays, and reps wasting time, and pause them.
  "This is where ACV alignment typically exposes overspend."

### Part 3 — Account Measurement (report it)

- **Weekly Pipeline Weather Report:**
  - Intro (2-3 sentences)
  - Weather per A and B tier: Sunny (ahead), Cloudy (needs attention), Rainy (at risk)
  - Leading indicators: meetings, engaged accounts, stage moves
  - Lagging indicators: opportunities, pipeline value, closed-won
  - MQLs count only from target accounts
- **TAM penetration view:** accounts per tier, then how many are engaged, qualified, opportunities,
  and closed.
- **Qualitative insights:** accounts broken into, a deal story, emerging risks, wins.
- **Executive slide:** TAM by tier, penetration, pipeline this quarter, the weather snapshot, and one
  line on what improved.

## Output

One file: `competitor-profiles/<company>-account-scoring-<YYYY-MM-DD>.md`, plus
`<company>-scored-accounts-<date>.csv` when a list is actually scored.

1. **The call.** One sentence naming which tier gets the budget and what spend to cut.
2. **Scoring model:** signals, weights with reasoning, tier cutoffs, and the test result.
3. **Tier map:** effort per tier, A and B plays in 1/1/1 form, and C/D waste to cut.
4. **Measurement setup:** the Pipeline Weather Report and TAM penetration templates, ready to fill.
5. **Open questions**, each naming the evidence that would resolve it.
6. **Hands off to:** GTM and demand gen (plays per tier), and the `buyer-personas` roles to target
   inside A accounts.

## Constraints

- **The model isn't trusted until it's tested.** No test against best customers and DQ leads means
  the model is labeled **untested hypothesis**, and no tier drives spend yet.
- **Arm's-length research** (no CRM): you can draft signals from public data and score a sample
  list, but you can't test the model. Measurement is **N/A** and must say so. Never invent pipeline
  numbers.
- Weights and tier cutoffs are this skill's judgment (source class 3). State them as such. The
  source doesn't prescribe them.
- Keyplay's case results (Hone 2.3x ACV, PartnerStack -34% cost per pipeline dollar and +58%
  pipeline value, Airbase 90% outbound lift) are the vendor's own claims (source class 2). Never
  cite them as independent proof.
- One message, one audience, one offer per play. Never a play aimed at "all A accounts" with three
  messages.

## Grounding

`Product Marketing/ICP and Personas/`: *Model and target a data-driven ICP with AI.md* (the workshop
transcript, primary) and *Workbook_ ICP modeling with AI.md* (the exercises).

## Related skills

- `competitor-research`: technographic signals, including which accounts use a competitor.
- `icp-definition`: runs first. Supplies the signal table and ICP definition.
- `market-segmentation`: firmographic and technographic attributes to score on.
- `buyer-personas`: the roles to reach inside A-tier accounts.
