---
name: pmm-positioning
description: >-
  Decide and test a product's positioning: who it's for, what category frames it, the specific
  current ways it replaces, the one reason it wins, and the story that makes switching feel
  urgent. Use for "define our positioning," "position [product]," "what should we compare
  ourselves to," "which category are we in," "is our positioning working," "audit our homepage
  positioning," "reposition after [change]," "villain," "simple promise," "positioning story,"
  "positioning canvas," or "review my positioning statement." Produces one short positioning
  document (the constitution) with a core positioning statement plus one statement per segment
  or situation. Feeds messaging, storytelling, launch, and pricing. Runs after icp-definition and
  competitor-research.
allowed-tools: Read Write Edit Bash WebSearch WebFetch
metadata:
  version: 0.2.0
---

# Positioning

Four schools live in `Product Marketing/Positioning/`. They answer different questions and
sometimes disagree. This skill routes between them. It never replaces them. Every stage reads the
source sections named in its stage file before doing the work.

**Two layers, never mixed** *(added after the Skillvue run, 2026-09-27)*:
- **Working notes** hold the work: evidence, interview guides, gates, source citations, rejected
  readings. They live outside the project, in `~/competitor-research-work/<company>-positioning-<date>/`.
- **The constitution** holds the answer: one short document a CEO decides from, and every
  downstream team builds from. It goes in `competitor-profiles/`. It shows no process.

Mike rejected the first Skillvue output because "it shows the work" and never delivered a
positioning statement. The work stays in the notes. The answer is the only thing that gets shipped.

## Step 0: classify the request

| Case | Trigger | Run |
|---|---|---|
| A. New positioning | Nothing approved exists | Stages 1 → 5 in order |
| B. Audit | "Is this working," a live homepage or deck | `references/audit.md`, then only the stages it flags |
| C. Reposition | Product, ICP, or market has moved | Audit first, then Stage 2 onward |
| D. Review a draft | Mike pastes a statement or canvas | Stage 3 gates, then Stage 4 gates |

If the case is unclear, ask one question with these four options. Do not default to A.

## Required inputs

- **`icp-definition` output.** It decides the primary audience. Without it, do not pick a best
  customer from where the proof sits: that ranks the market by past sales, which Mike rejected for
  segmentation. Offer to run `icp-definition` first.
- **`market-segmentation` output**, if it exists. Its segments become the rows of the situation
  statements.
- **`competitor-research` output.** Supplies the competing tools and their positioning.
- **Insider knowledge.** Ask Mike for any conversations with founders, product, sales, or
  customer success: transcripts, call notes, interview notes. They carry what public pages can't:
  what the company thinks its differentiator is, where deals come from, what it plans to stop
  selling. This is the substitute for Dunford's team exercise. Label it class 2.
- **Customer evidence:** interviews, win/loss notes, deal data, reviews.

A missing input is a gate. Say which is missing and offer: (1) run the upstream skill or get the
material, or (2) proceed, with every affected field marked **[Hypothesis]** in the notes and the
whole constitution labeled hypothesis at the top.

## The stages

Each stage file lists the source sections to read, what to do, and what goes in the notes.

1. **Evidence** (`references/stage-1-evidence.md`). Primary audience, the decisions or situations
   the product serves, the specific current ways each situation is handled today, and customer
   language.
2. **Strategic choice** (`references/stage-2-strategic-choice.md`). Category strategy, product
   type, comparators, awareness, game, credibility ceiling. 2-3 readings with a recommendation.
3. **Positioning core** (`references/stage-3-core.md`). The category frame, the one
   differentiator, the core statement, and one statement per segment or situation.
4. **Story** (`references/stage-4-story.md`). Change, stakes, villain, promised land, proof, and
   3-5 simple promise options.
5. **Test and roll out** (`references/stage-5-test.md`). Pitch test, pilot, rollout order.

## Live checkpoints (never resolve these alone)

1. **After Stage 2:** the audience, the current ways worth fighting, and the strategic reading.
2. **After Stage 3:** the category frame, the differentiator, and the statements.
3. **After Stage 4:** which simple promise goes to testing.

Show Mike each call as a short summary in chat, not as a document: the recommendation, the
competing readings, and the evidence for each. Mike absent: mark the call **[Hypothesis]** and
continue. Never present it as settled.

## What makes the constitution good

*Added after the Skillvue run, 2026-09-27.*

- **It contains positioning statements.** One core statement, plus one per segment or situation
  the product serves. A document without statements is not positioning.
- **The category covers everything the product does.** A product that informs many decisions
  cannot be framed by one use case. When no existing label covers the breadth, prefer an existing
  category plus the modifier that carries the difference ("the data warehouse built for the
  cloud"). Show the rejected frames in one line each.
- **Current ways are specific.** Name the actual method each situation runs on today: the
  spreadsheet, the named vendor, the annual ritual, the consultancy, who does it, and why it
  breaks for this buyer. If a row would fit any company's positioning, it is not specific enough.
- **One differentiator.** Why-we-win is one idea stated as one sentence. Capabilities appear only
  as the proof of how it's true. A list of three strengths is a failure.
- **Contrasts are real opposites.** "Evidence, not visibility" failed because the words are too
  close. Test each "X, not Y" by asking whether a buyer would feel the gap.
- **No process on the page.** No gates, interview guides, source citations, stage headers, or
  scoring tables.

## When the schools disagree

Read `references/conflicts.md` before blending anything. Each conflict has a ruling and the
condition that flips it. Never average two schools. If a conflict isn't in the register, show Mike
both readings and add it after he rules.

Use `references/crosswalk.md` whenever a classification appears. Pick the primary taxonomy it
names. Never stack all four in any artifact.

## Constraints

- **Source first.** Read the stage's source sections before writing. Cite them in the notes, never
  in the constitution. If the sources don't cover a question, say so in the notes and label the
  reasoning as judgment.
- **Credibility beats ambition.** Every claim needs proof that exists today (Fletch §20). A
  situation with no proof keeps its statement and says "proof: not yet public" in its row.
- **No manufactured customer insight.** Villain, change, and promise come from customer or
  insider evidence, or they are marked **[Hypothesis]**.
- **Known source defects** are listed in `references/source-map.md`.
- Writing follows `claude.md` Output Expectations. No "it's not X, it's Y" constructions.

## Output

1. **Constitution:** `competitor-profiles/<company>-positioning-<YYYY-MM-DD>.md`, built from
   `references/templates.md` → *Constitution*. About 150 lines at most.
2. **Working notes:** `~/competitor-research-work/<company>-positioning-<YYYY-MM-DD>/notes.md`,
   built from `references/templates.md` → *Working notes*.

## Grounding

- `Product Marketing/_INDEX.md`, Positioning rows.
- `references/source-map.md` for which file and section owns which question.
- `Product Marketing/MKT1 - Complete Marketing Framework.md` §4 (Steps 1-3.5, the statement
  format) and §12 (mistakes and the Pocus teardown).

## Related skills

- `icp-definition`: runs first. Decides the primary audience.
- `market-segmentation`: supplies the segments that become situation statements.
- `competitor-research`: supplies the competing tools.
- `messaging`: next step. Turns each statement into a message track.
- `storytelling-sales-narratives`: turns the story into decks and pages.
