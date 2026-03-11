# Task-to-Skills Mapping

| Task category | Typical subtasks | Required skills | Optional skills | Notes |
| --- | --- | --- | --- | --- |
| Research planning | scope a topic, define milestones, identify risks, sequence tasks | `research-planning` | `scientific-brainstorming` (pending) | New custom skill fills a previously uncovered workflow. |
| Literature review | find papers, organize references, synthesize evidence | `literature-review`, `citation-management`, `pyzotero` | `scientific-critical-thinking`, `scholar-evaluation` | Search-backend-heavy skills remain pending if licensing or API coupling is unclear. |
| Paper writing | draft sections, revise prose, structure manuscript, prepare submission | `scientific-writing`, `citation-management`, `code-to-paper` | `venue-templates`, `markitdown`, `markdown-mermaid-writing` | The writing stack is now aligned to CS paper and report workflows. |
| Paper-to-code implementation | extract modules, identify missing assumptions, design build order | `paper-to-code`, `code-reproduction` | `benchmark-design` | Useful when implementing from papers or supplements. |
| Code-to-paper conversion | convert repo/results into claims, figures, and outline | `code-to-paper`, `scientific-writing` | `experiment-tracking`, `scientific-visualization` | Prevents overclaiming from code-only evidence. |
| Review and rebuttal | assess rigor, answer reviewers, plan revisions | `peer-review`, `reviewer-response` | `scientific-critical-thinking`, `scholar-evaluation` | Rebuttal is now explicitly covered. |
| Benchmark design | define baselines, metrics, splits, ablations, fairness rules | `benchmark-design` | `statistical-analysis`, `statsmodels`, `scikit-learn` | High-value for ML, systems, and agent projects. |
| Experiment tracking | log runs, compare results, summarize best settings | `experiment-tracking` | `polars`, `dask`, `vaex` | Keeps ablations and baselines interpretable. |
| Code reproduction | rebuild environment, rerun results, log discrepancies | `code-reproduction` | `experiment-tracking`, `get-available-resources` | Important before extending a baseline or prior paper. |
| Data engineering and analysis | clean data, process large outputs, inspect failures | `polars`, `dask`, `vaex`, `exploratory-data-analysis` | `get-available-resources` | Good support already exists. |
| Statistical analysis | choose tests, fit models, report uncertainty | `statistical-analysis`, `statsmodels` | `scikit-learn`, `umap-learn` | Covers both guided and model-specific analysis. |
| Visualization | figures, dashboards, publication plots, technical diagrams | `matplotlib`, `seaborn`, `plotly`, `scientific-visualization` | `scientific-schematics` | Covers both exploratory and publication-oriented outputs. |
| ML and deep learning | baselines, training loops, fine-tuning, explainability | `scikit-learn`, `pytorch-lightning`, `transformers` | `shap`, `torch-geometric`, `stable-baselines3` | Strong support for core ML workflows. |
| Agent system development | define tools, prompts, state, evals, recovery logic | `agent-coding` | `transformers`, `modal`, `markdown-mermaid-writing` | Newly added custom workflow layer. |
| Presentation and communication | talks, posters, diagrams, visual summaries | `scientific-slides`, `latex-posters`, `scientific-schematics` | `scientific-visualization` | Slide support now explicitly targets CS talks, defenses, demos, and project updates. |
| Repo cleanup | normalize structure, separate source/artifacts, identify stale files | `repo-cleanup` | `markitdown` | Focuses on pre-release repo hygiene. |
| GitHub release preparation | verify docs, legal files, examples, blockers | `github-release-prep` | `repo-cleanup`, `venue-templates` | Designed for final public handoff. |