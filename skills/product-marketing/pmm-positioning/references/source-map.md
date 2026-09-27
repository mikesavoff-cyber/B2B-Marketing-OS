# Source map

Which source owns which question. Read this before citing a source. All paths are relative to
`Product Marketing/`.

## The four schools

| School | Author | File(s) | What it's best at |
|---|---|---|---|
| Dunford | April Dunford | `Positioning/April Dunford Positioning Framework` | Building positioning from real competitive alternatives with a team, for products that already have traction. Testing it through a sales pitch. |
| MKT1 | Emily Kramer | `Positioning/The MKT1 Guide to positioning.md` (Steps 1-2 only; the file stops there), `MKT1 - Complete Marketing Framework.md` §4 (Steps 1-3.5, including the statement format), §3, §5 (Perceptions), §12 (Pocus teardown) | Getting out of the weeds. Product type picks the comparator, then one who/what/why statement. Diagnosing overworked positioning. |
| Fletch | Fletch PMM (Anthony Pierri is named in MKT1 Complete §12) | `Positioning/Fletch PMM Positioning Frameworks` | The strategic bet: which category strategy, which alternatives to pick, category creation, budget reality, credibility. |
| Market of One | Brendan Dell (CXL course) | 8 files: `Positioning/Transcript - Positioning - *.md` | Customer-led narrative: best customers, interview mining, demand type, change and stakes, villain, promised land, simple promise, testing and rollout. |

Plus one supporting file, which is not a school:

| File | What it is | Use it for |
|---|---|---|
| `Positioning/Problem framing for positioning, messaging, storytelling, and copywriting.md` | Three general design-thinking articles (one is from Mural). No positioning method. | Only when the blocker is team disagreement about the problem. The 5 W + H prompt and the "we already know the problem" move are the useful parts. |

## Section index by question

| Question | Primary source | Secondary |
|---|---|---|
| Do we have a positioning problem? | Dell L1 (five questions) | MKT1 guide positioning mistakes figure; Fletch §15 four challenges |
| Is this method right for our stage? | Dunford §2 | Fletch §15 (outgrown positioning) |
| Who is the best customer? | `icp-definition` output | Dell L2 (gut, sales team, data: deal size, time to close, win rate); Dunford §3 component 4 |
| What do customers actually compare us to? | Dunford §3 component 1, §4 step 1 | Dell L3 question 1; MKT1 Complete §3 ecosystem map |
| Which alternatives do we choose to fight? | Fletch §13 | MKT1 guide Step 2 comparator |
| What customer evidence do we need? | Dell L3 (12 questions, 7-10 interviews) | Dunford §4 "before you start" |
| Same features as competitors: where does differentiation live? | Fletch §3 (ICP, alternatives, problem named, benefit) | Fletch §13 |
| Mature, immature, or new category? | Fletch §1 | Dell L4 demand type; MKT1 guide Step 2 product type |
| Should we create a category? | Fletch §14, §18 | MKT1 guide "new way" section; Dell L8 ("sometimes you just need to take the leap") |
| Stand-out game or education game? | Fletch §19 | Fletch §5 awareness stages |
| What can we credibly claim today? | Fletch §20 | MKT1 Complete §4 Step 3.5 ("too aspirational") |
| Horizontal product, many markets? | Fletch §16 | Fletch §11, §9 |
| Distinct capabilities and value themes | Dunford §3 components 2-3, §4 steps 2-3 | Dell L6 superpowers (unique, loved, effective) |
| Market category | Dunford §3 component 5 | Fletch §14, §18 |
| The positioning statement | MKT1 Complete §4 Step 3 (who / what by awareness / why better) | Dunford §5 canvas |
| Many situations, one product: which frame, how many statements? | Fletch §16 (product-markets-fit), §18 (existing category) | `conflicts.md` entries 10, 11 |
| What is the one differentiator? | Dunford §3 components 2-3 (so what → value) | MKT1 Complete §4 Step 3 ("one differentiator") |
| Who we are not for | Fletch §6 anti-value prop | Dunford §3 bad-fit accounts |
| Is the statement differentiated? | MKT1 Complete §4 Step 3.5 | Dunford §9 quality checks; Fletch §17 homepage test |
| Change and stakes, villain | Dell L5 | Dunford §6 Insight; Fletch §14 step 2 |
| Promised land, superpowers, proof | Dell L6 | Dunford §6 Perfect World, Proof |
| Simple promise | Dell L7 | Fletch §8 anti-fluff test |
| How to test | Dunford §6-7 sales pitch; Dell L8 pilot | Fletch §17 homepage test |
| Rollout | Dell L8 (bottom of funnel first) | MKT1 guide ("share the statement, link out to research") |
| Positioning vs. brand story vs. messaging | MKT1 guide positioning hierarchy; MKT1 Complete §5 story stack | Dunford §1, §8 |

Dell lesson numbers: L1 = 8 Elements, L2 = Identify Your Best Customers, L3 = Mine Your Best
Customers, L4 = Demand Type, L5 = Change, Stakes & Villain, L6 = Promised Land, Superpowers &
Proof, L7 = Simple Promise, L8 = Test and Roll Out.

## Sections that belong to other skills

Positioning reads these only as downstream context. It does not produce these artifacts.

- Fletch §2, §4, §5, §7, §8, §12: messaging, personas, awareness-stage assets, website pages.
  Owned by `messaging`.
- Fletch §9, §10, §11: GTM focus and revenue shape. Read §9 and §11 only when Stage 2 hits a
  horizontal-product question.
- Dunford §8 messaging document: owned by `messaging`. Stage 5 hands off to it.
- MKT1 Complete §10 website messaging architecture: owned by `messaging`.

## Known source defects (fix in the repo, not in this skill)

1. **The MKT1 guide file stops after Step 2.** `Positioning/The MKT1 Guide to positioning.md` has
   Steps 1-2 as text; its product-type table and research figure are embedded images. Steps 3
   and 3.5 exist only in `MKT1 - Complete Marketing Framework.md` §4. Cite §4 for the statement.
   There is no `MKT1 - Positioning statement template.md` in the repo; MKT1's one-page template
   is paywalled.
2. **The Dunford and Fletch files are secondary syntheses.** Both are titled "Complete Framework
   Reference." Neither is Dunford's or Fletch's own text. Treat their summaries as reliable, but
   say "per the Dunford reference file" when a call depends on exact wording.
3. **Dunford §9 embeds routing instructions inside a source.** It casts April as "strategic
   advisor (supporting Fletch-led work)." That's a decision about this system, not Dunford's
   method. This skill ignores it and uses `conflicts.md` instead.
4. **Dunford §9 misstates Fletch on category timing.** It says Fletch "sometimes starts with
   category framing earlier." Fletch §14 says the category name comes last, and Fletch §1 makes
   category *strategy* (mature, immature, new) the first bet. Both files agree the category
   *name* comes last. See conflict 3.
5. **Dunford's value-theme count is inconsistent.** §3 says 1-3 themes and 1-4 buckets. §5
   shows up to three. Use 1-3.
6. **`_INDEX.md` ranks Dunford "primary" and Fletch "secondary lens."** That ranking conflicts
   with this skill's per-question routing. Update the index rows to the "Read when" wording in
   this file.
7. **MKT1 Complete's table of contents doesn't match its headings.** The TOC lists 13 sections
   with "Positioning Mistakes" as 13. The headings stop at 12, which is "Positioning Mistakes,
   Diagnostics, and Pocus Teardown." This skill cites heading numbers (§12).
8. **Dell's worksheet, brand canvas, and 12-question spreadsheet are not in the repo.** The
   transcripts reference them as downloads. The 12 questions are recoverable from L3's text.
   The canvas fields are the 8 elements from L1.
