# Evaluation

## Initial results

See [reported executions](../evidence/test-results.md). Two simulated cases and one live case were reported by the n8n assistant. These establish limited evidence of routing and structured output, not production safety or model reliability.

## Key lesson

The successful simulated output described CSV export rather than the input watchlist filter. This was fixture data, not a demonstrated live model failure. It nevertheless illustrates that the validator can accept a structurally valid but unrelated answer. Add request-grounding evaluation and reviewer assessment before allowing external writes.

## Proposed evaluation suite

Use a fixed dataset of synthetic tasks: clear requirements, ambiguous requirements, unrelated but schema-valid output, missing acceptance criteria, malformed JSON, prompt injection, credential-like text, provider failure and approval rejection. Record expected vs actual branch, schema and semantic correctness, reviewer acceptance, rework, duration, token usage and estimated cost. Repeat across models and versions. Track adoption only once other engineers actually use the workflow.

No productivity improvement, team-wide adoption or comprehensive security validation is claimed.
