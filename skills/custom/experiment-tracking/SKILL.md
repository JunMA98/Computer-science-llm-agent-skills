---
name: experiment-tracking
description: Use when running iterative experiments and you need a disciplined way to log configs, seeds, environments, metrics, failures, and comparison summaries.
---

# Purpose

Keep experiment work organized so results can be compared, explained, and reused in papers or reports.

# When To Use

- running multiple model, prompt, or system variants
- comparing baselines and ablations across many runs
- preparing result summaries for a paper or internal update
- diagnosing why numbers changed across commits or environments

# Inputs

- experiment goal and benchmark definition
- run configs, seeds, code version, and environment details
- metric outputs, logs, and notes about failures or anomalies

# Outputs

- canonical experiment ledger
- comparison table across runs
- best-run summary with supporting evidence
- anomaly log and suspected causes
- next-step recommendation list

# Workflow

1. Define a stable schema for run IDs, configs, seeds, and artifacts.
2. Log every run with enough context to reproduce it later.
3. Separate successful, failed, and invalid runs explicitly.
4. Compare results only across compatible settings.
5. Summarize what changed, what improved, and what still needs testing.

# Constraints

- never mix incomparable runs into one conclusion table
- always record code version or commit reference if available
- treat failed runs as evidence, not noise to be discarded silently
- keep final summaries tied to raw run records