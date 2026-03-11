---
name: benchmark-design
description: Use when designing an evaluation plan for a CS, ML, or agent project and you need to choose datasets, baselines, metrics, ablations, compute budgets, and reporting rules.
---

# Purpose

Design a benchmark that is fair, reproducible, and aligned with the paper or project claim.

# When To Use

- defining a new evaluation protocol for a paper or prototype
- choosing baselines, metrics, and data splits
- planning ablations and error analysis before running experiments
- checking whether reported claims are actually testable

# Inputs

- task definition and target claims
- candidate datasets, models, or systems
- compute budget, runtime limits, and hardware constraints
- prior papers or existing benchmark conventions if available

# Outputs

- benchmark matrix of tasks, datasets, metrics, and baselines
- evaluation protocol and run rules
- ablation plan and error-analysis checklist
- reporting template for tables and plots
- risk notes about confounders or unfair comparisons

# Workflow

1. Translate the project claim into measurable questions.
2. Select datasets and splits that match the intended claim.
3. Define baseline tiers: trivial, standard, and strong reference systems.
4. Choose primary and secondary metrics, then add ablations and sanity checks.
5. Record compute, prompt, seed, and implementation fairness rules.

# Constraints

- do not compare systems under hidden budget mismatches
- avoid metric choices that only flatter the proposed method
- separate headline metrics from diagnostic metrics
- make ablations answer specific causal questions, not random variations