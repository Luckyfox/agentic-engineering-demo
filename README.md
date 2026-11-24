# ACDC – Agentic Engineering Pipeline

A small independent proof of concept inspired by n8n's Agent-centric Development Cycle, built while exploring the Staff Platform Engineer, Agentic Engineering role.

## What it does

A manually triggered synthetic feature request is analysed by an LLM, checked by deterministic validation, and routed to either a pending human review record or a validation failure record.

The prototype is an unpublished n8n Cloud workflow. It does not write to GitHub, change source code or deploy software. A pending review record is not an implemented human approval gate.

## Evidence so far (24 November 2026)

The n8n assistant reported two simulated routing tests and one live model execution (~14 seconds). The live response contained six requirements, nine acceptance criteria, eight open questions and four risks. The negative test correctly rejected an empty acceptance-criteria list. These results have not been independently audited against raw execution logs.

## Documentation

- [Specification](docs/SPECIFICATION.md)
- [Architecture](docs/ARCHITECTURE.md)
- [Guardrails](docs/GUARDRAILS.md)
- [Evaluation](docs/EVALUATION.md)
- [Agent instructions](AGENTS.md)
- [Reported test results](evidence/test-results.md)

## Reproduction status

The original workflow export and screenshot are pending. This repository currently documents the prototype; it is not yet a runnable distribution. No credentials, private repositories or customer data are included.

## Next steps

Export and inspect the genuine workflow JSON; add sanitized execution evidence; introduce semantic checks and authenticated approval; then add scoped GitHub integration and repeatable evaluation fixtures. No team-wide adoption or productivity improvement is claimed.
