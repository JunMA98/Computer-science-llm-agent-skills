# Usage Guide

Use this guide when you do not want to browse the repository skill-by-skill and instead want a fast path from a workflow need to the right public skills.

## Read the Public Metadata First

The public docs use two main metadata fields:

- `Primary Category`: the main home of a skill in [taxonomy.md](taxonomy.md)
- `Task Tags`: short labels such as `writing`, `paper-review`, `benchmark`, or `agents`

The [skills index](skills-index.md) also records a `Type` field (`Curated` or `Custom`) for provenance, but you usually do not need it to start using the skills.

## Start From Your Task

| If you are doing... | Start with | Then add | Why this path works |
| --- | --- | --- | --- |
| Literature review | `literature-review`, `citation-management`, `pyzotero` | `scientific-critical-thinking`, `markitdown` | Start with paper discovery and citation hygiene, then add critique and document conversion if needed. |
| Paper writing | `scientific-writing`, `citation-management`, `code-to-paper` | `venue-templates`, `scientific-visualization` | Draft the manuscript first, then adapt to venue expectations and improve figures. |
| Peer review or rebuttal | `peer-review`, `reviewer-response` | `scholar-evaluation`, `scientific-critical-thinking` | Separate structured assessment from response drafting and claim stress-testing. |
| Benchmark design | `benchmark-design`, `statistical-analysis` | domain tools such as `scikit-learn`, `transformers`, `stable-baselines3` | Define fair evaluation rules before choosing the model stack. |
| Experiment tracking | `experiment-tracking`, `get-available-resources` | `polars`, `dask`, `vaex`, `scientific-visualization` | Track runs first, then analyze and present results at the right scale. |
| Code reproduction | `code-reproduction`, `get-available-resources` | `benchmark-design`, `experiment-tracking` | Rebuild the environment and execution path before comparing outcomes. |
| Agent development | `agent-coding`, `transformers` | `modal`, `markdown-mermaid-writing`, `benchmark-design` | Combine model choice, system design, deployment, and evaluation planning. |
| GitHub release preparation | `github-release-prep`, `repo-cleanup` | `markitdown`, `venue-templates` | Clean structure and release blockers first, then fix docs or public-facing artifacts. |

If you want a broader matrix of tasks and supporting skills, also read [task-to-skills.md](task-to-skills.md).

## Start From Category

Use this route when you know the general class of work but not the exact skill yet.

| Category | Good starting question | Typical starting skills |
| --- | --- | --- |
| Research Planning & Task Decomposition | “How do I turn this idea into a plan?” | `research-planning` |
| Literature Review & Reference Management | “How do I map papers and keep citations clean?” | `literature-review`, `citation-management`, `pyzotero` |
| Paper Writing & Revision | “How do I turn notes or code into a publishable paper?” | `scientific-writing`, `code-to-paper`, `venue-templates` |
| Review, Rebuttal & Scholarly Evaluation | “How do I review this work or respond to reviewers?” | `peer-review`, `reviewer-response`, `scholar-evaluation` |
| Benchmarking, Reproducibility & Experiment Ops | “How do I design, rerun, or track experiments?” | `benchmark-design`, `experiment-tracking`, `code-reproduction` |
| Technical Writing & Artifact Conversion | “How do I convert or document technical material?” | `markdown-mermaid-writing`, `markitdown`, `paper-to-code` |
| Data Engineering, Statistics & Visualization | “How do I inspect, analyze, or visualize results?” | `exploratory-data-analysis`, `polars`, `scientific-visualization` |
| ML / LLM / Graph / RL Workflows | “Which model or training stack should I start from?” | `scikit-learn`, `transformers`, `pytorch-lightning`, `torch-geometric` |
| Agent Systems & Automation Development | “How do I structure a tool-using agent system?” | `agent-coding` |
| Presentation & Publication Assets | “How do I present the work clearly?” | `scientific-slides`, `latex-posters`, `scientific-schematics` |
| Repository Maintenance & Open-Source Release | “How do I make this repo public-ready?” | `repo-cleanup`, `github-release-prep` |
| Mathematical & Algorithmic Tools | “How do I reason about the math or graph structure?” | `sympy`, `networkx` |

For the full inventory behind those categories, use [skills-index.md](skills-index.md).

## Recommended Navigation Paths

### Paper-centric path

1. Start with `literature-review` and `citation-management`
2. Move to `scientific-writing`
3. Add `code-to-paper` if the source of truth is an existing codebase
4. Add `venue-templates` when the draft is close to submission
5. Add `peer-review` or `reviewer-response` when review-stage work begins

### Experiment-centric path

1. Start with `benchmark-design`
2. Check hardware with `get-available-resources`
3. Run and organize work with `experiment-tracking`
4. Use domain tools such as `scikit-learn`, `transformers`, `pytorch-lightning`, or `stable-baselines3`
5. Analyze outputs with `exploratory-data-analysis`, `polars`, `statistical-analysis`, and `scientific-visualization`

### Release-centric path

1. Start with `repo-cleanup`
2. Convert scattered materials with `markitdown` if needed
3. Verify public-readiness with `github-release-prep`
4. Improve docs with `markdown-mermaid-writing`
5. Polish presentation assets with `scientific-slides`, `latex-posters`, or `scientific-schematics` if the release includes talks or demos

## If You Only Want One Entry Point

Use this order:

1. [skills-index.md](skills-index.md) for the full catalog
2. [task-to-skills.md](task-to-skills.md) for concrete workflow mapping
3. [taxonomy.md](taxonomy.md) if you want to understand the repository's category system