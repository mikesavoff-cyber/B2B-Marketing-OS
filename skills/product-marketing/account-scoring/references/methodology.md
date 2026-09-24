# Account Scoring Methodology — Full Detail

*Source: Keyplay (Eric Linssen), "Model and target a data-driven ICP with AI" (the transcript is
primary), and "Workbook: ICP modeling with AI" (the exercises).*

## Contents
- Why ICP sits upstream
- Signal map (if icp-definition hasn't run)
- Building and testing the model
- Engagement tiers and plays
- Measurement

---

## Why ICP sits upstream

"Everything in your company is downstream of ICP":
- customer success, retention, and expansion
- product metrics like time to value
- cost per qualified lead and cost per opportunity

Framing for leadership: "I want to solve this ICP problem, not because I care about marketing only,
but because I care about NRR."

---

## Signal map (if icp-definition hasn't run)

1. Pull 10-20 **best customers** (strong retention, high expansion, or consistently high ACV) and
   10-20 **DQ leads** ("accounts you intentionally rejected because they were a poor fit"). "Do
   *not* use churned accounts."
2. Enrich both lists with:
   - company size
   - industry and sub-industry
   - markets served
   - sales motion
   - team structure (AEs, SDRs, RevOps, Security)
   - tech stack (CRM, MAP, category tools)
   - growth indicators (hiring velocity, expansion, new product lines)
3. Traits shared by best customers become "better if..." signals. Traits shared by DQ leads become
   "avoid if..." signals.
4. Draft the definition: "Our offering is best for [companies] / Who are [situations] / They focus
   on [outcomes] / They struggle with [problems]."

Keyplay's own example of good signals:
- 10+ AEs assigned to account-based territories
- sophisticated RevOps
- HubSpot as the source of truth
- selling multiple products
- a territory planning project coming up

Tools named: Google Sheets/Excel, CRM (Salesforce, HubSpot, Pipedrive), LinkedIn and company
websites, enrichment (Apollo, ZoomInfo, Clay, Clearbit), and ChatGPT or Claude to classify patterns.

---

## Building and testing the model

- Take the signals and "weight them appropriately" to produce 0-100 fit scores across the SAM.
- **AI for signals:** "If you look at signals that you care about about target accounts... that
  maybe a best AE would look at." AI reads the website and scores things like "do they have an
  existing partner program" (PartnerStack) or "is it an e-commerce or an online marketplace," which
  "is pretty difficult for the existing tools to do."
- **Test:** run DQ leads and top customers through the model. DQ leads should land mostly C and D,
  and top customers high. Keep tweaking until they do. Without the test, "people are still gonna
  just go out building their own lists."

---

## Engagement tiers and plays

**Workbook exercise:**
1. Select 3-5 A-tier segments, 3-5 B-tier segments, and your C and D buckets.
2. Assign effort: Passive, Targeted, or Full Activation. Tier rules are in SKILL.md.
3. For A and B, design one play each:
   - **Audience:** one ICP segment inside the tier
   - **Message:** a specific pain unique to that audience
   - **Offer:** a next step that solves it (framework audit, benchmarking report, teardown)
   - Also define: channels, teams involved, expected CAC, and desired outcome (SQLs, first
     meetings, pipeline amount)
4. For C and D: list the channels, plays, and reps wasting time, mark what pauses permanently, and
   define what stays inbound-only.
5. Final tier map: definitions, effort, A/B plays, C/D elimination rules, and CAC-to-ACV notes.

**Worked examples:**
- **PartnerStack:** tiers split across SMB, mid-market, and enterprise. An A-scoring account gets
  full activation. A low-scoring enterprise account gets no targeted spend.
- **Thoropass:**
  - Message: "Experiencing death by audits?"
  - Audience: companies with multiple compliance frameworks
  - Offer: in-house auditors instead of multiple outside auditors
  - Run as always-on ads plus a coordinated LinkedIn strike
- **Keyplay:** a security-audience play with the message "avoid wasting money on bad-fit accounts"
  and a strategic AI segmentation offer.

---

## Measurement

**Pipeline Weather Report** (PartnerStack CMO Tyler's format, "treat it like a weekly newsletter and
build subscribers"):
1. Intro: 2-3 sentences on what happened this week.
2. Weather forecast per A and B tier: Sunny (ahead of pace), Cloudy (stable, needs attention), Rainy
   (pipeline at risk).
3. Leading indicators, week over week: meetings booked, accounts showing intent or engagement,
   accounts moving stages.
4. Lagging indicators: opportunities created, pipeline value, closed-won. Use sparklines or arrows.

"MQLs are only MQLs [from] target accounts, and they're more valuable at their A's."

**TAM penetration view:** accounts per tier A/B/C/D, then how many are engaged, qualified, created as
opportunities, and closed. Map the tiers against enterprise, mid-market, and SMB for the total
dollar value of the market opportunity, which "investors love to see."

**Qualitative insights**, weekly:
- 2-3 accounts broken into, each with a 3-4 sentence summary
- a deal story or call snippet
- emerging risks
- wins

**Executive slide:** TAM by tier, penetration by tier, pipeline this quarter, the weather snapshot,
and one sentence on what improved. Use it for the monthly leadership and board update.

This "positions you as a strategic operator, not a channel executor."
