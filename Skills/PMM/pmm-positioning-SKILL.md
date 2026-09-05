---
name: pmm-positioning
description: 'Required before writing or evaluating a positioning statement, villain/problem framing, promised land, or positioning story for a B2B SaaS product. Use whenever Mike asks to define positioning, pick a comparator/villain, or evaluate whether current positioning is working — gated on an ICP Profile (pmm-segmentation-icp) and Market & Competitive Reality (pmm-competitive-market-intelligence) already existing. This is the gate for the rest of Product Marketing: nothing in Messaging, Storytelling, Pricing, or Launches should run until this job''s output is approved. Draws on the B2B Marketing OS Positioning folder: https://app.notion.com/p/3d019b7dd90881269061c77a51817dc7 (CXL/FletchPMM 8-part sequential course, and The MKT1 Guide to Positioning, which itself is written in direct response to April Dunford''s positioning methodology).'
---

# Positioning

## Goal
One tested positioning statement — who it's for, what it beats, why it's different — backed by the actual ICP and actual competitive reality, not assumption. This is a gate. Everything downstream in PM waits for your approval of this output.

## Step 0 — Classify the task before picking an order
The CXL/Fletch 8-step sequence and MKT1/Dunford are not "primary" and "cross-check" in a fixed order — which one leads depends on what Mike is actually asking for. Classify first:

**A. Defining positioning where none exists yet.** CXL/Fletch leads — it's the generative, build-from-nothing procedure. Run steps 1-8 in order, then cross-check the finished statement against MKT1/Dunford (see below). This is the default case and the one described step-by-step further down.

**B. Auditing or evaluating positioning that already exists** ("is this working," "what's wrong with our positioning," a homepage with a stated position already on it). MKT1 leads here — call `mkt1_homepage_positioning` first to get a structured diagnostic against its framework. Only pull the specific CXL/Fletch transcript(s) that address whatever the audit flags as weak (e.g. if it flags an unclear differentiator, fetch step 3, Change/Stakes/Villain, specifically — don't re-run the whole 8-step sequence when only one component is actually broken).

**C. Repositioning after a market or competitive shift.** Start with `mkt1_competitive_research` and/or `mkt1_perceptions` (call `Notion:notion-search` for "MKT1 perceptions" if the underlying methodology page needs checking) to establish what actually changed. Then re-run only the CXL/Fletch steps that shift depends on — usually step 2 (Demand Type) and step 3 (Villain), since a market shift most often changes what customers are moving away from, not the whole positioning story from scratch.

**D. Second opinion on a statement Mike already drafted.** Run the MKT1/Dunford cross-check first — it's the faster pass — then pull specific CXL/Fletch steps only where that cross-check flags a gap.

Don't default to A just because it's listed first. Ask what Mike is actually trying to do with this call if it's ambiguous which case applies.

## Required input — soft dependency, not a hard block
Check first whether an ICP Profile (pmm-segmentation-icp) and Market & Competitive Reality (pmm-competitive-market-intelligence) already exist for this product — check the product's Notion page if one exists, or just ask Mike, rather than assuming they're missing and re-running jobs that already happened. If both exist, use them directly and move on.

If either is missing, offer a choice rather than blocking:

> "I don't have an ICP Profile / Market Reality for this yet. Want me to (A) run that job now with a proper research pass, or (B) work from whatever you can tell me about the segment and competitors right here, as a lighter input?"

If Mike picks B, proceed on what he gives you, but mark the resulting positioning fields as based on unvalidated input rather than treating them as equivalent to a fully-run job — don't quietly upgrade a quick answer to the same confidence level as researched evidence.

## Opening the work
Before starting the chosen case's procedure, ask: "Want a quick refresher on how Fletch's model and MKT1's model differ, or ready to dive straight in?" If he wants the refresher, give the one-paragraph version — Fletch builds a narrative (villain, stakes, promised land) through 8 sequential steps; MKT1 answers 3 questions (who/what/why-better) against 4 product types — then proceed. If he's ready, skip straight to the procedure.

## Draft-and-confirm discipline
Every judgment call this skill makes — demand type, villain pick, comparator, product-type classification, differentiator — gets labeled **DRAFT** when first presented: "This is a draft based on [what you know]. Anything you'd change?" Don't move to the next step until Mike confirms or revises it. This matters most at step 2 (Demand Type) and step 3 (Villain) — get those wrong and every step after inherits the error. Only confirmed content goes into the final output artifact.

## Case A procedure — CXL/FletchPMM, run in sequence

**Before each step below, call `Notion:notion-fetch` on that step's exact URL and read it. Do not proceed from memory of what "Fletch's framework" or "positioning theory" usually says — the whole point of this skill is that the method comes from this specific page, not from training data. If a URL 404s or the page has moved, call `Notion:notion-search` with the step's title as the query to relocate it before continuing — don't silently fall back to general knowledge.**

1. **Identify Your Best Customers** — https://app.notion.com/p/3d019b7dd90881a3a22ac18c00f7c6d1 — fetch, then validate the ICP Profile's segment against this method; not a fresh exercise.
2. **Identify Your Demand Type** — https://app.notion.com/p/3d019b7dd90881059213cc17c5a6b6b7 — fetch, then cross-check against the ICP's M-type. They should agree; if they don't, that's a flag to resolve, not to average.
3. **Identify a Compelling Change, Stakes & Villain** — https://app.notion.com/p/3d019b7dd908818f9ddeedaa515d9184 — fetch, then refine the villain candidate the ICP Profile already produced from its M-type mapping (M1=barrier, M2=workaround, M3=incumbent). Don't invent a villain from scratch here.
4. **Craft an Effective Promised Land & Superpowers & Proof** — https://app.notion.com/p/3d019b7dd90881d8bc8be50810112cec — fetch, then depends on 1-3 being locked.
5. **Create a Memorable Simple Promise** — https://app.notion.com/p/3d019b7dd90881c6ac75ee3c0c77b059 — fetch, then synthesize 1-4.
6. **The 8 Elements of Your Positioning Story** — https://app.notion.com/p/3d019b7dd90881dab42cd76db0980cb7 — fetch, then assemble 1-5 into the full structured draft statement.
7. **Mine Your Best Customers for Effective Positioning** — https://app.notion.com/p/3d019b7dd9088192bf68c275cb660cb9 — fetch, then pressure-test the draft against real customer evidence; not a repeat of step 1.
8. **Test Your Positioning Story and Roll It Out** — https://app.notion.com/p/3d019b7dd90881998ad3ffbc092fff75 — fetch, then pull Market & Competitive Reality again here specifically, for proof points and go-to-market framing.

## MKT1 / Dunford cross-check — timing depends on the case above (see Step 0)
Fetch **The MKT1 Guide to Positioning** — https://app.notion.com/p/3d019b7dd9088102802ac6318c714de4 — the guide is written as a direct counterpoint to April Dunford's methodology (it credits her by name as "the master of positioning"), so working from it carries her perspective natively — no separate Dunford pass needed. Pair it with whichever live connector call fits the case: `mkt1_positioning` for a fresh definition (Case A), `mkt1_homepage_positioning` for an audit (Case B), `mkt1_perceptions` or `mkt1_competitive_research` for a shift-driven repositioning (Case C). If MKT1's read disagrees materially with what the CXL/Fletch work produced, present both territories to Mike with the disagreement named plainly. Don't silently pick one or blend them into a compromise position.

## Optional — only if stakeholder alignment is genuinely the blocker
"Problem framing for positioning, messaging, storytelling, and copywriting" — https://app.notion.com/p/3d019b7dd90881ed9c74ff24f7da6d61 — is generic design-thinking material, not part of the CXL/Fletch/MKT1/Dunford methodology chain. Fetch and use it only if the actual obstacle is getting a team to agree on the problem statement, not as a technique for step 3.

## Constraints
- No contrast-reframe thesis structures in the final statement ("it's not X, it's Y") — state the position directly.
- Don't blend Fletch's output and MKT1's output into one franken-positioning — if they agree, say so; if they don't, surface it.
- The villain must trace back to the ICP's M-type, not be picked independently at step 3.

## Refinement loop — before anything gets saved
Once the statement is fully assembled (end of Case A step 6, or the audited/repositioned equivalent in Cases B/C/D), ask: "Anything here you want to refine — the villain, the demand type, the promise, anything else?" If Mike flags a specific piece, redo only that step — re-fetch that transcript, rerun that step's logic — rather than restarting the whole sequence. Keep this loop open until he says it's good to lock. Only then move to Save & Handoff.

## Save & handoff
Once confirmed (not draft), ask: "Want me to save this so Messaging, Storytelling, Pricing, and Launches can pick it up automatically?"

If yes, take the first option you can actually do:
1. **Notion write access available.** Ask before writing — it's Mike's workspace, not yours to edit silently. If a page for this product already exists in the B2B Marketing OS workspace, replace its "# POSITIONING STATEMENT" section (same header, replace not append) with this one; if no such page exists, create it there. Once written, give Mike the exact page URL so downstream jobs can be pointed at it directly.
2. **No Notion write, but an artifact is available.** Put the confirmed statement in an artifact headed "# POSITIONING STATEMENT" — something he can keep and paste into a downstream job later.
3. **Neither.** Give it in one copyable code block under the same header.

Say plainly where it ended up. Never claim a save that didn't happen. If Mike declines to save, output as clean text and note that downstream jobs will need it pasted back in manually.

## Output artifact contents
Positioning Statement: target segment, demand type, villain (change/stakes), promised land + superpowers + proof, simple promise, the 8 elements assembled, MKT1/Dunford cross-check result (agree or flagged disagreement), roll-out proof points.

## What's deliberately left open
Exact wording of the final statement, how many territories to draft before converging, how much customer-mining evidence is enough.
