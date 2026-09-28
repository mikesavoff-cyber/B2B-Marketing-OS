# Retrieval protocol

How to get methodology out of the knowledge base for a decision. Adapted from the GTM Playbook
source-of-truth protocol Mike approved in ChatGPT (2026-09-27): full corpus → retrieval layer →
reasoning → synthesis. Never compress the corpus into a summary and reason from the summary.

## The order

1. **Name the decision first.** Write the question the step must answer ("which comparator do we
   fight?"), not a keyword. Don't pick a framework from the request's wording.
2. **Open `methodology-map.md`.** Find every source and section that owns this decision, across
   all layers. Don't stop at the first match.
3. **Read the actual section.** Open the file and read the section itself. Never rely on a title,
   the index, this skill's summaries, or model memory.
4. **Read the whole methodology unit.** Beyond the headline framework, take its purpose, when to
   use it, assumptions, steps, criteria, examples, anti-patterns, validation, and what comes
   before and after. Skip only clear boilerplate.
5. **Follow dependencies.** If the source says it depends on or feeds another source, read that
   one too, and keep the order the sources set. A validation method is not a competing framework.
6. **Classify overlaps.** When two sources answer the same decision, name their relationship
   (layers and relationship types are in `methodology-map.md`). Check `conflicts.md`. If they
   disagree and no ruling exists, show Mike both readings.
7. **Pick the smallest set.** One primary method per decision, plus a supporting one only when it
   adds what the primary can't. Say why. Don't merge distinct methods into one invented framework.
8. **Apply, then label.** Every statement in the working notes is one of:
   - **Source:** what the file says, with file and section.
   - **Application:** how that method applies to this company.
   - **Synthesis:** a combination of sources whose relationship requires it.
   - **Judgment:** this agent's call.

## Source priority

1. Files in `Product Marketing/Positioning/`, read in this session.
2. Other repo KB files the map points to (MKT1 Complete, `ICP and Personas/`, `Messaging/`).
3. Rulings in `conflicts.md` (Mike's decisions override source defaults).
4. General model knowledge, only where the sources are silent, labeled judgment.

Model knowledge never silently overwrites a source. Never attribute a framework to an author the
repo doesn't hold.

## Fidelity rules

- Keep the sources' distinctions: positioning vs. messaging, ICP vs. persona, category strategy
  vs. category name, research vs. validation, statement vs. story vs. tagline.
- Don't simplify away a distinction to make the output shorter. The constitution is short because
  it holds decisions, not because methods were blurred.
- If a needed file can't be read, say so. Never claim a source was read when it wasn't.

## Gotchas

- `The MKT1 Guide to positioning.md` is the primary MKT1 source (Steps 1-4). `MKT1 - Complete
  Marketing Framework.md` §4 is a summary of it; cite the guide.
- The Dunford and Fletch files are syntheses. Their own section numbers are what you cite.
- Fletch §2, §4, §5, §7, §8, §12 are messaging methods. Read them only as downstream context.
- Dell's lessons are transcripts. Quote exact lines when a rule decides a call; paraphrase drifts.
