# Market & Competitive Intel Research Workflow

Purpose: identify and research a company's real competitive set, grounded in verified data only. Never in invented categories, invented facts, or unverified assumptions.

Source: the 10-lesson Competitive Intel course in `Product Marketing/Competitive Intel/` (sequence verified via each transcript's own next/previous-lesson references, not inferred from filenames). This file only documents what has actually been executed and validated so far — Steps 0-8, plus one suggested (not required) downstream action after the workflow completes. Nothing past this point is written until we've actually gone through it.

A separate, downstream workflow (`battlecard-weekly-refresh.md`) consumes this workflow's Step 5 output and keeps it current on a schedule. See that file for the automated-refresh process — it is not part of this one-time research workflow.

## Step 0: Ground the target's real category first

Run `mkt1_homepage_positioning` on the target's own homepage before anything else.

Purpose: establish the real product type (10x Better / New Way / Vertical Solution / Buy vs Build) and the real comparator, from what the homepage actually says — not from the company's own invented category language, and not from assumption.

**Before this step is considered done, crawl the full site, not just the homepage.** Follow every nav and footer link, specifically: Customers, Case Studies, Proof/Results, Product/Platform pages, Pricing, About, Resources. A real, documented failure of this workflow happened by skipping this: a run concluded a target had "no proof of value beyond a few named logos" while its actual Customers/Case Studies page — never fetched — held real proof the whole time. That is not a minor miss; it's a false claim about the target stated with confidence, built entirely on laziness about which pages got read. The homepage is where positioning language lives; it is never where proof lives. Never conclude anything about a company's evidence, customer base, or capabilities from the homepage alone.

Never accept a company's self-described category name (e.g. a made-up product category) as real market structure without this check. If the check finds a category-confusion or positioning-mismatch gap, note it — that gap is itself a finding, and it will bias any later competitor search that isn't corrected for it.

Output: product type, real comparator, positioning gaps.

## Step 1: Identify the competitor set

1. Ask for insider/known-competitor knowledge first, before running any tool. Ask: what competitors does the company itself name (job posts, decks, interviews, sales material)? What do you already know, and why does each one matter? Capture name + reason for each. This step applies to every project, whether or not prior research already exists for it.
2. Set the goal metric, if the data exists: competitive win rate, won ÷ (won+lost), tracked overall and per competitor. If no internal deal data exists (e.g. external research, no CRM access), say so and skip it. Don't invent a number.
3. Run automated discovery to fill gaps only, never as the primary source: `mkt1_competitive_research`, option C ("find from scratch": web search + `/vs/` page detection + shared-customer signal) or option B (expand a starter list). Interpret every discovered candidate against the real product type from Step 0, not an invented category — this is the specific failure mode that missed real competitors and over-trusted a made-up category in the first run of this process.
4. Combine into one list: insider names (with reasoning) + discovery names.
5. Present the full list back for correction. Never treat it as final until confirmed. State no fact about any candidate unless verified live or given directly.
6. Cap the confirmed list at 5. Expand later, once the system built around those 5 is running.

## Step 2: Research each competitor across the 3 stakeholder lanes

Source: Lesson 2 (Gathering Competitive & Market Insights: Startups & Mid-Market).

For each confirmed competitor, gather ALL of the following before answering any question — never answer a lane's questions from partial research:

**Marketing lane** (positioning, buyer, market sentiment):
1. **The whole site, not just the homepage** — live fetch, not memory. Homepage first for positioning/hero language, then follow every nav and footer link: Customers, Case Studies, Proof/Results, Product/Platform pages, Pricing, Resources. Proof of value lives on the Customers/Case Studies page, essentially never on the homepage — a competitor's evidence does not get marked "doesn't exist" until those specific pages have actually been fetched and read, not just linked from the nav.
2. G2 / TrustRadius / Trustpilot / Glassdoor — pull via web search when direct site access is blocked; capture both praise and complaints, not just star ratings.
3. Community check — Reddit, Quora, LinkedIn (posts/discussion, not the company page), Facebook groups, Discord, Slack. Run all of them, not just Reddit. Report an empty result as a real finding ("no public community presence found"), never skip a source silently or fabricate chatter that isn't there.

**Product lane** (how it's used, where it's strong/weak):
1. Knowledge base / docs / developer portal — feature depth, how it actually works.
2. G2/TrustRadius filtered to feature-specific feedback, not general sentiment.
3. Google Alerts substitute — this skill cannot configure a live, ongoing alert. Run a one-time news search as a proxy and say plainly that real ongoing monitoring still needs to be set up by the human running this.

**Leadership lane** (growing, fading, or acquired):
1. LinkedIn Premium Insights tab substitute — this skill does not have Premium access. Use Crunchbase, PitchBook, Tracxn, and press coverage (funding rounds, layoffs, acquisitions, executive hires) instead, and say plainly it's a substitute, not the named source.
2. When sources disagree on a hard number (funding total, headcount), report both and flag the discrepancy rather than picking one.
3. Check specifically for the two outcomes that change a competitor's status entirely: being acquired (no longer an independent buying decision) and material layoffs/funding drought (real distress, not spin) — both are bigger findings than any star rating.

**Answering the 3 marketing questions:** only after all three lanes above are gathered, not before. If new information surfaces later (e.g. a later community-search pass finds something a first pass missed), go back and revise the earlier answer — don't leave it stale. This was gotten wrong once in this process: the marketing questions were answered before the full community pass ran, and had to be corrected afterward.

## Step 3: Synthesize into the final competitive brief

Source: senior-PMM output quality, per the system's own Output Expectations bar (not itself a numbered lesson).

Structure, in this order:
1. **The bet** — one paragraph naming the overall competitive picture and the single highest-leverage move, stated before any per-competitor detail.
2. **The target's own positioning reality check** — restate the Step 0 finding up top; every recommendation downstream depends on it.
3. **At-a-glance comparison table** — one row per competitor: trajectory, core wedge against the target, sharpest exposure.
4. **Per-competitor sections** — positioning, buyer, market read, trajectory, and a concrete sales attack line for each. Every claim traces back to Step 2's research, nothing new introduced here.
5. **What this means for the target, directly** — named implications, each with a concrete consequence, not generic advice.
6. **Open questions** — each paired with what would actually resolve it, including any conflicting numbers found in Step 2.
7. **Handoff note** — what this artifact gates downstream (positioning/messaging work should not start until this is confirmed).

Publish to the project's actual Notion directory, inside its Market Research/Competitive Intel folder — not just left in chat.

## Step 4: Catalog every insight and route it

Source: Lesson 4 (Understanding Your Audience: An Ongoing Mindset).

Treat internal stakeholders as an audience, not a captive recipient list — insight that never reaches someone in a form they'll actually read has the same value as insight that was never gathered.

For every finding produced in Step 2, log it in a table with exactly these columns:

| Company | Insight | For Team | Channel | Cadence |
|---|---|---|---|---|

1. **Company** — which competitor (or the target itself) the insight is about. Group rows by company, keep them together — don't interleave across companies.
2. **Insight** — a 1-2 sentence summary in plain language, not a copy-pasted source excerpt.
3. **For Team** — which stakeholder(s) it benefits: Sales, Marketing, Product, or C-suite.
4. **Channel** — which of the three distribution channels it routes to: Battlecard (sales/marketing, quick-dismiss use), Newsletter (product/C-suite, strategic-update use), or Slack/Teams channel (company-wide FYI). An insight can route to more than one.
5. **Cadence** — Monthly (the default) or **Immediate**. Immediate applies only to the named major-event categories: acquisitions, funding rounds, major product releases, or comparably severe events (e.g. a live lawsuit, a large layoff independently reported as business distress). Immediate items get delivered the moment they're found, not held for a batch.

This table is the artifact that Lessons 5 (battlecards) and 6 (newsletter) pull from — it is not itself the battlecard or the newsletter.

## Step 5: Build the battlecards

Source: Lesson 5 (Building Battlecards for Sales & Marketing Teams), objectives 1-3, applied with the story-arc structure below.

**Lesson's 3 objectives, answered directly:**
1. **The single most important thing to include:** the "quick dismiss" — a 2-3 sentence bullet citing the competitor's real weakness, the target's real strength, or both — placed above everything else, because most of the time a rep just needs to move past a competitor's name mid-call, not read a full comparison.
2. **Tools, by budget:** affordable — build in-house with a design team, or a Canva license (upload brand colors, pick a template, keep it plain and to-the-point, don't over-design); bigger budget — Crayon or Clue's native battlecard filters, synced to their tracked competitor feed (Lesson 3, paid tier).
3. **Where to distribute:** wherever the sales/marketing team's collateral already lives (Drive, Dropbox/Box, or a CMS like Highspot/Seismic/Showpad, or directly in Salesforce) — never a new location people have to remember. Communicate it in an existing recurring venue (a standing team meeting), and treat the card as a living collaboration: ask for feedback on how well the quick dismisses land, fold in what's already working informally, revisit with the same team about 4 weeks later with an improved version. This distribution/feedback loop requires an actual internal sales team and CMS — mark N/A for external research, same as Win/Loss and displacement campaigns.

**Story-arc structure for the card content itself** (applied on top of the lesson's own format, for cards that need to be run live and spoken, not just read):

Each battlecard is written as a compressed 6-beat arc a rep can run in 30-60 seconds on a live call:

1. **Stasis** — the prospect's current belief or assumption about the competitor.
2. **Trigger** — the actual line the prospect says that starts this moment ("We're also looking at X").
3. **Rising action** — 2-3 escalating facts, each one raising the stakes higher than the last, all traceable to Step 2's verified research — never invented for dramatic effect.
4. **Climax** — the single sharpest, most damning fact, stated as its own short line.
5. **Falling action** — the pivot to the target's own position, stated as relief, not attack.
6. **Resolution** — a concrete next step the rep actually asks for (a pilot, a walkthrough, a document to send) — never ends on the dismissal alone.

Every fact in the arc must trace back to Step 2 or Step 4's table. The arc reorders and dramatizes verified findings; it never introduces new ones.

## Step 6: Build the newsletter

Source: Lesson 6 (Competitive Newsletters for Product & the C-Suite).

**What it's for, and why it's built differently from the battlecard:** the battlecard (Step 5) stays deliberately shallow so a rep can act on it in seconds mid-call. The newsletter is the opposite audience — product teams and the C-suite — and is where real depth belongs: strategic and product updates (M&A, funding, partnerships, major releases, positioning/messaging shifts), tied back to the target's own situation, never a copy-pasted press release.

**Critical input rule, learned the hard way in this process:** pull from ALL prior research steps — Step 0 (the target's own positioning reality check), the full depth of Step 2 (not just its routed one-liners), and any Enterprise-tier data (SEMrush, Gartner Peer Insights) — never from Step 4's cataloging table alone. Step 4's table is a compressed routing log by design; using only its one-line summaries produces a newsletter with real facts but none of their supporting specifics (exact figures, named sources, review counts, discrepancies). The first run of this step made exactly that mistake and had to be redone pulling from the full research base.

**Before writing individual items, look for the bigger story:** don't just list events — the lesson's own method is that a landscape moves in small increments until a single event resets the whole category (its worked examples: Salesforce/Slack, HubSpot/The Hustle, the iPhone). Check whether the period's findings share a pattern (e.g. multiple acquisitions/distress events clustering in the same window) and lead with that, not with an unconnected list.

**The 3-question filter, applied per insight before it's included:**
1. How does this relate to the target company?
2. Is there a bigger story to this?
3. What questions does this raise — and do the legwork to answer them (follow up on an internal/adjacent data point) rather than leave the question open in the newsletter itself.

**Structure:**
1. Table of contents at the top, most important item first, with a real teaser line per item, not just a title.
2. Per-item format: competitor name as the heading, a short bolded one-line verdict under it, then a body — dense paragraph form, not bullet/emoji fragments (rejected once in this process for being less readable, not more).
3. A subject line and preview text at the very top of the whole piece, written to actually earn an open (per the lesson's cited Litmus stat, preview text alone drives up to 24% of open decisions).

**Tooling named in the lesson:** Grammarly and the Hemingway App for the editing pass (apply their standard manually when the actual apps aren't available: short sentences, active voice, no unnecessary complexity); MailChimp for preview-text tooling, list management, and open/click tracking. Screenshots only when they clearly add signal beyond the text — don't include one by default.

**The communication step, same discipline as Step 5:** announce it's coming, ask for feedback afterward, treat it as a standing partnership with the recipients. Requires a real internal audience to do this with — mark N/A for external research, same as Steps 5's distribution loop, Win/Loss, and displacement campaigns.

**Cadence:** monthly baseline, immediate exception for major events (same rule as Step 4) — but the newsletter itself is still the complete rollup for the period even for items already pushed out immediately through another channel.

## Step 7: Win/Loss — quantitative research (part 1 of 2)

Source: Lesson 7 (Developing a Competitive Strategy through Win/Loss, part 1).

**Structural constraint, stated before anything else:** this step requires the target company's own CRM (to build the closed-won/closed-lost contact lists) and the ability to actually email that company's real prospects and customers. **Mark N/A for external research** — same category as Lesson 3's Chorus.ai and Lesson 9's displacement campaigns. What follows is the methodology and output format, ready to run the moment this step is done from inside the company rather than about it from outside.

**What it is and why it's the pivot point of the course:** every prior lesson pulled insight from third-party resources or the target's own sales team. This lesson names that as incomplete — the most important resource is prospects and customers directly, because internal materials carry the company's own biased narrative. A win/loss program is the corrective: outsider perspective, and the competitor value props that never surface from the company's own materials.

**Two pillars, this part covers one:** win/loss rests on quantitative and qualitative research. Part 1 (this step) is quantitative only — surveys. Qualitative (interviews) is Step 8.

**What quantitative research is here:** numerical data via survey, split into two tracks — survey closed-lost accounts to learn which competitor they chose and why (the "loss" half), survey closed-won customers to learn why they chose the target (the "win" half).

**Why surveys specifically:** reach (email thousands at once, impossible with interviews) and speed (meaningful response volume within days, faster with an incentive). Best used to quickly test a theory or substantiate a claim about a trend already noticed — not as a first, exploratory pass.

**Tools:** Google Forms for something simple and affordable, but it lacks conditional logic and design flexibility; GetFeedback when either of those is needed.

**Survey design rules:**
1. Cap at 10 questions or fewer, targeting under 5 minutes to complete — a real constraint that forces focus, not just a length limit.
2. Anchor questions to the consideration and decision stages of the buying funnel specifically, not the whole journey. Pull in multiple internal stakeholders when the audience is large, to cover their interests and guarantee engagement with the results later.
3. Add a segmenting question (e.g. company headcount) whenever a cross-segment pattern matters, not just an aggregate result.
4. Test the survey on yourself, then a few colleagues, before it goes live — confirm the flow and the ~5-minute target actually hold.

**Invite email rules:** body under 200 characters regardless of audience. Closed-won: thank them for being a customer, ask plainly to learn from their evaluation process, no incentive by default — they're already in good standing and likely to respond without one. Closed-lost: thank them for evaluating the company (not for being a customer), make the incentive explicit and visible — without it, response rate likely won't be high enough to see a real pattern.

**Output format** (established and confirmed against illustrative/fictional data before use on real data):
1. **Survey design section** — goal, question count/target time, the full question list per track (won and lost), each question's type (multiple choice / open text / segmenting).
2. **Invite email section** — both templates, each under 200 characters, incentive handling stated explicitly per track.
3. **Findings summary section**, written in the same decisive, pattern-first voice as the competitive brief: response rate; why customers chose the target; why lost prospects chose someone else, naming which competitor won each lost deal; any segment pattern found; and — critically — cross-check whether the customer-side hesitation and the lost-prospect objection are actually the same underlying blocker, since that convergence is itself the highest-value finding a win/loss program can produce.

Every number in the output must be either real (pulled from the target's actual CRM/survey platform) or explicitly and repeatedly labeled as illustrative/fictional placeholder data — never presented ambiguously.

## Step 8: Win/Loss — qualitative research (part 2 of 2)

Source: Lesson 8 (Developing a Competitive Strategy through Win/Loss, part 2).

**Structural constraint, same as Step 7:** real interviews require the target's own prospects/customers and contact access. **Mark N/A for external research.** What follows is the confirmed methodology and output format, ready the moment this runs from inside the company.

**What it is and why it's necessary alongside Step 7:** qualitative research here means interviews — non-numerical data, collected because answers in an interview aren't one-word the way a survey response is; they're stories with detail a survey structurally can't capture, and you can go off-script to dig into anything interesting that surfaces. The lesson's own framing: "context is everything."

**The cost, stated honestly:** interviews take real time — target 15-20 minutes each — and need at least 10 *related* interviews (matched on industry, product evaluated, or company size) before any pattern can be trusted. Don't interview "anybody that'll take it" — target the specific segment you actually care about.

**Reuse, don't rebuild:** the interview guide starts from the Step 7 survey's own questions, opened up for follow-up rather than written fresh.

**During the interview:** stay alert to what's actually said over what's scripted — ask the unplanned follow-up, dig into a pause or an odd word choice. This is a skill that improves with repetition; early interviews feeling awkward is expected, not a failure.

**Tools:** a call recorder — Zoom's native recorder is the pragmatic default if the org already uses Zoom; Chorus.ai when transcription accuracy and cross-call keyword playlists matter (e.g. pulling every mention of a specific word across all interviews at once to instantly surface a trend). Calendly for scheduling, to remove the back-and-forth.

**Sourcing — the two gotchas that will silently delay the program if missed:**
1. **Over-invite closed-lost accounts.** They respond at a meaningfully lower rate than closed-won customers — correct for it by inviting more lost accounts than you have interview slots for, don't just accept a smaller lost-side sample.
2. **Timing window.** Reach out within roughly 3 weeks of the deal closing. Beyond that, recall degrades and interviews start producing "I don't really remember." Filter outreach by opportunity-closed date to enforce this.

**Reporting — combine with Step 7's quantitative output, then answer two umbrella questions before presenting anything:**
1. **What needs to happen to act on this?** Name the concrete requirement (a proof point, a feature, a process change), what it would cost, how long it would take, and who owns it — not just the raw finding. The interviews and survey themselves are the bare minimum of a win/loss program; this implication-mapping is what actually makes the output usable.
2. **Who needs to see this?** Identify every stakeholder with a real interest, not just leadership — looping people in late or not at all is named directly as the reason win/loss findings often produce no action at all.

**Output format** (confirmed against illustrative/fictional data before use on real data):
1. **Interview guide** — reused/adapted from the Step 7 survey questions.
2. **Sourcing plan** — target split (e.g. 10 won / 10 lost), the over-invite ratio actually used for closed-lost, and the close-date window applied.
3. **Findings as patterns, not anecdotes** — group repeated language/themes across interviews (cite how many of the total mentioned it), name which competitor won each lost deal, and explicitly cross-check whether a customer-side hesitation and a lost-prospect objection are the same underlying blocker — that convergence is the single highest-confidence finding this step can produce.
4. **Reporting section** — the two umbrella questions answered directly (what would it take to act, who needs to see it), closing with a deliverable that links to the same raw data (survey spreadsheet plus interview transcripts/playlist) everyone reading it can check.

Same rule as Step 7: every fact in the output is either real or explicitly and repeatedly labeled as illustrative/fictional — never ambiguous.

## Suggested next action (after Steps 0-8 are complete): proactive displacement campaign

Source: Lesson 9 (Organizing a Competitive Marketing Campaign). This is **not** a numbered research step — it's a suggested downstream action once the research workflow (Steps 0-8) has produced a confirmed competitive picture. It's fundamentally different in kind from Steps 0-8: those are research and reporting; this is outbound execution, and it requires real company infrastructure — an actual outbound-capable email/CRM setup, consent/compliance handling for cold outreach, and (for the tooling below) a paid contact-enrichment seat. Treat it as a recommendation to bring to whoever owns demand gen/outbound once the research is done, not something this workflow runs itself.

**Known gap in the source lesson, worth stating plainly:** the lesson opens by promising to teach "how to get inside the head of your ideal customer," but never actually delivers a discrete method for that beyond the general targeting logic below — flagging that the promise is thinner than the delivered content, not filling the gap with invented material.

**What it is:** the pivot from reactive competitive intelligence (everything in Steps 0-8) to proactively targeting a competitor's own customer base.

**Before starting:** check whether a competitive campaign already exists at the company — partner with it rather than duplicate it.

**Step 1 — choose the target audience:** either a competitor already reliably beaten (target their existing customer base directly), or a legacy vendor in a market just entered.

**Step 2 — build the contact list, by budget:**
1. Free: CRM opportunity/account notes, if sales reliably fills them in (not guaranteed without a mandatory field); otherwise, LinkedIn engagement on the competitor's own posts as a proxy for "these are their customers."
2. Paid: a contact-enrichment tool (e.g. ZoomInfo's "Reach" extension) to convert LinkedIn engagement into real contact info, or to build a list directly filtered by "technologies installed" (i.e. accounts actually running the competitor's product) — the more scalable version of the same idea. A lower-cost alternative exists per the source lesson but its exact name is garbled in the transcript; don't guess it, verify before recommending a specific tool.

**Step 3 — parallel plays, independent of the email campaign:**
- SEM: branded-keyword bidding on the competitor's name, budget-dependent.
- SEO: comparison-intent landing pages built around what a prospect would actually search to compare the two companies — available regardless of budget.

## Standing rules — apply at every step, not just once at the top

- Never state a company or product fact — mechanics, positioning, competitor status, category — from memory, hedged or not. Verify live, or say "unknown."
- **Never judge a company's proof, customers, or capabilities from its homepage alone.** Read the whole site — Customers, Case Studies, Proof/Results, Product pages, Resources — before concluding anything is missing. A claim that "no proof exists" is only ever valid after those specific pages were actually fetched, never after the homepage was.
- Never accept a company's self-described category as validated market structure without checking it (Step 0).
- Never treat an automated discovery list as final. Always present it for human correction before using it.
- File real outputs into the project's actual directory as they're produced, not just in chat.
- Never ship raw findings without the analysis layer on top. Research produces facts; every artifact this workflow produces (Step 3's brief, Step 4's routing, Step 5's battlecards, Step 6's newsletter) has to add the judgment of what actually matters and why, not just relay what was found — an unfiltered dump of insights onto sales, product, or leadership adds confusion on top of whatever they already had, it doesn't help them. This is the reason Step 6 pulls from full research depth instead of Step 4's compressed table, and the reason every artifact opens with a stated bet — this rule is what those specific instructions are protecting.
