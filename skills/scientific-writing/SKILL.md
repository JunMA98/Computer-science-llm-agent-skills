---
name: scientific-writing
description: Draft and revise computer science papers, theses, reports, and technical research documents. Use when writing or rewriting abstracts, introductions, methods, experiments, limitations, artifact sections, related work, or when converting notes, code, and results into publishable CS prose.
---

# Scientific Writing

Use this skill for computer science research writing, not generic scientific prose. Optimize for technical clarity, evidence-backed claims, and venue-aware structure.

## Frame the Writing Task

Identify the document type before drafting:
- conference paper
- journal article
- thesis chapter
- technical report
- project proposal
- benchmark or artifact report

Also identify the research style:
- empirical ML / NLP / CV
- systems or infrastructure
- software engineering
- HCI / user study
- security
- theory / algorithms
- interdisciplinary computing

The section strategy depends on this choice. Do not force every document into the same template.

## Build a Claim-to-Evidence Map

Before writing, list:
- the main claim
- what evidence supports it
- what assumptions or scope limits apply
- what comparisons make the claim credible

Only then draft prose. In CS writing, weak structure usually comes from claims appearing before the evidence chain is clear.

## Section Guidance

### Abstract

Cover, in order:
- problem and setting
- why the problem is hard or important
- core idea or system contribution
- evidence: benchmark, experiment, theorem, deployment result, or user study
- concrete takeaway

Avoid generic phrases like "promising results" without numbers or scope.

### Introduction

A strong CS introduction usually answers:
- what problem matters
- why current methods or systems are insufficient
- what technical challenge blocks progress
- what idea or design addresses that challenge
- what evidence supports the contribution
- what the paper contributes

Make contributions specific. "We propose a framework" is weak unless the framework changes capability, efficiency, robustness, interpretability, usability, or understanding in a measurable way.

### Method / System / Approach

Write enough detail for a technically literate reader to reconstruct the design:
- task definition or threat model
- assumptions and scope
- algorithm, architecture, pipeline, or protocol
- data flow or component interaction
- training, inference, or runtime behavior
- complexity, cost, or engineering tradeoffs when relevant

### Experiments / Evaluation

In CS, this section carries most of the paper's credibility. Make it easy to audit:
- datasets and splits
- baselines and why they are fair
- metrics and what they capture
- implementation details that affect outcomes
- hardware / compute budget when important
- ablations, error analysis, stress tests, or user studies
- limitations and negative results if they matter to interpretation

### Discussion / Limitations

State where the method or system may fail. This strengthens the paper when the limitation is honest and bounded.

## Style Rules

- Prefer short, technical sentences over inflated language.
- Replace vague qualifiers with measurable statements.
- Define notation, task setting, and abbreviations at first use.
- Keep paragraph topic sentences strong; each paragraph should advance one point.
- Separate empirical claims from hypotheses.
- Do not oversell novelty when the main value is engineering, benchmarking, or integration.

## Use Local References Selectively

Read only the references that match the writing problem:
- `references/writing_principles.md` for general style discipline
- `references/imrad_structure.md` when shaping standard paper flow
- `references/figures_tables.md` when revising figure/table integration
- `references/citation_styles.md` when bibliography formatting matters
- `references/reporting_guidelines.md` when transparency or reporting completeness is under review

Use assets only when they solve a real formatting task:
- `assets/scientific_report_template.tex`
- `assets/scientific_report.sty`
- `assets/REPORT_FORMATTING_GUIDE.md`

## Default Outputs

When the user asks for writing help without a strict format, return:
1. a suggested section structure
2. a revised draft or outline
3. a list of unsupported claims or missing evidence
4. concrete revision priorities