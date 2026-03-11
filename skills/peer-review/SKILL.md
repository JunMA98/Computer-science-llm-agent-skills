---
name: peer-review
description: Review computer science papers, rebuttals, and artifact submissions for conferences, journals, and workshops. Use when evaluating novelty, technical correctness, empirical rigor, reproducibility, clarity, significance, or when drafting a structured review, meta-review, or author questions.
---

# Peer Review

Use this skill for CS-style reviewing. Focus on technical soundness and evidence quality, not generic editorial commentary.

## Start by Identifying the Review Context

Clarify or infer:
- venue and track
- paper type: empirical ML, systems, SE, HCI, security, theory, benchmark, dataset, or tool paper
- review stage: initial review, rebuttal response, camera-ready check, or artifact evaluation
- whether the user wants a private assessment, a review draft, or a list of author-facing questions

Venue context matters because expectations differ across fields, but the core review standard is stable: claims must match evidence.

## Core Review Dimensions

Evaluate these dimensions explicitly.

### 1. Problem significance and positioning
- Is the problem meaningful for the field?
- Is the paper positioned against the right prior work?
- Does the paper distinguish incremental engineering from genuine conceptual advance?

### 2. Technical soundness
- Are the assumptions clear and reasonable?
- Is the method, proof, protocol, or system design internally coherent?
- Are there hidden dependencies, unstated constraints, or ambiguous implementation choices?

### 3. Empirical rigor
- Are datasets, splits, metrics, and baselines appropriate?
- Are comparisons fair in data, compute, tuning budget, and evaluation protocol?
- Are variance, seeds, ablations, and failure cases handled well enough for the claim strength?

### 4. Reproducibility and transparency
- Can a knowledgeable reader reproduce the key result from the description?
- Are code, artifacts, prompts, checkpoints, configs, or system settings available or at least described clearly?
- Are limitations and negative cases disclosed?

### 5. Clarity
- Is the writing precise enough to follow the contribution and evidence?
- Do figures and tables actually support the claims?
- Is there a gap between what the abstract promises and what the paper demonstrates?

## Common CS Failure Modes

Look for issues that frequently invalidate otherwise polished papers:
- weak or outdated baselines
- unreported tuning asymmetry
- benchmark contamination or split leakage
- cherry-picked qualitative examples
- missing ablations for key design choices
- reporting only best runs instead of robust aggregates
- metric choice that hides obvious failure cases
- conclusions that exceed the tested setting
- theory disconnected from implementation reality
- systems claims without realistic workload analysis

Read `references/common_issues.md` when you want a broader checklist of failure patterns.
Read `references/reporting_standards.md` when transparency, completeness, or reproducibility reporting is part of the decision.

## Review Writing Structure

When drafting a review, default to this structure:
1. concise summary of the paper and claimed contribution
2. strengths grounded in evidence
3. major concerns ordered by impact
4. minor concerns or presentation issues
5. concrete questions for the authors
6. overall assessment separated from the factual concerns

Keep every criticism actionable. Cite the exact mismatch between claim and evidence whenever possible.

## Tone Rules

- Be direct, not hostile.
- Avoid vague praise that hides major technical concerns.
- Do not invent certainty when the paper is ambiguous; state the ambiguity.
- Separate objective issues from preference or taste.
- If the decision hinges on missing evidence, say what experiment, proof detail, or clarification would change the assessment.

## Default Deliverables

When no review format is requested, return:
- a 3 to 6 sentence summary
- strengths
- major concerns
- minor concerns
- author questions
- an overall recommendation with confidence if appropriate