# Methodology map

The positioning knowledge base is a connected system, not a flat folder. This file says what each
source is, which decision it owns, what it depends on, and which part of the constitution it can
fill. Paths are relative to `Product Marketing/`. Read `retrieval-protocol.md` for how to use it.

## Contents
- Layers
- Source inventory
- Component registry (what fills each constitution slot, and when)
- New-source protocol
- Known source defects

---

## Layers

Every source, or section of a source, sits in one layer. Two sources with similar titles in
different layers are not duplicates.

| Layer | What it does | Example |
|---|---|---|
| Foundation | Defines what positioning is and what it is not | MKT1 guide intro, Dunford §1 |
| Process | The steps, in order | Dunford §4, MKT1 guide Steps 1-3 |
| Component | Produces one element of the answer | Dell L5 villain, Fletch §6 anti-value prop |
| Template | The shape the answer is shared in | MKT1 statement template, Dunford §5 canvas |
| Validation | Tests whether the answer works | MKT1 guide Step 3.5, Dunford §9, Dell L8 |
| Diagnostic | Finds what is broken in existing positioning | Dell L1 five questions, MKT1 Complete §12 |
| Application | A worked example or context variant | SnoutDesk, Pocus teardown, Snowflake |
| Support | Helps the work but holds no positioning method | Problem framing |

## Source inventory

| File | School | Layers | Owns these decisions | Depends on | Feeds |
|---|---|---|---|---|---|
| `Positioning/The MKT1 Guide to positioning.md` (Steps 1-4, full) | MKT1 | Foundation, process, validation | Research ≠ positioning; product type + comparator; who / what (by awareness) / why better; one differentiator; multiple audiences or products | Research outputs: primary audience, competitor map, primary problem | Messaging |
| `Positioning/MKT1 - Positioning statement template.md` | MKT1 | Template | The company-wide share format: statement block on top, "summary of decisions" below, options considered and rejected | The guide, Steps 2-3 | The constitution's statement block and decisions |
| `MKT1 - Complete Marketing Framework.md` §4, §12 | MKT1 (secondary synthesis) | Process summary, diagnostic, application | Five positioning mistakes; Pocus teardown principles | The guide | Audit mode, messaging |
| `Positioning/April Dunford Positioning Framework` | Dunford (secondary synthesis) | Foundation, process, template, validation | Alternatives by approach; capabilities → value themes; best-fit and bad-fit; category decided last; readiness; sales-pitch test; quality checks | Traction, a team, real short lists | Canvas, pitch test, messaging doc |
| `Positioning/Fletch PMM Positioning Frameworks` | Fletch (secondary synthesis) | Component, application, validation | Category strategy (mature / immature / new); choosing 2 alternatives; anti-value prop; stand-out vs. education game; existing category for budget; JTBD anchor; product-markets-fit; credibility levels; homepage and anti-fluff tests | Primary audience | Category, current ways, "not for," gates, messaging (§2, §4, §5, §7, §8, §12 belong to messaging) |
| `Positioning/Transcript - ... The 8 Elements ...` (Dell L1) | Market of One (Dell) | Foundation, diagnostic | The eight story elements; five positioning-problem questions; story over statement | None | Story |
| `... Identify Your Best Customers` (L2) | Dell | Component | Best customer by spend, speed, frequency, stakes; gut → sales → data | Deal data, if any | Audience (only when `icp-definition` is missing) |
| `... Mine Your Best Customers ...` (L3) | Dell | Process | 12 interview questions mapped to elements; 7-10 interviews | Best customer | Evidence ledger (customer language) |
| `... Identify Your Demand Type` (L4) | Dell | Component | New concept / new paradigm / established category; nine questions | Current alternatives | Story emphasis, category strategy |
| `... Change, Stakes & Villain` (L5) | Dell | Component | Change (real, relevant, risky); stakes; villain criteria | Demand type, customer language | Story |
| `... Promised Land ... Superpowers ... Proof` (L6) | Dell | Component | Promised land (five elements); superpowers (unique, loved, effective); 3+ proof points | Value themes | Story, proof |
| `... Memorable Simple Promise` (L7) | Dell | Component | Simple promise (six elements); 3-5 options | Villain, promised land | Promise |
| `... Test Your Positioning Story and Roll It Out ...` (L8) | Dell | Validation | Pilot, deck and landing-page tests, 5+ best customers, bottom-of-funnel-first rollout | Story, promise | Test plan |
| `Positioning/Problem framing for positioning, messaging, storytelling, and copywriting.md` | Support (Mural and others) | Support | A problem statement cut from 40 to 20, 10, then 5 words; customer and business angles; root cause | None | The problem line in the bet, only when the team disagrees on the problem |

## Component registry

The constitution has fixed slots. The skill decides which component fills each slot for this
company. Record the choice, and the components rejected, in the working notes. One slot gets one
primary component; add a supporting one only when it adds something the primary can't.

| Slot | Default component | Use instead or add when | Never |
|---|---|---|---|
| **The bet** | MKT1 product type + comparator, plus Fletch §19 game | Add the problem-framing statement (5 words) when the evidence shows teams describing the problem differently | Write it before Stage 3 is approved |
| **For / not for** | `icp-definition` primary audience + Fletch §6 anti-value prop | Dell L2 best customer only when there's no ICP output and Mike accepts a hypothesis; Dunford best-fit as the consistency check | Pick the audience by where case studies sit |
| **Category** | Dunford §3 component 5 (context that makes value obvious), chosen from Fletch §1 strategy | Existing category + modifier (Fletch §18) when no label covers the product's breadth (conflict 11); JTBD anchor (Fletch §14) for a new way | Invent a category name for an early-stage company without Mike's written sign-off (conflict 4) |
| **Current ways** | Dunford alternatives grouped by approach, then Fletch §13 to choose the 2 to fight | MKT1 comparator for the product type when one comparator dominates | List a category of methods instead of the specific method |
| **Why we win** | MKT1 "why better" (one differentiator vs. the comparator), derived via Dunford capabilities → value | Fletch §3 when features match competitors (difference lives in who and what you replace); Fletch §20 caps it at current proof | List several strengths |
| **Statements** | MKT1 three-blank statement for the primary audience | One statement per situation or segment when buyers, triggers, or current ways differ (conflict 10, Fletch §16); a future statement (MKT1 3.5) only if Mike asks; one full re-run per product for multi-product companies (MKT1 Step 3) | Change the differentiator between statements |
| **Story** | Dell L5-L6 (change, stakes, villain, promised land) | Full eight elements when the buyer isn't solution aware (new way, new paradigm); change + villain only for a 10x-better stand-out game | Tell a story that argues against a different comparator than the statements |
| **Promise** | Dell L7, 3-5 options scored on the six elements | Fletch §8 anti-fluff test on every option; Fletch §20 proof per option (conflict 6) | Promise an outcome the proof doesn't show |
| **Will not position as** | Rejected category frames + anti-value prop | Name the shelf each rejected frame would put the company on | Pad it with frames nobody proposed |
| **Decisions summary** | MKT1 template "summary of decisions": product type chosen from the four, audience tiers, awareness level, options considered for "why better" | Only when the constitution is shared company-wide (default: yes) | Paste research into it; link out instead (MKT1 process step 3) |
| **Test plan** (notes) | Dunford §6 pitch + Dell L8 deck and landing-page tests | Fletch §17 homepage test when a homepage exists | Invent test results |

## New-source protocol

The folder will grow. A file that isn't in the inventory above is unmapped. Never use an unmapped
file silently, and never skip it.

1. Read the whole file, including its 3-line header.
2. Classify it: school, layer(s), the decisions it owns, what it depends on, what it feeds.
3. Compare it with every mapped source that owns the same decision. Name the relationship:
   foundation, process, template, validation, diagnostic, application, alternative approach,
   complementary method, or genuinely redundant. Similar titles are not proof of redundancy.
4. If it disagrees with a mapped source, add an entry to `conflicts.md` marked "open for Mike."
5. If it offers a new way to fill a constitution slot, add it to the component registry as an
   option. The default changes only after Mike approves.
6. Add a row to the inventory and to `Product Marketing/_INDEX.md` in the same session.
7. Tell Mike in the chat summary: what the file is, where it sits, and what it changes.

## Known source defects

1. **Dunford and Fletch files are secondary syntheses** ("Complete Framework Reference"), not the
   authors' own text. Say "per the Dunford reference file" when a call depends on exact wording.
2. **Dunford §9 embeds a routing instruction** ("April as strategic advisor supporting
   Fletch-led work"). That is a system decision, not Dunford's method. Ignore it; use
   `conflicts.md`.
3. **Dunford §9 misstates Fletch on category timing.** Fletch §14 puts the category *name* last;
   §1 makes category *strategy* the first bet. See conflict 3.
4. **Dunford's value-theme count varies** (1-3 in one place, 1-4 buckets in another). Use 1-3.
5. **The MKT1 template's placeholder rows pair "Buy vs. build" with the new-way comparator.**
   Filler, not a matched example. The template also words 10x better as "better solution to known
   problem in existing category"; the guide omits "known problem."
6. **MKT1 Complete's table of contents doesn't match its headings.** Cite heading numbers.
7. **Dell's worksheet, brand canvas, and spreadsheet are not in the repo.** The 12 questions are
   recoverable from L3; the canvas fields are L1's eight elements.
