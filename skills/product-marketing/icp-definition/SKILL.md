---
name: icp-definition
description: >-
  Define and prove a company's ideal customer profile (ICP): which segments to
  target, how proven each one is, what energy state they are in, whether they
  fit a product-led motion, and who buys. Use whenever the task involves
  "define our ICP," "ideal customer profile," "who should we target," "which
  segment first," "is this our ICP," "ICP for [company]," "M1 M2 M3,"
  "MOAT," "PLG fit," "who is the buyer," or "prioritize our segments."
  Produces an ICP priority map plus one ICP profile per prioritized segment.
  Feeds buyer-personas, account-scoring, positioning, and messaging. Built from
  `Product Marketing/ICP and Personas/` and the Buyer Personas lesson.
allowed-tools: Read Write Edit Bash WebSearch WebFetch
metadata:
  version: 1.0.0
---

# ICP Definition

"A broad ICP is worse than no ICP. 'B2B startups' or 'mid-market companies' aren't ICPs — they're
industries. If a segment definition can't be tested and falsified, it's not doing any work"
(*ICP Definition Builder*).

The ICP is "who you deliver the most real business value to... it's not always who closes fastest
or who might be the cheapest to get, but it's who you deliver the most value to" (Keyplay, *Model
and target a data-driven ICP*).

## Inputs

- **Company name and URL.** Required.
- **`competitor-research` final output** (`competitor-profiles/<company>-competitive-research-<date>.md`).
  Needed for Step 2 (who M3 buyers use today) and the Competitive framing field in the profile.
  If it's missing, say so and mark M3 and competitive fields "not yet researched."
- **`market-segmentation` output**, if one exists. Its segments are the candidates this skill
  proves and prioritizes.
- **Customer data**, if available: best customers, disqualified (DQ) leads, retention, usage,
  NPS/PMF survey results. Without it, every segment stays **Hypothesis** (Constraints).

## ICP vs. persona: keep them separate

- **ICP** = the company or team: "Firmographics, size, stage, what they believe, what they're trying
  to do."
- **Persona** = the individual: "job title, day-to-day motivations, what they personally need."

"A team can be squarely in the ICP while containing three different personas with three different
messages" (*ICP Definition Builder*). This skill defines the ICP and maps the buying roles.
`buyer-personas` builds the people.

## Process: five steps, run in order

Full rules, tables, and examples for every step: `references/frameworks.md`.

### Step 0 — Validate with data (the ground-truth layer)

Run it first, and re-run it any time a segment moves up or down in maturity.
- **Signal map.** Compare 10-20 best customers against 10-20 DQ leads. "Do *not* use churned
  accounts, they still bought, so the signal is muddy" (Keyplay *Workbook*). Traits common to best
  customers become "better if..." signals. Traits common to DQ leads become "avoid if..." signals.
- **The data signals that confirm a segment.** It retains better, uses the product more, scores
  higher on NPS/PMF, and closes faster than the rest of the base. "If a segment looks right on
  paper but doesn't show up in these signals, the segment is wrong — not the data."
- **Real enthusiasm vs. polite indifference.** "Founders get lied to gently." Signal lists are in
  `references/frameworks.md`.
- **Confidence.** 0-4 matching paying customers = Hypothesis. 5-9 = Signal. 10+ = Confirmed.
  "Don't promote on vibes."

### Step 1 — Define segments and their maturity (MKT1)

- **Segment = Role + Company Type**, specific enough to build a target list from.
- **Maturity** (evidence, not aspiration):
  - Core: PMF proven
  - Scaling: actively expanding
  - Testing: early signal
  - Future: intentionally deprioritized
- **Rules:**
  - Most companies have 1-2 Core segments.
  - No Future segment means something is missing.
  - Segments with the same buyer, sales cycle, and messaging are one segment.
- **Time allocation today.** Record the actual share of marketing time per segment. Call out any
  mismatch with maturity directly.

### Step 2 — Classify the energy state (M1 / M2 / M3)

Primary source: *"You're building your ICP wrong."* "Instead of starting with firmographic
attributes, start with energy... the activities, behaviors, and unmet desires."
- **M1, potential energy:** the desire exists but they're doing nothing about it. Remove the barrier.
- **M2, kinetic energy:** already doing it, but in a worse way. Redirect the energy.
- **M3, captured energy:** already using a competitor. Steal share. Pull the competitors from
  `competitor-research`.

"A good message aimed at the wrong group becomes a bad message." Prioritize one M group:
"devote 60 to 80% of the GTM budget to it." Layer firmographics on *after* the M group is chosen.

### Step 3 — Score PLG fit (MOAT)

Primary source: `Product Marketing/ICP and Personas/Wes Bush - MOAT PLG Fit (Product-Led Growth 2nd ed).md`.
Flag each dimension Green, Yellow, or Red:
- **Market strategy:** SMB or mid-market = Green. Mid-market with significant enterprise = Yellow.
  Pure enterprise = Red.
- **Ocean conditions:** red ocean = Green. Blue ocean = Yellow. There is no Red.
- **Adoption layers:** product only = Green. Plus knowledge or skill = Yellow. Heavy on all three = Red.
- **Touch-to-value:** no-touch = Green. Low- or high-touch with a plan to reduce it = Yellow.
  High-touch where the team must be involved before any value = Red.

Flag stacking yellows, especially Yellow Ocean plus Yellow Adoption. The source is Wes Bush's book.
Where it differs from `ICP Definition Builder.md`, the book wins: mid-market alone is Green.

### Step 4 — Map the buyer architecture

- **Buying committee** (*Buyer Personas* lesson): economic buyer (owns the budget), user buyer (uses
  it daily), technical buyer (evaluates specs and requirements), and coach or champion ("jazzed
  about your offering and they want to see you win"). One person can play several roles.
- **Expansion motion:** bottom-up or top-down, and the value multiplier.
- **PQL candidates:** 2-3 behaviors that show a user has hit meaningful value. "At Slack, a PQL is
  an account that has reached its 2,000 message limit" (Wes Bush). "Find these in data, not theory."

## Output

One file: `competitor-profiles/<company>-icp-<YYYY-MM-DD>.md`. Templates:
`references/templates.md`.

1. **The call.** One sentence naming the Core segment to lead with and what NOT to target yet.
2. **ICP definition sentence** (Keyplay format): "Our offering is best for [companies], who are [in
   situations], they focus on [outcomes], they struggle with [problems]."
3. **ICP priority map.** Every segment with maturity and time allocation.
4. **Signal table.** "Better if..." and "avoid if..." signals.
5. **One ICP profile per prioritized segment.** Data validation, maturity, energy, MOAT, buyer
   architecture, narrative implications.
6. **Open questions**, each naming the evidence that would resolve it.
7. **Hands off to:** `buyer-personas` (roles to interview), `account-scoring` (signal table), and
   positioning and messaging (Villain, Lead message, and Proof format fields).

## Constraints

- **No segment is promoted without data.** For arm's-length research (no CRM, no usage data, no
  surveys), every segment is **Hypothesis** and the Data Validation block says "not available,
  external research." Never fill it with guesses.
- Every claim cites its source: a live page, a review, `competitor-research` output, or customer
  data. The source classes are stated once at the top.
- Maturity is set by evidence (win rate, cycle length, customer count), never by who is excited.
- Name at least one Future segment and at least one "who NOT to target yet."
- Writing: one lead message per segment, no hedged recommendations, and open with the call.
  Name the workaround concretely: not "another CRM," but "your team exports from Salesforce... into
  a Friday afternoon spreadsheet" (*ICP Definition Builder*).

## Grounding

- `Product Marketing/ICP and Personas/`:
  - *ICP Definition Builder.md* (a secondary synthesis; checked against the primary sources below)
  - *You're building your ICP wrong* (primary source for M1/M2/M3)
  - *Wes Bush - MOAT PLG Fit (Product-Led Growth 2nd ed).md* (primary source for MOAT and PQL)
  - *Model and target a data-driven ICP with AI.md* and *Workbook_ ICP modeling with AI.md* (signal
    map and ICP definition sentence)
- `Product Marketing/Segmentation & Persona Research/`: *Buyer Personas* (buying committee)

## Related skills

- `competitor-research`: runs first. Supplies M3 competitors and competitive framing.
- `market-segmentation`: supplies the candidate segments.
- `buyer-personas`: next. Builds the people inside each prioritized segment.
- `account-scoring`: next. Turns the signal table into a 0-100 fit score for every account.
