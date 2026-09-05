---
name: pmm-segmentation-icp
description: 'Required before defining, validating, or prioritizing a target customer segment or ICP for a B2B SaaS product. Use whenever Mike asks to define an ICP, prioritize segments, build buyer personas, or figure out who a product is actually for — including as the second job in the PM sequence, gated on a Market & Competitive Reality artifact already existing (see pmm-competitive-market-intelligence). No positioning, messaging, storytelling, pricing, or launch work should start without this job''s output. Draws on the B2B Marketing OS: ICP and Personas — https://app.notion.com/p/3d019b7dd908813e85faf60670dae0dc (ICP Definition Builder, Model & Target a Data-Driven ICP with AI, Workbook: ICP Modeling with AI) and Segmentation & Persona Research — https://app.notion.com/p/3d019b7dd908818bb21cc382a9cdd0e6 (Buyer Personas, How to Build Segments, Segmentation Deep Dives, Building Personas, Bringing It All Together).'
---

# Segmentation & ICP

## Goal
One ICP profile (or a small prioritized set) that downstream PM work can build on directly — not a firmographic guess. "Done" means the profile has an actual maturity level, an actual energy state, and actual buyer architecture, each backed by evidence, not aspiration.

## Required input
The Market & Competitive Reality artifact from Job 1. If it doesn't exist yet, run that job first — don't define an ICP against assumed market context.

## The lead methodology
Use **ICP Definition Builder** as the primary procedure, in its own stated order:
- **Step 0 — Data validation.** Before calling any segment real, check it against retention, usage, survey signal, and paying-customer count if that data exists. A segment that looks right on paper but doesn't show up in these signals is wrong — say so. If this data doesn't exist for the product in question (new/unlaunched, no analytics), say that plainly and treat the resulting ICP as a hypothesis, not a confirmed segment — don't quietly skip the check.
- **Step 1 — Segment definition & maturity (MKT1).** Role + Company Type defines a segment. Assign Core/Scaling/Testing/Future by evidence, not by what Mike wants to be true.
- **Step 2 — Market energy (FletchPMM M1/M2/M3).** This is the layer that actually changes the narrative logic downstream — classify each segment's energy state before any messaging gets written. M1 (potential, barrier is the villain), M2 (kinetic, workaround is the villain), M3 (captured, incumbent is the villain). Get this wrong and everything downstream inherits the wrong villain.
- **Step 3 — PLG fit (Wes Bush MOAT).** Note: the doc's own referenced deep-dive file for full MOAT scoring rubrics isn't present in this KB as of this build — work from the summary table in the main doc, and flag if a MOAT call feels underspecified rather than inventing rubric detail that isn't there.
- **Step 4 — Buyer architecture.** Same caveat — the referenced buyer-architecture template file isn't present; use the key-fields list in the main doc.

Use the **Segmentation & Persona Research** transcripts as the how-to layer underneath this — when the main doc's steps need more procedural depth (how to actually run a segmentation exercise, how to build a persona from scratch), pull the relevant transcript rather than improvising.

## Live cross-check
Run `mkt1_icp_prioritization` against the same product and compare its role+company-type output to what the KB procedure produced. If they materially disagree, surface it — don't silently pick one.

## Constraints
- Keep ICP (team/company level) and Persona (individual level) separate — don't collapse them past the fast-map stage once a segment is promoted to Core.
- A broad ICP is worse than no ICP — "B2B startups" is an industry label, not a segment.
- No triple value prop, no hedged recommendations, no throat-clearing in the output — state maturity, M-type, and MOAT calls directly.
- Don't promote a segment's maturity level on vibes — the data validation checklist gates that.

## Output artifact
One ICP Profile per prioritized segment, following the Full ICP Profile Output structure in ICP Definition Builder: data validation status, ICP/Persona split, MKT1 maturity + time allocation, M-type + narrative implications (villain, promised land, lead message, proof format), MOAT assessment, buyer architecture. This is what Positioning, Messaging, and Storytelling consume next — particularly the Villain, Lead Message, and Proof Format fields.

## What's deliberately left open
How many segments to prioritize, how deep the persona work goes per segment, which MOAT/buyer-architecture gaps matter enough to flag versus note and move past.
