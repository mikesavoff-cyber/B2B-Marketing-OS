# PMM OS Architecture

## The system

PMM OS separates six concerns:

```text
                    PMM OS
                       │
        ┌──────────────┼──────────────┐
        │              │              │
    KNOWLEDGE       CONTEXT         SIGNALS
        │              │              │
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

### Knowledge

Accumulated PMM expertise: frameworks, concepts, methods, examples, source material, and synthesized perspectives. It should be reusable across disciplines.

### Context

The reality the PMM is operating in: company, product, customers, market, competitors, commercial constraints, strategy, roadmap, and project state.

### Signals

Live evidence from systems such as analytics, CRM, customer calls, support, web research, and competitor monitoring. Signals are evidence sources, not static knowledge.

### Skills

Procedures for performing specific PMM jobs. A skill defines activation criteria, inputs, retrieval needs, steps, decision points, failure conditions, escalation, and outputs.

### Agents

Reasoning roles that apply skills to knowledge, context, evidence, and tools. An agent is not synonymous with a skill.

### Workflows

Orchestrated sequences of agents and human gates that accomplish an end-to-end PMM outcome, such as a product launch or repositioning.

## First vertical slice

The initial implementation should prove one complete path rather than attempting to build the entire PMM suite at once:

```text
New Product Launch
        ↓
Project Intake
        ↓
Product Truth
        ↓
Market + Customer + Competitive Research
        ↓
ICP
        ↓
Positioning
        ↓
Value Proposition
        ↓
Messaging
        ↓
Narrative
        ↓
GTM
        ↓
Launch
        ↓
Activation / Enablement / Demand / Product / CS
        ↓
Measurement
        ↓
Learning
```

The first production capabilities should therefore be:

1. Research Agent
2. Positioning Agent
3. GTM / Launch Orchestrator

These should be built against the shared skill standard in `AGENTS.md` and accompanied by evaluations.

## Retrieval architecture

The canonical corpus may live as Markdown/JSON in GitHub, but GitHub should not be treated as the retrieval database itself.

The intended path is:

```text
Canonical knowledge files
        ↓
Ingestion / normalization
        ↓
Metadata + chunks + indexing
        ↓
Search / retrieval
        ↓
Agents
```

Start with the simplest retrieval layer that supports full-text search, semantic retrieval, and metadata filtering. Introduce a more sophisticated knowledge graph or infrastructure only when a demonstrated use case requires it.

## Source-aware reasoning

Agents should retain provenance internally. When expert perspectives conflict, surface the conflict rather than collapsing it into false consensus.

A useful output pattern is:

```text
Evidence
Facts
Hypotheses
Assumptions
Expert perspectives
Conflicts
Recommendation
Risks
Unresolved questions
Human decision required
```

## Autonomy boundary

The system should increasingly own research, synthesis, monitoring, evidence organization, first-pass analysis, option generation, documentation, coordination, QA, measurement, and repetitive execution.

The human PMM remains the decision-maker for strategic choices, positioning judgment, narrative judgment, material tradeoffs, and high-consequence external actions unless a workflow explicitly establishes another approval policy.
