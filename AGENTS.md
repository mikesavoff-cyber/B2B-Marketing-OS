# PMM OS — Agent System Standard

PMM OS is an agentic product-marketing operating system. It separates knowledge, context, skills, agents, workflows, and human decisions.

## Core architecture
- `knowledge/` — canonical PMM knowledge and source material; reusable across disciplines.
- `context/` — company/product/customer/market/competitive reality.
- `agents/` — reasoning roles that apply skills to knowledge, context, evidence, and tools.
- `workflows/` — orchestration of agents and explicit human decision gates.
- `evaluations/` — tests for skills and agents.
- `integrations/` — external systems and live evidence sources.
- `scripts/` — ingestion, normalization, indexing, validation, automation.
- `schemas/` — structured output contracts.

## Skill standard
A skill is an executable operating procedure, not a persona prompt. Production skills should specify purpose, activation/non-activation conditions, required/optional inputs, evidence and retrieval requirements, procedure, decision points, human gates, failure conditions, escalation rules, outputs, and evaluation criteria.

A skill tells an agent **how to perform the job**. It should not become a dumping ground for the PMM corpus.

## Knowledge standard
Knowledge documents should be source-aware and reusable across disciplines. Prefer metadata including `id`, `title`, `disciplines`, `concepts`, `sources`, `type`, and `confidence`. Preserve provenance so agents can distinguish expert/framework knowledge from company evidence and live market signals.

## Evidence
Agents must distinguish facts, observed evidence, hypotheses, assumptions, and recommendations. Never silently turn an assumption into product, customer, market, or competitive truth.

## Human judgment
Automate research, synthesis, monitoring, evidence organization, first-pass analysis, option generation, documentation, coordination, QA, measurement, and repetitive execution where appropriate. Strategic positioning, narrative choices, material tradeoffs, and high-consequence external actions require explicit human decision gates unless a workflow deliberately defines otherwise.

## Change discipline
Before adding an agent, ask whether the capability belongs in an existing skill or workflow. Before adding knowledge, check whether the concept already exists. Avoid duplicating concepts across discipline folders; use metadata to associate reusable knowledge with multiple disciplines. Production changes should be testable through `evaluations/` where feasible.
