# Account Scoring Templates

## Contents
- Account Scoring Document (the full output)
- Scoring Model
- Tier Map
- 1/1/1 Play Card
- Pipeline Weather Report
- TAM Penetration View
- Executive Slide

---

## Account Scoring Document

```markdown
# [Company] — Account Scoring

**Date**: [YYYY-MM-DD] · **Model status**: [Tested against N best / N DQ / Untested hypothesis]
**Source classes**: (1) directly observed · (2) company's or vendor's own claim · (3) this skill's judgment (weights, cutoffs)

## The call
[One sentence: which tier gets the budget, and what spend to cut.]

## Scoring model
[Scoring Model]

## Tier map
[Tier Map + one 1/1/1 Play Card for A and one for B]

## Measurement setup
[Pipeline Weather Report + TAM Penetration View, or "N/A: no CRM access (external research)"]

## Open questions
- [Question]: resolved by [specific evidence]

## Hands off to
- GTM / demand gen: [plays per tier]
- buyer-personas: [roles to reach inside A accounts]
```

---

## Scoring Model

```markdown
| Signal | Type (better if / avoid if) | Weight | Why this weight | Source |
|---|---|---|---|---|
| [e.g. 10+ AEs in account-based territories] | better if | +20 | [strength in best vs DQ contrast] | [data / public] |
| [e.g. consumer apps] | avoid if | -25 | | |

**AI-scored signals**: [signal] (prompt: "[rate X on 1-10 from the website]")
**Tier cutoffs** (this skill's judgment): A = [x-100] · B = [...] · C = [...] · D = [0-...]
**Test result**: best customers → [% A/B] · DQ leads → [% C/D] · [pass / re-weight]
```

---

## Tier Map

```markdown
| | Tier A | Tier B | Tier C | Tier D |
|---|---|---|---|---|
| Definition (score + traits) | | | | |
| Accounts in SAM | | | | |
| GTM effort | Full activation | Targeted | Passive | Inbound only |
| Spend / CAC | High (fits ACV) | Medium | None targeted | Zero paid/outbound/ABM |
| Plays | [Play Card] | [Play Card] | — | — |
| Pause permanently | — | — | [channels/plays/reps] | [channels/plays/reps] |
| CAC-to-ACV note | | | | |
```

---

## 1/1/1 Play Card

```markdown
**Tier**: [A / B] · **Audience**: [one segment inside the tier]
**Message**: [one specific pain, e.g. "Experiencing death by audits?"]
**Offer**: [one next step that solves it]
**Channels**: [...] · **Teams**: [...] · **Expected CAC**: [...] · **Outcome**: [SQLs / meetings / $ pipeline]
```

---

## Pipeline Weather Report

```markdown
# Pipeline Weather — Week of [date]

**Intro**: [2-3 sentences, directional]

**Forecast**
- Tier A: ☀️ Sunny / ⛅ Cloudy / 🌧️ Rainy — [one line why]
- Tier B: [...]

**Leading indicators** (WoW)
| | This week | Last week | Δ |
|---|---|---|---|
| Meetings booked | | | |
| Accounts showing intent / engagement | | | |
| Accounts moving stages | | | |

**Lagging indicators**
| Opportunities created | Pipeline value | Closed-won |
|---|---|---|

**Qualitative**: accounts broken into (3-4 sentences each) · deal story · risks · wins
```

---

## TAM Penetration View

```markdown
| | A | B | C | D |
|---|---|---|---|---|
| Accounts in TAM | | | | |
| Engaged | | | | |
| Qualified | | | | |
| Opportunities | | | | |
| Closed | | | | |
| Penetration % | | | | |
```

---

## Executive Slide

```markdown
- TAM by tier: [...]
- Penetration by tier: [...]
- Pipeline created this quarter: [...]
- Weather snapshot: A [☀️/⛅/🌧️] · B [...]
- What improved: [one sentence]
```
