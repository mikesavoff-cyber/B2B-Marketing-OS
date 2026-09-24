---
name: buyer-personas
description: >-
  Build buyer personas from real buyer research: the five rings of buying
  insights, the buying committee, an interview plan and guide, and a buyer
  profile with quotes. Use whenever the task involves "buyer personas," "build
  our personas," "who is the buyer," "persona research," "buyer interviews,"
  "interview guide," "buying committee," "what does the buyer care about,"
  "decision criteria," "perceived barriers," or "persona for [role]." Also
  turns personas into messaging inputs, barrier-busting content, product gaps,
  and sales-enablement material when asked. Feeds messaging, content, and
  sales enablement. Built from the Segmentation and Persona Research course
  in `Product Marketing/Segmentation & Persona Research/`.
allowed-tools: Read Write Edit Bash WebSearch WebFetch
metadata:
  version: 1.0.0
---

# Buyer Personas

A buyer persona is "a detailed archetype of someone who represents your perfect customer, and these
are based on insights and research" (*Buyer Personas*). "It's not hypotheses about what your
customers may want... It's actually doing the work of going and asking the questions" (*Course
Introduction*).

## Inputs

- **`icp-definition` output** (`competitor-profiles/<company>-icp-<date>.md`). It names the
  prioritized segment and its buying roles. Personas are built for those roles. "A customer segment
  is a portion of your market... a persona is the people that might make up that segment."
- **`competitor-research` output.** It supplies the alternatives buyers compare, which feed
  Decision Criteria and Perceived Barriers.
- **Access level.** Can we interview real buyers, or is this arm's-length research? This decides
  the mode (Process below).

## Buyer persona vs. user persona

"A buyer persona is really focused on that presale behavior... what gets them to actually get over
the buying hurdle." "A user persona is somebody after the sales cycle." This skill builds **buyer**
personas. Say so if the request is really about users.

## The five rings of buying insights

The core of every persona (*Buyer Personas*, from Adele Revella's *Buyer Personas*):

1. **Priority initiatives:** why they'd buy anything at all. "This isn't about your product. It's
   about the customer absent of your product."
2. **Success factors:** the tangible and intangible rewards they expect, at both the
   organizational and personal level ("everyone will see me as a strategic force").
3. **Perceived barriers:** why they wouldn't see you as the best option.
4. **Buyer's journey:** the steps and information they need to decide.
5. **Decision criteria:** what they use to evaluate options, and why. Peer recommendations are
   "one of the most common."

"Keep drilling in on this idea of why." Details and examples: `references/methodology.md`.

## Buying committee

In B2B, "a purchasing decision isn't made by any one person":
- **Economic buyer:** funds the purchase
- **User buyer:** uses it daily
- **Technical buyer:** evaluates specs and regulations
- **Coach or champion:** "they want to see you win"

"One person might play multiple roles." Build one profile per distinct role.

## Process: six steps

From *Building Personas*. Full detail: `references/methodology.md`.

1. **Pick the interviewer.** Neutral, not sales: "the buyer immediately opens up, because they know
   they're not about to be sold to." Pick someone intellectually curious.
2. **Pick who to interview.** Existing customers, past customers, pipeline, and especially "people
   that our business is not actively talking to."
3. **Design the questions.** Frame them as a story. Use a "structured and repeatable survey
   template" mapped to the five rings. Drill into the specific information sources they use.
4. **Conduct the interview.** Record it, research the person first, and tell them why you're
   doing it. Stay curious and use open-ended questions.
5. **Process the findings.** Mark each transcript against the five rings and pull the quotes.
6. **Present** as a buyer profile: a top-considerations list per ring, with key quotes.

**Mindset:** operate "with a cynic's mindset... assume they don't want to buy it." And "don't let
perfect be the enemy of good": "only 44% of companies... have buyer personas clearly defined."

**Numbers:**
- 8-10 interviews per persona
- ask "why" up to three times on key points
- avoid yes/no questions
- refresh at least every 12 months, plus 1-2 ongoing interviews a month

### Two modes

- **Interview mode** (buyer access exists): run all six steps. Profiles are built from real quotes.
- **Preliminary mode** (arm's-length research, no buyer access): the course's own first step is to
  "create a preliminary buyer persona based on... past experiences" and then "validate or
  invalidate the assumptions." Build the five rings from public buyer voice:
  - review text on G2, TrustRadius, and Capterra
  - community threads
  - the company's case studies
  - job posts for the role

  Quote the source for each point. Label the whole profile **[Hypothesis]** and attach the
  interview plan and guide that would validate it. Never write an invented quote as if a buyer
  said it.

## Output

One file: `competitor-profiles/<company>-buyer-personas-<YYYY-MM-DD>.md`. Templates:
`references/templates.md`.

1. **The call.** One sentence naming the persona that matters most to win, and why.
2. **Buying committee map** for the prioritized segment.
3. **One buyer profile per role:** basics, plus the five rings, each with its top considerations
   and a supporting quote and source.
4. **Interview plan and guide:** who interviews, who gets interviewed, the questions, and the
   timeline. Always included in preliminary mode.
5. **Open questions**, each naming the evidence that would resolve it.
6. **Hands off to:** messaging (the needs × capabilities × proof input table), content, and sales
   enablement.

**Only when asked**, apply the personas (*Bringing it All Together*): a message map,
barrier-busting content, product gaps, and a sales playbook with challenge questions. Methods are in
`references/methodology.md` → *Applying personas*. Don't produce these by default.

## Constraints

- Every point in a ring cites a source: an interview transcript, a review, a thread, a case study, or
  a job post. No source means cut the point, or mark it **[Hypothesis]**.
- Never present a paraphrase or invented line as a buyer quote. Real quotes only, with attribution.
- Sales never runs the interviews ("don't have the sales team conduct the interviews").
- Messaging drawn from personas should rest on the first four rings. "The buyer's journey is more
  the role of your go-to-market motion, as opposed to your messaging."
- A persona is one role inside one segment, never "our customers" in general.

## Grounding

`Product Marketing/Segmentation & Persona Research/`: *Buyer Personas*, *Building Personas*,
*Bringing it All Together*, and *Course Introduction & Overview*.

## Related skills

- `competitor-research`: supplies the alternatives buyers compare.
- `icp-definition`: runs first. Names the segment and buying roles to build personas for.
- `market-segmentation`: the segment each persona sits inside.
- `account-scoring`: uses the same buying roles to pick contacts inside scored accounts.
