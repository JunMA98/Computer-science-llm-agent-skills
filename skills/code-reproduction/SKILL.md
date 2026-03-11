---
name: code-reproduction
description: Use when reproducing a paper, repo, benchmark, or reported result and you need an explicit plan for environment setup, execution, discrepancy logging, and final reproduction status.
---

# Purpose

Reproduce reported results without overstating success and without losing track of discrepancies.

# When To Use

- implementing or rerunning a paper's released code
- checking whether a baseline can be reproduced before extending it
- validating a public repo before building new work on top of it
- preparing an artifact report or reproducibility note

# Inputs

- target paper, repo, or benchmark claim
- environment requirements and hardware constraints
- available scripts, checkpoints, configs, and datasets

# Outputs

- reproduction plan and execution order
- environment summary and setup log
- discrepancy report between expected and observed behavior
- reproduction status: exact, partial, failed, or blocked
- list of missing assumptions or undocumented steps

# Workflow

1. Extract the exact claims to reproduce before running anything.
2. Reconstruct the environment and document every assumption.
3. Run the minimum viable path first, then expand to full results.
4. Compare observed outputs against reported numbers or behaviors.
5. Log mismatches with likely causes instead of hiding them.

# Constraints

- distinguish exact replication from faithful reimplementation
- never claim success without a concrete comparison target
- treat undocumented setup steps as findings, not personal fixes
- keep a clear boundary between upstream behavior and your modifications