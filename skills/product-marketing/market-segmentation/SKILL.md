---
name: market-segmentation
description: >-
  Split a company's market into a small set of usable customer segments, and
  decide which segmentation types to use. Use whenever the task involves
  "segment our market," "customer segmentation," "market segments," "how
  should we segment," "which segments exist," "firmographic" or
  "technographic segmentation," "segmentation survey," or "break the market
  into groups." Produces a segment map of 4 or fewer segments, each tested
  as measurable, accessible, substantial, and actionable. Feeds icp-definition,
  buyer-personas, and account-scoring. Built from the Segmentation and
  Persona Research course in `Product Marketing/Segmentation & Persona Research/`.
allowed-tools: Read Write Edit Bash WebSearch WebFetch
metadata:
  version: 1.0.0
---

# Market Segmentation

"Segmentation is the practice of dividing your market into smaller and more approachable groups"
(*Course Introduction*). The goal is to avoid "boiling the ocean" and find groups "you can easily
pursue with targeted and efficient strategies."

## Inputs

- **Company name and URL.** Required.
- **`competitor-research` final output**, if one exists for this company
  (`competitor-profiles/<company>-competitive-research-<date>.md`). Each segment has its own
  competitors: "for each segment, there's a different set of competition, a different set of
  players" (*Understanding Segmentation*). Use it to name the competitors per segment.
- **Any existing segmentation.** "Most businesses naturally segment their market" (*Understanding
  Segmentation*). Start from what they already do, then test it.

## Initial Assessment

Four factors decide how to segment (*Understanding Segmentation*). Answer each before choosing types:

1. **B2B or B2C?** B2B skews to firmographic, technographic, and some psychographic data. B2C skews
   to behavioral and geographic.
2. **Top-down or bottoms-up?** Top-down starts from a commercial goal ("where can we actually hit
   that revenue target?"). Bottoms-up starts from how individuals think about buying.
3. **Company stage.** Early-stage companies get bigger, broader segments: they are resource
   constrained and "still learning." Mature companies look for niche emerging segments.
4. **Corporate strategy.** Disrupting an existing category means segments are "pretty defined."
   Creating a new category means "a lot more research" to find them.

## The Five Segmentation Types

Demographic, behavioral, psychographic, geographic, and firmographic + technographic
(*Segmentation Deep Dives*). "It's not going to be one or none. It's probably going to be a mix of
a few." Attributes, benefits, data sources, and examples for each type:
`references/segmentation-types.md`.

For B2B, firmographic + technographic is the default backbone. Technographic ("technologies used")
is "often overlooked" and valuable when the product only works with certain tools.

## Process: Five Steps

From *How to Build Segments*:

1. **Preliminary research.** Ask customers "a combination of open-ended and structured questions."
   "Simply talking to your customers is extremely valuable and helps you get to insights quicker."
2. **Decide the segmentation types.** "There's no hard and fast rule here." Pick from the Initial
   Assessment and the five types.
3. **Gather the data.** Instrumented usage, website analytics, third-party databases, and surveys.
   Survey rules: open with the demographic or firmographic filter questions your team agreed on,
   keep answers structured, and make options "mutually exclusive and collectively exhaustive."
   Survey skeleton: `references/templates.md` → *Segmentation Survey*.
4. **Identify the segments.** "Limit yourself to four segments or less." More than four is
   "another segmentation effort altogether." "Be creative and experimental." "Take your time. This
   is the hardest part of the process."
5. **Test and iterate.** Every segment must pass MASA:
   - **Measurable:** can you tell whether someone is in the segment from the data?
   - **Accessible:** can you reach and act on this data?
   - **Substantial:** can this segment actually buy your product?
   - **Actionable:** segments are ideally mutually exclusive and collectively exhaustive.

## Common Mistakes

From *How to Build Segments*:

- **Wrong size.** Too small or specialized gives messaging "no room to breathe." You want
  one-to-many, not one-to-one.
- **Frozen segments.** "You're not going to define a set of segments and they're going to stay
  static forever." Set a revisit cadence.
- **Ignoring new personas.** "Be aware that new types of people may be entering your business
  audience."

## Output

One file: `competitor-profiles/<company>-segment-map-<YYYY-MM-DD>.md`, built from
`references/templates.md` → *Segment Map*. It holds:

1. **The call.** One sentence naming the segment to lead with and the one to deprioritize.
2. **Segmentation approach.** The four factors and the types chosen, with the reason for each.
3. **Segment map.** 4 segments or fewer. Each gets a name, defining attributes, estimated size,
   data source, competitors in this segment, and a MASA check.
4. **Open questions**, each naming the evidence that would resolve it.
5. **Hands off to:** `icp-definition` (which segments to prove and prioritize), `buyer-personas`
   (who sits inside each segment), and `account-scoring` (firmographic and technographic
   attributes to score on).

## Constraints

- Every segment attribute cites its source: a survey, a database, usage data, a live page, or
  `competitor-research` output. An attribute with no source is marked **[Hypothesis]**.
- For arm's-length research with no customer access, no survey or usage data exists. Build the
  map from public sources (the company's solutions and customer pages, review-site filters,
  job posts) and label the whole map a hypothesis to validate with a survey.
- Never exceed 4 segments in one map.
- Segmentation is not personas. A segment is "a portion of your market." A persona is "the people
  that might make up that segment" (*Buyer Personas*). Stop at the segment and hand people-level
  work to `buyer-personas`.

## Grounding

`Product Marketing/Segmentation & Persona Research/`: *Course Introduction & Overview*,
*Understanding Segmentation*, *Segmentation Deep Dives*, *How to Build Segments*.

## Related skills

- `competitor-research`: runs first. Supplies the competitors per segment.
- `icp-definition`: next step. Proves which segments are real and prioritizes them.
- `buyer-personas`: builds the people inside a segment.
- `account-scoring`: turns segment attributes into a 0-100 fit score.
