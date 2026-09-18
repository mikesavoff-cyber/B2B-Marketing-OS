# B2B Marketing OS

Multi-function B2B marketing operating system: one agent per marketing function (orchestrator + five leads), skills that perform individual jobs, workflows that sequence them, and a knowledge base of practitioner methodology (course transcripts, frameworks, workbooks) that every decision must be grounded in — not generic model knowledge.

## Architecture

- `agents/` — six function agents. `b2b-marketing-director` receives every request first, routes, sequences, and enforces gates. The five leads (`product-marketing-lead`, `gtm-lead`, `growth-lead`, `content-lead`, `demand-gen-lead`) own their lanes and produce the artifacts. Each agent file carries its own lane, grounding pointers, skill list, and output contract.
- `Skills/` — focused capabilities, invoked when a request matches a skill's description. The `description` frontmatter is the entire routing gate: written in the language of requests, not internal jargon. (Currently flat under `Skills/PMM/`; a per-function layout is planned.)
- `Workflows/` — sequences of jobs (e.g. `pmm-strategy-foundation`).
- Knowledge base at repo root, one folder per function: `Product Marketing/`, `Growth/`, `GTM/`, `Content Strategy/`, `B2B Content Funnels/`. Each folder's `_INDEX.md` is the retrieval entry point. Demand Gen has no knowledge folder yet — flag gaps, never invent methodology.

## Grounding (progressive disclosure)

Context loads in tiers; load the next tier only when the current one proves it needed.

- Before any task: the director reads `CLAUDE.md` and the `_INDEX.md` of every knowledge folder the task touches.
- An agent never batch-reads a knowledge folder. Read the folder's `_INDEX.md`, select files by the "Read when" column, read only those.
- Skills hardcode the paths they always need in their own Grounding sections. Anything outside their lane goes through the folder index.
- If the index doesn't cover a topic, `grep` the folder before concluding the knowledge doesn't exist. "Not in the index" is not "doesn't exist."
- When a run discovers knowledge the index's "Read when" column would not have surfaced, update the index in the same session.

## Knowledge vs. project state

- Knowledge (the root folders) is static methodology, shared across projects.
- Project state is the approved outputs of prior steps for one company/project (e.g. `Artifacts/<company>/` or its Notion tree).
- Later steps consume approved artifacts, not just methodology. A missing required artifact is a gate: the prior step hasn't run or been approved. Surface it; do not work around it.

## Execution rules

- Product Marketing outputs gate every downstream function. GTM, Growth, Content, and Demand Gen build on approved PM artifacts for that project — they never re-derive positioning, messaging, or ICP.
- Do not assume the full PM sequence must run end to end. Ask which step or sequence is needed; propose before executing; confirm with Mike before running.
- Human-in-the-loop at almost every step. When a request arrives: understand, surface the relevant agents/skills/workflows, propose an approach, wait for confirmation, then execute one step at a time with validation between steps.
- Follow the agent's lane boundary. Do not duplicate another function's responsibility; consume its approved output instead.
- Do not skip required upstream dependencies, and do not reconstruct missing upstream outputs from assumptions.
- A job is complete only when the required output artifact exists and satisfies its skill's completion requirements — never because a skill was invoked.
- Strategic judgment calls (positioning direction, which threat is real, which segment first) are Mike's: present evidence and competing readings when he is present; mark **[Hypothesis]** when he is not. Never present a strategic guess as settled.

## Output expectations

Every artifact must take a stance (open with the bet, not a survey), name concrete triggers and consequences, state its confidence once at the top (observed / company-claimed / agent judgment) and then stop labeling, and be usable by its downstream consumer without re-doing the research. Strategic artifacts are written in persuasive voice; executable hand-offs (runbooks, scripts, briefs, checklists) in plain voice: one meaning per word, one idea per sentence, 20 words or fewer for instructions. Every artifact ends with open questions and what it hands to the next step. When output is rejected, the fix goes into the skill or agent file, not just the artifact.
