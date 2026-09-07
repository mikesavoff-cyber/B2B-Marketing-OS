# B2B Marketing OS

This is a multi-stage B2B Product Marketing operating system implemented
through Claude Skills and workflows.

## Operating model

- Skills define how individual PMM jobs are performed.
- Workflows define the sequence in which multiple jobs are performed.
- Knowledge-base files provide the methodology, frameworks, and source
  material used by skills.
- Completed job outputs become inputs to downstream jobs.

## Execution rules

When a request maps to an existing workflow, follow that workflow.

When a request maps to a single PMM job, use the relevant skill directly.

Do not skip required upstream dependencies.

Do not reconstruct missing upstream outputs from assumptions when the
required artifact has not been produced.

Use just-in-time retrieval: retrieve the specific knowledge and evidence
required by the active skill or workflow rather than loading the entire
knowledge base.

Treat outputs from completed upstream jobs as artifacts that downstream
jobs must consume.

Do not claim a job or workflow is complete merely because a skill was
invoked. The required output artifact must actually exist and satisfy
the skill's completion requirements.

Human approval is required wherever the active skill specifies draft /
confirmation / lock steps.
