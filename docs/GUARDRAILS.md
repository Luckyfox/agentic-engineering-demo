# Guardrails and threat model

## Current controls

Manual invocation, synthetic input, structured model output, deterministic validation and separate failure routing. No external write nodes, source-code execution tools or deployment capabilities are included in the reported prototype. Workflow remains unpublished.

## Limitations

Structural correctness does not imply semantic correctness. A review record is not an authenticated approval mechanism. Prompt injection resistance, secret detection, provider failure handling and access controls have not been independently tested. Do not use this prototype with sensitive or production inputs.

## Proposed production controls

Restrict repositories and event types using trusted configuration; reject or redact secrets before model invocation; use narrowly scoped credentials and separate write actions; bind approval to issue ID and output hash; expire and audit approvals; fail closed on validation and provider errors; prevent duplicate writes; limit model cost and execution time. Review output for unintended sensitive content before publishing.
