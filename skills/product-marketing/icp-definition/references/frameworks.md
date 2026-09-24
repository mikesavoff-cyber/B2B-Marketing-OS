# ICP Frameworks — Full Rules

Read mid-task when a step needs its full detail. Sources are named per section.

## Contents
- Step 0: Data validation and signal map
- Step 1: MKT1 segment maturity
- Step 2: M1 / M2 / M3 energy
- Step 3: MOAT PLG fit
- Step 4: Buyer architecture

---

## Step 0: Data validation and signal map

*Sources: ICP Definition Builder (PostHog method section); Keyplay Workbook, "Build a complete ICP
signal map."*

**Start narrow, add detail as confidence builds:**
1. Make a best guess with 3 attributes and test it immediately against real signups and customers.
2. Gather intel continuously: signup questions, retention comparisons, power-user analysis,
   NPS/PMF survey responses.
3. Add detail only as data confirms it. Each added attribute should narrow the definition.
4. "You'll know the ICP is right when it feels almost too narrow."

**Signal map (Keyplay):**
1. Pull 10-20 best customers (strong retention, high expansion, or high ACV) and 10-20 DQ leads
   (rejected for poor fit). Not churned accounts.
2. Enrich both lists with:
   - company size
   - industry and sub-industry
   - markets served
   - sales motion (sales-led, PLG, hybrid)
   - team structure
   - tech stack
   - growth indicators (hiring velocity, expansion, new product lines)
   
   "You're looking for patterns, not precision."
3. Traits shared by best customers become "better if..." signals.
4. Traits shared by DQ leads become "avoid if..." signals.
5. Contrast matters: "it looks like everyone in our best customers have Google Analytics... so do
   all of your DQ leads. So that doesn't make sense."
6. Draft the definition sentence: best for / who are / they focus on / they struggle with.

**Data signals that confirm a segment:** retention better than the base, usage higher (and
high-value events reached faster), NPS/PMF higher, sales cycle faster.

**Real enthusiasm (ICP signal):**
- visibly excited in the demo, not just polite
- strongly agrees with the problem framing, unprompted
- gives ongoing, specific feedback
- invites colleagues without being asked
- uses the product even when it's rough
- refers others with the same problem
- starts paying, or asks to pay before you charge
- shares the product publicly

**Polite indifference (false positive):**
- "interesting," "cool," "clever," with no commitment behind it
- uses it for something you didn't intend
- says they wouldn't pay when asked directly
- refers you to someone junior with no purchase authority

**Timing:**
- A real ICP takes 3-12 months to sharpen.
- Don't lock in off 1-2 customers. 5 similar paying customers is a real signal for B2B, and 10+ is
  strong confirmation.
- "Cold outbound is a legitimate ICP-testing tool... Warm intros produce polite yeses that look like
  signal and aren't."

**Checklist before promoting a segment's maturity:**
- [ ] Retains better than the base?
- [ ] Uses the product more and reaches value faster?
- [ ] Rates higher on NPS/PMF?
- [ ] 5+ paying customers who look like this (10+ for high confidence)?
- [ ] Real enthusiasm signals, not polite interest?
- [ ] Narrow enough that it could be wrong, or still "an industry label wearing an ICP costume"?

If any box is unchecked, the segment stays at its current maturity.

---

## Step 1: MKT1 segment maturity

*Source: ICP Definition Builder.*

- **Role:** specific. "VP of Marketing," not "marketers." "Head of RevOps," not "ops teams."
- **Company type:** specific enough to build a target list from. "Series B SaaS, 100-500 employees,
  product-led motion," not "tech companies."

| Level | Name | Meaning |
|---|---|---|
| 1 | Core | PMF proven. Shortest cycle, highest win rate, most efficient acquisition. |
| 2 | Scaling | Actively expanding into it. Product works, but messaging, channel, or motion still need refinement. |
| 3 | Testing | Early signal, unproven. No repeatable success yet. |
| 4 | Future | Intentionally deprioritized. Naming it "prevents it from sneaking into plans." |

**Time allocation reveals mismatches:**
- 40% on a Testing segment "because one exec is excited about it"
- nothing on Core "because it runs itself"
- time spread evenly instead of concentrated on proven segments

---

## Step 2: M1 / M2 / M3 energy

*Primary source: "You're building your ICP wrong." Narrative logic, villain, and proof format are
from ICP Definition Builder.*

**The firmographic trap:** "Just because a company matches a set of business attributes does not
mean its employees will need your product." Firmographics "aren't inherently evil — they are just a
bad starting point." Layer them on after choosing the M group.

| | M1: Potential | M2: Kinetic | M3: Captured |
|---|---|---|---|
| State | Desire exists, action blocked | Already doing it, worse | Already using a competitor |
| Example | Duolingo (80% weren't trying to learn before signup) | DocuSign (paper signing) | Figma (Adobe users) |
| Narrative | Remove the barrier | Redirect existing energy | Differentiate |
| Villain | The barrier (cost, complexity) | The workaround, named concretely | Incumbent limitations they already resent |
| Proof format | Before/after | Effort and time comparison | Head-to-head on what they care about |
| CRM example message | "Finally keep track of every lead" | "Skip manual updates for good" | "Salesforce is clunky. Ours is a delight." |

- **Mismatch:** tell a Salesforce user they'll "finally be able to track leads" and "they'll think
  you're crazy."
- **Prioritize:** "Choose one segment, devote 60 to 80% of the GTM budget to it." Going after all
  three means "three completely separate go-to-market campaigns."
- M2 in a red ocean is "the highest-leverage PLG ICP combination" (ICP Definition Builder).
- Record per segment: M-type, current behavior, trigger event, workaround, awareness level.

---

## Step 3: MOAT PLG fit

*Primary source: Wes Bush, Product-Led Growth 2nd ed. Full extract:
`Product Marketing/ICP and Personas/Wes Bush - MOAT PLG Fit (Product-Led Growth 2nd ed).md`.*

| Dimension | Green | Yellow | Red |
|---|---|---|---|
| Market | SMB or mid-market | Mid-market with significant enterprise | Pure enterprise (structural) |
| Ocean | Red ocean | Blue ocean (educate first) | None |
| Adoption | Product only | Product plus knowledge or skill | Heavy product, knowledge, and skill |
| Touch-to-value | No-touch | Low- or high-touch with a plan to reduce | High-touch before any value |

**Reading the flags:**
- **All green:** PLG now.
- **Yellows:**
  - Ocean yellow → pair education with the product.
  - Adoption yellow → guided onboarding or AI agents.
  - Touch yellow → automate the path to value.
- **Yellows stacking:** "Fix the flags, then build the motion."
- **Enterprise only:** use product-led elements to support sales. Don't build strategy around
  self-serve.
- **Founder blind spot:** founders "forget that they have years of context that their users don't."
  Test adoption with someone who has never seen the product.

**PLG spectrum by ACV:**
- Sales-led: above ~$50k
- Hybrid product-led sales: ~$5k-$50k
- Self-serve: below that

---

## Step 4: Buyer architecture

*Sources: Buyer Personas lesson (buying committee), Wes Bush (PQL), ICP Definition Builder (fields).*

**Buying committee:**

| Role | Who | What they need |
|---|---|---|
| Economic buyer | Owns the budget | ROI, risk, proof |
| User buyer | Uses the product daily | Ease, fit to their workflow |
| Technical buyer | Evaluates features, specs, regulations | Requirements met |
| Coach / champion | Wants you to win | Material to sell internally: ROI framing, security docs, case studies |

- "Sometimes one person might play multiple roles."
- "At the beginning of a sales cycle, it's really important to know who these people are... and
  then have a strategy for winning each of them over."

**Profile fields:**
- **End user:** role, JTBD, activation definition, first-week success, champion signals.
- **Economic buyer:** role, buying trigger, risk concerns, proof required, deal-size threshold.
- **Champion:** who, what activates advocacy, what they need to sell internally, their risk if it
  goes wrong.
- **Expansion:** bottom-up or top-down. Value multiplier: collaboration, data, integration, or none.
- **PQL candidates:** 2-3 behaviors, found in data. Slack's 2,000 messages "was discovered
  empirically."
