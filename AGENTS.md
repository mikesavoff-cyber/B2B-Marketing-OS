# PMM OS — Agent System Standard

## Purpose

PMM OS is an agentic product-marketing operating system. It separates knowledge, context, skills, agents, workflows, and human decisions so the system can perform research-heavy and procedural PMM work without turning strategic judgment into autonomous prompt output.

## Core architecture

- `knowledge/` — canonical PMM knowledge and source material. Knowledge is reusable across disciplines and should not be duplicated merely because multiple agents use it.
- `context/` — company/product/customer/market/competitive reality for a specific operating environment.
- `agents/` — reasoning roles that perform a PMM job using skills, knowledge, context, evidence, and tools.
- `workflows/` — orchestration of multiple agents and human decision gates for end-to-end PMM projects.
- `evaluations/` — tests that verify agents and skills continue to behave correctly as the system evolves.
- `integrations/` — connectors to external systems and live evidence sources.
- `scripts/` — ingestion, normalization, indexing, validation, and other automation.
- `schemas/` — shared structured output contracts.

## Skill standard

A skill is an executable operating procedure, not a persona prompt. Every production skill should specify:

1. Purpose
2. Activation / trigger conditions
3. Non-trigger conditions
4. Required inputs
5. Optional inputs
6. Evidence and knowledge retrieval requirements
7. Procedure / sequence
8. Decision points
9. Human decision gates
10. Failure / stop conditions
11. Escalation rules
12. Expected outputs
13. Evaluation criteria
14. Examples or test cases where useful

A skill should tell an agent **how to perform the job**. It should not become a dumping ground for the PMM corpus.

## Knowledge standard

Knowledge documents should be source-aware and reusable across disciplines. Prefer metadata such as:

- `id`
- `title`
- `disciplines`
- `concepts`
- `sources`
- `type`
- `confidence`

Keep source material separate from synthesized concepts when practical. Preserve provenance so agents can distinguish expert/framework knowledge from company evidence and live market signals.

## Evidence hierarchy

Agents must distinguish:

- facts
- observed evidence
- hypotheses
- assumptions
- recommendations

Never silently turn an assumption into product, customer, market, or competitive truth.

## Human judgment

PMM OS should automate information gathering, synthesis, monitoring, pattern detection, first-pass analysis, option generation, documentation, coordination, QA, and repetitive execution where appropriate.

Strategic positioning, narrative choices, major tradeoffs, and high-consequence external actions should have explicit human decision gates unless a workflow deliberately defines otherwise.

## Output discipline

Agents should prefer structured, inspectable outputs over opaque prose. Outputs should make evidence, confidence, assumptions, unresolved questions, risks, and required human decisions visible.

## Changes to this system

Before adding an agent, ask whether the capability belongs in an existing skill or workflow. Avoid creating overlapping agents with slightly different prompts.

Before adding a new knowledge document, check whether the concept already exists. Avoid duplicating the same concept across discipline folders; use metadata to associate reusable knowledge with multiple disciplines.

All production changes should be testable through `evaluations/` where feasible.
