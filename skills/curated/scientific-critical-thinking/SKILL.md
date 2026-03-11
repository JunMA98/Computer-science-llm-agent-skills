---
name: scientific-critical-thinking
description: Critically examine claims, assumptions, evidence, and argument quality in computer science papers, experiments, benchmark plans, and technical proposals. Use when stress-testing a research idea, detecting confounders, checking causal leaps, or identifying missing controls before writing, reviewing, or implementing.
---

# Scientific Critical Thinking

Use this skill to pressure-test research reasoning in computer science. The goal is not skepticism for its own sake; the goal is to find where the evidence chain is weak and how to strengthen it.

## Default Lens

For any claim, ask:
- what exactly is being claimed
- what evidence is offered
- what assumptions are required for the claim to hold
- what plausible alternative explanations remain
- what evidence would actually falsify the claim

This lens works for papers, experiment plans, benchmark designs, and internal research proposals.

## CS-Specific Checks

### Problem formulation
- Is the task or threat model defined precisely?
- Is the scope realistic or selectively simplified?
- Are important constraints hidden in preprocessing, oracle information, or infrastructure assumptions?

### Data and benchmark design
- Are train/validation/test boundaries defensible?
- Could leakage, duplication, contamination, or benchmark saturation explain the result?
- Are datasets representative of the deployment or research setting being claimed?

### Baselines and comparisons
- Are the baselines strong enough?
- Are tuning budgets, data access, tools, and compute budgets comparable?
- Is an apparent gain really due to a confounded variable such as scaling, extra data, or filtering?

### Metrics and interpretation
- Do the metrics capture the failure modes that matter?
- Is the improvement practically meaningful or only statistically visible?
- Are averages hiding subgroup collapse, instability, or extreme tail behavior?

### Causal language and overclaiming
- Does the evidence justify causal or general statements?
- Is a narrow result being generalized to a broader claim about intelligence, robustness, usability, or efficiency?
- Does the paper confuse correlation, proxy performance, and actual capability?

### Reproducibility and robustness
- Would the conclusion survive different seeds, environments, workloads, or datasets?
- Are there ablations or controls for the components that supposedly matter?
- Are negative results or boundary conditions missing?

## Domain Hints

Apply the same core logic, but emphasize different checks by subfield:
- ML / LLMs: leakage, benchmark contamination, scaling confounds, seed sensitivity, weak ablations
- systems: unrealistic workloads, missing bottlenecks, benchmark gaming, environment dependence
- software engineering: dataset labeling quality, project selection bias, threat to external validity
- HCI: task realism, study power, participant bias, ecological validity
- security: attacker model gaps, unrealistic assumptions, incomplete threat coverage
- theory: hidden assumptions, theorem-to-practice disconnect, omitted edge cases

## Use Local References Selectively

Read only the references that help the current critique:
- `references/experimental_design.md`
- `references/statistical_pitfalls.md`
- `references/common_biases.md`
- `references/logical_fallacies.md`
- `references/evidence_hierarchy.md`
- `references/scientific_method.md`

## Useful Output Formats

Choose one depending on the task:
- claim-to-evidence audit
- list of confounders and missing controls
- stronger experiment design
- reviewer-style critique
- risk register for a proposed research direction
- questions that must be answered before implementation or submission

## Default Output

When the user simply asks for a critical analysis, return:
1. the main claims being examined
2. the strongest supporting evidence
3. the weakest links or confounders
4. what additional evidence would materially strengthen the case