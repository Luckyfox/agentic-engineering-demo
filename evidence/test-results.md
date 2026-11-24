# Reported execution evidence — 24 November 2026

Source: n8n assistant conversation in the demonstration workspace. Raw execution logs have not been independently inspected.

| Execution | Mode | Input/output condition | Reported result |
|---|---|---|---|
| 1 | Simulated model output | Structurally valid sample about CSV export | Passed schema validation; pending_human_approval |
| 2 | Simulated model output | Empty acceptance_criteria | Rejected; validation_failed |
| 3 | Live model | Synthetic watchlist filtering request FR-1042 | Passed; pending_human_approval; about 14 seconds |

Live model reported: gpt-6.1-terra via built-in AI credits. Output: six requirements, nine acceptance criteria, eight open questions and four risks. No external writes were reported. The workflow remained unpublished.

The simulated pass fixture did not match the source feature request. This limits the evidence of semantic correctness and motivates a future grounding check. The actual workflow export and screenshot are not yet committed.
