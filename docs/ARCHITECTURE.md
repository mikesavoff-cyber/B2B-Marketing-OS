# PMM OS Architecture

## The system

```text
                    PMM OS
                       │
        ┌──────────────┼──────────────┐
    KNOWLEDGE       CONTEXT         SIGNALS
        └──────────────┼──────────────┘
                       ▼
                     SKILLS
                       ▼
                     AGENTS
                       ▼
                   WORKFLOWS
                       ▼
                 HUMAN PMM
                       ▼
                  EXECUTION
                       ▼
                  MEASUREMENT
                       │
                       └── learning/evidence ──► system
```

**Knowledge** = accumulated PMM expertise: frameworks, concepts, methods, examples and synthesized perspectives.

**Context** = company/product/customer/market/competitive reality, strategy, roadmap, constraints and project state.

**Signals** = live evidence from analytics, CRM, customer calls, support, web research and competitor monitoring. Signals are evidence sources, not static knowledge.

**Skills** = procedures for performing specific PMM jobs.

**Agents** = reasoning roles that apply skills to knowledge, context, evidence and tools.

**Workflows** = orchestrated sequences of agents and human gates for end-to-end PMM outcomes.

## First vertical slice

```text
New Product Launch → Intake → Product Truth →
Market + Customer + Competitive Research → ICP →
Positioning → Value Proposition → Messaging → Narrative →
GTM → Launch → Activation/Enablement/Demand/Product/CS →
Measurement → Learning
```

First capabilities: Research Agent, Positioning Agent, GTM/Launch Orchestrator.

## Retrieval architecture

Canonical knowledge can live as Markdown/JSON in GitHub, but GitHub is not the retrieval database itself:

```text
Knowledge files → ingestion/normalization → metadata + chunks + indexing → search/retrieval → agents
```

Start with full-text/semantic retrieval and metadata filtering. Add more infrastructure only when a demonstrated use case requires it.

## Source-aware reasoning

Agents retain provenance and should surface conflicts between expert perspectives rather than invent consensus. Outputs should distinguish evidence, facts, hypotheses, assumptions, recommendations, risks, unresolved questions, confidence and human decisions.

## Autonomy boundary

The system should increasingly own research, synthesis, monitoring, evidence organization, first-pass analysis, option generation, documentation, coordination, QA, measurement and repetitive execution. The human PMM remains the decision-maker for strategic choices, positioning, narrative, material tradeoffs and high-consequence external actions unless explicitly delegated.
