---
name: code-to-paper
description: Use when turning an existing codebase, experiment set, or system into a paper plan and you need contribution framing, evidence mapping, figure planning, and missing-experiment detection.
---

# Purpose

Translate implemented work into a paper-ready argument with clear claims and supporting evidence.

# When To Use

- writing a paper from an already-working repo or prototype
- deciding whether current code and results are strong enough for submission
- mapping experiments and artifacts into sections, tables, and figures
- finding missing evidence before drafting a paper around the work

# Inputs

- codebase structure and current system behavior
- experiment logs, result tables, figures, or demos
- target venue or paper type if known

# Outputs

- contribution framing and paper outline
- claim-to-evidence map
- figure and table plan
- list of missing experiments, baselines, or ablations
- recommended paper scope for the current evidence level

# Workflow

1. Identify what the code actually demonstrates today.
2. Convert implemented capabilities into candidate claims.
3. Match each claim to evidence, tables, figures, or missing experiments.
4. Build an outline around the strongest supported narrative.
5. Flag overclaims and scope the paper to what can be defended.

# Constraints

- do not inflate implementation work into unsupported novelty claims
- prefer narrower defensible contributions over broad weak stories
- separate evidence already available from evidence still needed
- make missing baselines and ablations explicit before drafting aggressively