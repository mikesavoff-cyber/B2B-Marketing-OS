# Audit mode (Cases B, C, D)

Goal: diagnose existing positioning and say which stage is broken. Don't rebuild what works.

## Read first

1. Dell L1: the five "do you have a positioning problem" questions.
2. MKT1 Complete §12: five mistakes, root causes, and the Pocus teardown's six principles.
3. MKT1 Complete §4 Step 3.5: signs positioning isn't differentiated.
4. Dunford §9: quality checks and common gaps.
5. Fletch §17 (homepage test), §8 (anti-fluff), §15 (four ways companies outgrow positioning),
   §20 (credibility gap).

## Do

1. **Get the current positioning as it's actually stated.** Homepage hero, pitch deck, any
   positioning doc. Pull the homepage live. Optional: the MKT1 connector
   `mkt1_homepage_positioning` gives a structured read against MKT1's framework. Treat it as a
   second opinion, not the verdict.
2. **Reverse-engineer it** into the Stage 2 and 3 fields: implied comparator, product type,
   who, what, why better. Blank fields are findings.
3. **Run the diagnostics.** Each finding cites the source rule it fails:
   - MKT1 five mistakes (bad research, forest for the trees, kitchen sink, inside baseball,
     game of telephone).
   - MKT1 Complete §4 Step 3.5 signs.
   - Dunford §9 checks.
   - Fletch §17 three questions, §8 fluff test, §20 credibility question.
   - Dell L1 five questions.
4. **Case C only:** match the situation to one of Fletch §15's four challenges.
5. **Route.** Map each finding to the stage that fixes it:

| Finding | Rerun |
|---|---|
| Unclear who it's for, too many audiences | Stage 1, then Stage 3 "who" |
| Wrong or missing comparator, competing with everything | Stage 2 |
| Kitchen sink, 2-3 differentiators, fluff | Stage 3 |
| Claims outrun proof | Stage 2 credibility, then Stage 3 |
| Clear positioning, weak copy (game of telephone) | Not positioning. Hand to `messaging`. |
| No urgency, "nice to have" reactions | Stage 4 |
| Never tested with buyers | Stage 5 |

## Output

Diagnosis memo: the verdict in one sentence, the reverse-engineered positioning, findings with
source citations, and the rerun plan. Template in `templates.md`, section "Audit memo."
