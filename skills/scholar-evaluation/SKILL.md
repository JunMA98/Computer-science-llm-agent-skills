---
name: scholar-evaluation
description: Score and assess CS papers, proposals, literature reviews, and benchmark plans using a structured evaluation rubric. Use when a quantitative or semi-structured assessment is needed for research quality, novelty, technical soundness, empirical rigor, reproducibility, clarity, and submission readiness.
---

# Scholar Evaluation

Use this skill when the user wants more structure than a free-form review but does not need a full venue-specific peer review.

## Good Fits

- comparing multiple candidate papers
- grading a draft literature review
- evaluating a research proposal before implementation
- checking whether a benchmark plan is rigorous enough
- estimating whether a draft is close to submission quality

## CS-Oriented Dimensions

Score or discuss these explicitly:
- problem importance and positioning
- novelty or distinct value
- technical soundness
- empirical rigor or evaluation adequacy
- reproducibility and artifact clarity
- writing clarity and organization
- risk areas that could block publication or adoption

## Local Resources

- `references/evaluation_framework.md`
- `scripts/calculate_scores.py`

Use the script when a numeric roll-up is useful. Otherwise keep the evaluation semi-structured and explain the score rationale.

## Working Rules

- Do not hide major flaws behind an average score.
- Separate missing evidence from poor writing.
- State what would most improve the work.
- Use scoring to support judgment, not replace it.

## Default Output

When no format is requested, return:
1. dimension-by-dimension assessment
2. strengths
3. highest-impact weaknesses
4. overall readiness judgment