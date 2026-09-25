---
name: market-segmentation
description: >-
  Map and define the segments in a company's whole target market: who each
  segment is, what triggers them to buy, who is involved, what they use today,
  and how to attack it. Use whenever the task involves "segment our market,"
  "customer segmentation," "market segments," "how should we segment," "which
  segments exist," "map our market," "segmentation survey," or "break the
  market into groups." Produces a segment map of 4 or fewer segments that cut
  across industries, each tested as measurable, accessible, substantial, and
  actionable. Does not rank segments or pick a lead: that decision belongs to
  icp-definition. Feeds icp-definition, buyer-personas, account-scoring,
  positioning, and messaging. Built from the Segmentation and Persona Research
  course in `Product Marketing/Segmentation & Persona Research/`.
allowed-tools: Read Write Edit Bash WebSearch WebFetch
metadata:
  version: 1.1.0
---

# Market Segmentation

"Segmentation is the practice of dividing your market into smaller and more approachable groups"
(*Course Introduction*). The goal is to avoid "boiling the ocean" and find groups "you can easily
pursue with targeted and efficient strategies."

## Map the market, don't rank it

*Added after the Skillvue run, 2026-09-25. The first map led with the industry where Skillvue
already had customers, and Mike rejected it: "you shouldn't prioritize industries and verticals only
based on whether you have proof in them — that's the whole point of a startup — to win those and
then do the proof."*

- The map defines and describes segments. It does not rank them, pick a lead, or drop a segment
  because the company has no customers there yet.
- The market in scope is the **whole target market** (for example, "enterprises with 1,000+
  employees, any industry"), not the industries the company has already sold into.
- Existing customers show up as **examples** inside a segment, never as its boundary.
- Choosing where to go first belongs to `icp-definition`, which has the data to make that call.
- Early companies need "bigger segments" because they are "still learning" (*Understanding
  Segmentation*). A few broad segments, each big enough to learn in, beat narrow niches.

## Inputs

- **Company name and URL.** Required.
- **The market in scope:** size threshold, geographies, and expansion path. Take it from the user
  or the company's own site (offices, languages, "European enterprises"). Ask if it's unclear.
- **`competitor-research` final output**, if one exists
  (`competitor-profiles/<company>-competitive-research-<date>.md`). "For each segment, there's a
  different set of competition" (*Understanding Segmentation*). Use it to fill each segment's
  Current alternatives.
- **Any existing segmentation.** "Most businesses naturally segment their market." Read the
  company's own solutions page and customer-story filters first: they show how it already slices
  the market.

## Initial Assessment

Four factors decide how to segment (*Understanding Segmentation*). Answer each before choosing types:

1. **B2B or B2C?** B2B uses company traits to recognize segments. Role-level detail belongs to
   `buyer-personas`.
2. **Top-down or bottoms-up?** Top-down starts from a revenue goal. Bottoms-up starts from how
   buyers experience the problem.
3. **Company stage.** Early-stage companies get a few broad segments. Mature companies look for
   niche emerging ones.
4. **Corporate strategy.** Disrupting an existing category means buyers already shop for
   alternatives. Creating a new category means "a lot more research" to find the segments.

## How to cut the market

The five types are demographic, behavioral, psychographic, geographic, and firmographic +
technographic (*Segmentation Deep Dives*). "It's probably going to be a mix of a few." Attributes,
data sources, and examples: `references/segmentation-types.md`.

**B2B default** *(added after the Skillvue run, 2026-09-25)*: cut by **buying situation**, not
industry. A buying situation is the population or decision a company is trying to fix, plus the
buyer who owns it. One large company usually holds several buying situations at once, each with
its own trigger, budget owner, need, and competitors.
- **Behavioral** (the decision being made and what triggers the purchase) is the main cut.
- **Firmographic** (size, workforce or org shape) is how you recognize each segment from outside.
- **Geographic** maps the expansion path.
- **Technographic** is usually a fit signal for `account-scoring`, not a segment on its own.
- Industries go inside each segment as "where you find them."

The course's own advice supports cutting this way: "Be creative and experimental... don't be afraid
to slice your customer segments in ways that you haven't tried before" (*How to Build Segments*).

## Process: Five Steps

From *How to Build Segments*:

1. **Preliminary research.** Ask customers "a combination of open-ended and structured questions."
   With no customer access, use public sources: solutions pages, customer stories, industry pages,
   job posts, and `competitor-research` output.
2. **Decide the segmentation types.** Use the Initial Assessment and the B2B default above.
3. **Gather the data.** Instrumented usage, analytics, databases, and surveys. Survey rules: open
   with filter questions, keep answers structured, and make options "mutually exclusive and
   collectively exhaustive." Survey skeleton: `references/templates.md` → *Segmentation Survey*.
4. **Identify the segments.** "Limit yourself to four segments or less." "Be creative and
   experimental." "Take your time. This is the hardest part of the process."
5. **Test and iterate.** Every segment must pass MASA:
   - **Measurable:** can you tell from data or public signals who is in it?
   - **Accessible:** can you reach its buyers?
   - **Substantial:** is it big enough, and able to buy?
   - **Actionable:** is it distinct, with a different buyer or trigger from the others?

## Common Mistakes

From *How to Build Segments*:

- **Wrong size.** Too small or specialized gives messaging "no room to breathe."
- **Frozen segments.** "You're not going to define a set of segments and they're going to stay
  static forever."
- **Ignoring new personas.** "Be aware that new types of people may be entering your business
  audience."
- **Segmenting by where the proof is** *(Skillvue run, 2026-09-25)*: that draws the map around
  past sales, not the market.

## Output

One file: `competitor-profiles/<company>-segment-map-<YYYY-MM-DD>.md`, built from
`references/templates.md` → *Segment Map*. It holds:

1. **How to read this map:** the market in scope, how it's cut and why, the four factors, and the
   types used. State plainly that the map doesn't rank segments.
2. **Up to 4 segments.** Each gets a definition; where you find them (industries); how to recognize
   them from outside; the problem they're trying to fix; what triggers a purchase; who's involved
   (buyer, users, influencers); current alternatives; how the company fits, with customer examples;
   how to attack it (entry point, message, buyer); and a MASA check.
3. **How the segments relate:** different buyers and budgets, the land-and-expand path between
   segments, and how competition changes by segment.
4. **Open questions**, each naming the evidence that would resolve it.
5. **Hands off to:** `icp-definition` (which segment and geography to go after first),
   `buyer-personas` (the roles named in each segment), `account-scoring` (the signals that
   recognize each segment), and positioning and messaging (the entry message per segment).

## Constraints

- **Never rank the segments, pick a lead, or drop a segment for lack of proof.** Prioritization
  belongs to `icp-definition`.
- Every segment claim cites its source: a live page, a survey, a database, or `competitor-research`
  output. Company claims (stats, customer counts) are labeled as the company's own.
- For arm's-length research with no customer access, label the whole map a hypothesis and name the
  survey or conversations that would validate it.
- Never exceed 4 segments in one map.
- Segmentation is not personas. Name the roles involved in each segment, then hand the people-level
  work to `buyer-personas`.

## Grounding

`Product Marketing/Segmentation & Persona Research/`: *Course Introduction & Overview*,
*Understanding Segmentation*, *Segmentation Deep Dives*, *How to Build Segments*.

## Related skills

- `competitor-research`: runs first. Supplies each segment's current alternatives.
- `icp-definition`: next step. Decides which segments to go after first, and proves them.
- `buyer-personas`: builds the people inside each segment.
- `account-scoring`: turns each segment's recognition signals into a 0-100 fit score.
