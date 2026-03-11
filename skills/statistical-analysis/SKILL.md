---
name: statistical-analysis
description: Choose and report statistical analyses for CS experiments, benchmarks, user studies, and offline evaluations. Use when selecting tests, checking assumptions, comparing multiple runs or seeds, estimating uncertainty, reporting effect sizes, or deciding whether differences in results are credible.
---

# Statistical Analysis

Use this skill for analysis planning and result interpretation in computing experiments.

## Common CS Cases

- compare models across multiple seeds
- assess whether an ablation difference is meaningful
- analyze benchmark subsets or error slices
- evaluate user-study outcomes in HCI or interactive systems
- report uncertainty for retrieval, ranking, generation, or systems metrics
- choose between parametric, nonparametric, permutation, bootstrap, or Bayesian approaches

## Workflow

1. Define the unit of analysis correctly.
2. Check whether samples are paired, repeated, hierarchical, or independent.
3. Choose tests that match the design and metric distribution.
4. Report uncertainty and effect size, not only p-values.
5. State what the analysis does and does not justify.

## Local Resources

- `references/test_selection_guide.md`
- `references/assumptions_and_diagnostics.md`
- `references/effect_sizes_and_power.md`
- `references/reporting_standards.md`
- `references/bayesian_statistics.md`
- `scripts/assumption_checks.py`

## CS-Specific Rules

- Prefer paired analyses when systems are evaluated on the same items.
- Treat multi-seed results as repeated measurements, not independent benchmarks.
- Report variance and confidence intervals when benchmark scores are unstable.
- Use bootstrap or permutation methods when classical assumptions are weak.
- Do not reuse APA-style prose as the default; write for technical readers.

## Default Output

When the user asks for statistical guidance without a required format, return:
1. recommended analysis plan
2. assumptions to verify
3. what to report in the paper or report
4. caveats that limit interpretation