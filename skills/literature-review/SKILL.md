---
name: literature-review
description: Review and synthesize computer science literature for related-work sections, surveys, benchmark positioning, and paper comparison. Use when mapping a CS topic, building a reading list, tracing citation chains, comparing baselines, summarizing papers, or identifying research gaps in machine learning, systems, software engineering, HCI, security, theory, or adjacent computing areas.
---

# Literature Review

Focus on computer science research workflows rather than general science review writing. Produce outputs that help with CS papers, project planning, replication, baseline selection, and problem framing.

## Start With Scope

Clarify these points before collecting papers:
- research question or topic boundary
- subfield and paper type: ML, systems, SE, HCI, security, theory, agents, etc.
- output goal: related-work section, survey note, baseline shortlist, reading memo, or gap analysis
- time window, venue band, and whether preprints are acceptable
- whether code, benchmark, dataset, or artifact availability matters

If the request is underspecified, infer a narrow and defensible scope instead of collecting a broad paper dump.

## Prioritize CS-Specific Evidence

Prefer primary and operationally useful sources:
- papers from target venues, arXiv, OpenReview, ACM/IEEE, USENIX, JMLR, or equivalent primary sources
- official project pages, benchmark documentation, and code repositories when implementation or reproducibility matters
- survey papers only as orientation, not as the final authority

For each paper, extract fields that matter in computing:
- problem setting and task definition
- method family or system design
- datasets, benchmarks, and evaluation splits
- baselines and comparison protocol
- metrics and what they actually measure
- compute, runtime, hardware, or deployment assumptions when relevant
- code, model, or artifact availability
- key limitations and open questions

## Workflow

### 1. Build a candidate set

Use a small set of precise search queries first. Expand only when coverage is clearly missing.

If local scripts are useful:
- use `scripts/search_databases.py` to scaffold search terms or batch query logic
- read `references/database_strategies.md` when refining search patterns

### 2. Screen for relevance

Drop papers that are off-task, obsolete for the question at hand, or only weakly connected by keywords.

Keep explicit notes for why a paper survives screening:
- foundational
- state of the art
- closest baseline
- contrasting approach
- benchmark source
- negative example or flawed comparison

### 3. Normalize extraction

Create a compact comparison matrix instead of free-form notes. A good CS review table usually includes:
- citation
- venue and year
- task / setting
- core idea
- datasets / benchmarks
- main metrics
- strongest result or takeaway
- reproducibility status
- relevance to the user's project

Use `assets/review_template.md` if a structured review document is needed.

### 4. Synthesize, do not list

Convert the paper set into a defensible synthesis:
- cluster papers by problem formulation, method family, or evaluation regime
- identify what assumptions differ across papers
- explain where comparisons are not apples-to-apples
- separate mature patterns from recent but weakly validated claims
- point out underexplored settings, failure cases, or missing evaluations

### 5. Produce the right output

Choose the output format that matches the user's task:
- related-work draft for a paper
- survey-style thematic summary
- baseline shortlist for experiments
- reading memo per paper
- gap analysis and next-step suggestions
- benchmark landscape summary

## Writing Rules

- Prefer precise contrasts over vague praise.
- Do not summarize every paper equally; emphasize the papers that change the user's decisions.
- Do not treat citation count as proof of quality.
- Flag when evidence is weak because results rely on a single dataset, missing code, or unfair comparisons.
- If the user needs final manuscript citations, use `scripts/verify_citations.py` before claiming citation details are clean.
- Read `references/citation_styles.md` only when a citation or bibliography format is requested.

## Default Deliverables

When no format is specified, return:
1. a short topic framing
2. a grouped paper matrix
3. 3 to 6 synthesis bullets
4. research gaps or unresolved questions
5. concrete next actions for experiments, reading, or writing