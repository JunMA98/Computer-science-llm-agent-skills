---
name: repo-cleanup
description: Use when a research or prototype repository has become messy and you need a disciplined cleanup plan for structure, naming, docs, unused files, configs, and reproducibility hygiene.
---

# Purpose

Improve repository clarity so code, experiments, and documents are easier to understand and maintain.

# When To Use

- before public release or collaborator handoff
- after a rapid prototyping phase left the repo inconsistent
- when folders, scripts, and outputs have become hard to navigate
- when experiment artifacts and source code are mixed carelessly

# Inputs

- repository layout and current file structure
- known pain points, stale outputs, and documentation gaps
- any constraints about files that must not be touched

# Outputs

- cleanup plan ordered by safety and impact
- proposed directory and naming normalization
- list of stale, duplicated, or misplaced files
- documentation gaps and configuration hygiene fixes
- explicit separation of safe cleanup versus risky cleanup

# Workflow

1. Inspect the repo structure before proposing moves.
2. Identify clutter, ambiguity, and unsafe mixing of source and generated outputs.
3. Group cleanup work into structure, naming, docs, configs, and artifacts.
4. Separate non-destructive cleanup from anything that needs confirmation.
5. Produce a minimal end state that is easier to release and maintain.

# Constraints

- do not assume generated files are disposable without checking
- separate cleanup suggestions from destructive actions
- preserve provenance for experiment outputs that may still matter
- favor clear structure over cosmetic churn