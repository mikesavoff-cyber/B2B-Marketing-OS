# Templates

## Contents
- Constitution (the output)
- Working notes (the work)
- Audit memo

---

## Constitution

*Shape approved on the Skillvue run, 2026-09-27 (v2), with Mike's fixes to "current ways" and
"why we win." The decisions section follows `MKT1 - Positioning statement template.md`.*

This is the only file that goes to `competitor-profiles/`. It holds decisions, not process: no
gates, citations, interview guides, stage headers, scoring tables, or red-team tables. About 150
lines at most. Each slot is filled by the component the registry chose (`methodology-map.md`);
leave out a slot only when the registry says it doesn't apply, and say so in one line.

```markdown
# [Company] positioning

**Version [n], [date]. Status: [hypothesis until tested with customers / tested / approved].**
Built from: [inputs, one line]. Sources: (1) observed, (2) company's own claims, (3) judgment.

## The bet
[2-3 sentences: what we are, who it's for, what we lead with; what we refuse to lead with, and why.]

## At a glance
| | |
|---|---|
| **For** | [primary audience] |
| **Category** | [the frame] |
| **We replace** | [the 2-4 current ways we fight, a few words each] |
| **Why we win** | [the one differentiator, one sentence] |
| **Villain** | [the thing] |
| **Promise** | [recommended simple promise] |
| **Proof** | [3-5 names] |

## Who it's for, and who it isn't
**For:** [who, the trigger that puts them in market, the buyer who owns the question]
**Not for:** [2-4 bad fits, each with the reason]

## What we are: the category
[2-3 sentences on why the product is hard or easy to frame.]
**Recommendation: [frame].** [the budget it maps to; the vendor list it puts us next to; how the
modifier carries the difference]
**Considered and rejected:** [each frame in one line, with the reason]

## The current ways we replace
| Situation | How it's done today | Who does it | Why it breaks |
|---|---|---|---|
| [decision] | [the specific spreadsheet, vendor, ritual, consultancy, or habit] | [role] | [the failure this buyer feels] |

## Why we win
**[The one differentiator, one sentence.]**
[2-4 sentences: the trade-off every current way accepts, and why only we escape it.]
How it's true: [1-3 capabilities, as proof of the one idea]

## Positioning statements
**Core statement:** For [primary audience] who [situation], [company] is the [category] that
[what]. Unlike [primary current way], it [differentiator], so [outcome].

**By situation.** Same differentiator, different entry.
| Situation | Who | Statement | Proof |
|---|---|---|---|
| [situation] | [buyer] | For [who] facing [situation], [company] [does what]. Unlike [its specific current way], [why better] | [named proof, or "not yet public"] |

## The story
- **Change:** [the shift that already happened]
- **Stakes:** [who wins, who loses]
- **Villain:** [the thing, not the feeling]
- **Promised land:** [what the customer becomes]

**Simple promise options, for testing:**
1. **"[recommended]"** [why, one line]
2. "[option]" [trade-off, one line]
3. "[option]" [trade-off, one line]

## We will not position as
- [frame, and the shelf it would put us on]

## Summary of decisions
- **Product type:** [chosen from 10x better / new way / vertical solution / buy vs. build], so the comparator is [ ].
- **Audience:** [primary, and the other segments that get messaging, not their own positioning]
- **Awareness:** [problem / solution / product aware], so "what it is" [explains the problem / the solution / our approach].
- **Why better, options considered and rejected:** [each in one line]
- **Research behind it:** [links to competitor-research, segment map, ICP, notes]

## Open questions
- **[Question]** Resolved by: [specific evidence]
- **[Accepted weakness from the red team]** Resolved by: [specific evidence]

## Hands off to
- **messaging:** the core statement and each situation statement as its own message track.
- **storytelling-sales-narratives:** the story and the promise options.
- **product-launch:** [lead theme].
- **pricing-packaging:** [what the category and bundling imply].
```

---

## Working notes

Saved to `~/competitor-research-work/<company>-positioning-<date>/notes.md`. Cite sources here.
Checkpoints are argued here before Mike sees a short summary in chat.

```markdown
# [Company] positioning notes, [date]

## Gate check
Inputs present / missing; insider material received; option taken.

## Evidence ledger (evidence-ledger.md)
### Company reality
| Claim | Evidence | Source | Class | Confidence | Would falsify it | Implication |
### Market evidence
(same columns)
### Critical unknowns / useful unknowns

## Retrieval log (retrieval-protocol.md)
| Decision | Sources read (file, section) | Relationship | Primary method | Supporting | Why |
Unmapped files found, and what the new-source protocol decided.

## Component choices (methodology-map.md registry)
| Slot | Component chosen | Rejected | Why |

## Stage 1: Evidence
Readiness; audience; situations; current ways per situation; language bank; interview guide
(only if interviews are missing).

## Stage 2: Readings
Classification (crosswalk row), mismatches, category existence test, comparators, awareness,
game, credibility ceiling, horizontal path.
| Reading | Evidence for | Cost / risk | Verdict |

## Stage 3: Core
Capabilities → so what → value. Candidate differentiators. Category frames tested. Statement
drafts. Gate results.

## Stage 4: Story
Element tests. | Promise option | Simple | Transformation | Slays villain | Feels true + proof | Customer language | Fits demand type |
Pitch-setup check.

## Stage 5: Red team (red-team.md)
| Claim | Adversary | Attack | Evidence for the attack | Verdict | Change |

## Stage 6: Test
Pitch storyboard, test plan, fail criteria, results log (never invented), rollout order.
```

---

## Audit memo

```markdown
VERDICT: [one sentence]
Current positioning, reverse-engineered: comparator / product type / who / what / why
| Finding | Source rule it fails | Evidence | Rerun stage |
Rerun plan: [stages, in order]
```
