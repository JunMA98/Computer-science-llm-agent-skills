# Attribution and Provenance

This file tracks the upstream-derived skills copied into this public repository.

Upstream reference repository: `K-Dense-AI/claude-scientific-skills`
Canonical upstream URL: `https://github.com/K-Dense-AI/claude-scientific-skills`

Repository-authored custom skills in `skills/custom/` are original additions for this project and are not copied from the upstream repository.

| Public item | Source path | Decision | License note | Notes |
| --- | --- | --- | --- | --- |
| `skills/curated/exploratory-data-analysis` | `scientific-skills/exploratory-data-analysis` | `rewrite` | `MIT license` | Selected from upstream, rewritten for CS-specific use, and included in the public curated set. |
| `skills/curated/dask` | `scientific-skills/dask` | `keep` | `BSD-3-Clause license` | Selected and copied as a retained curated skill. |
| `skills/curated/polars` | `scientific-skills/polars` | `keep` | `https://github.com/pola-rs/polars/blob/main/LICENSE` | Selected and copied as a retained curated skill. |
| `skills/curated/vaex` | `scientific-skills/vaex` | `keep` | `MIT license` | Selected and copied as a retained curated skill. |
| `skills/curated/matplotlib` | `scientific-skills/matplotlib` | `keep` | `https://github.com/matplotlib/matplotlib/tree/main/LICENSE` | Selected and copied as a retained curated skill. |
| `skills/curated/plotly` | `scientific-skills/plotly` | `keep` | `MIT license` | Selected and copied as a retained curated skill. |
| `skills/curated/scientific-visualization` | `scientific-skills/scientific-visualization` | `keep` | `MIT license` | Selected and copied as a retained curated skill. |
| `skills/curated/seaborn` | `scientific-skills/seaborn` | `keep` | `BSD-3-Clause license` | Selected and copied as a retained curated skill. |
| `skills/curated/scholar-evaluation` | `scientific-skills/scholar-evaluation` | `keep` | `MIT license` | Selected and copied as a retained curated skill. |
| `skills/curated/scientific-critical-thinking` | `scientific-skills/scientific-critical-thinking` | `rewrite` | `MIT license` | Selected from upstream, rewritten for CS-specific use, and included in the public curated set. |
| `skills/curated/networkx` | `scientific-skills/networkx` | `keep` | `3-clause BSD license` | Selected and copied as a retained curated skill. |
| `skills/curated/torch-geometric` | `scientific-skills/torch-geometric` | `keep` | `MIT license` | Selected and copied as a retained curated skill. |
| `skills/curated/literature-review` | `scientific-skills/literature-review` | `rewrite` | `MIT license` | Selected from upstream, rewritten for CS-specific use, and included in the public curated set. |
| `skills/curated/citation-management` | `scientific-skills/citation-management` | `keep` | `MIT License` | Selected and copied as a retained curated skill. |
| `skills/curated/pyzotero` | `scientific-skills/pyzotero` | `keep` | `MIT License` | Selected and copied as a retained curated skill. |
| `skills/curated/transformers` | `scientific-skills/transformers` | `keep` | `Apache-2.0 license` | Selected and copied as a retained curated skill. |
| `skills/curated/scikit-learn` | `scientific-skills/scikit-learn` | `keep` | `BSD-3-Clause license` | Selected and copied as a retained curated skill. |
| `skills/curated/umap-learn` | `scientific-skills/umap-learn` | `keep` | `BSD-3-Clause license` | Selected and copied as a retained curated skill. |
| `skills/curated/sympy` | `scientific-skills/sympy` | `keep` | `https://github.com/sympy/sympy/blob/master/LICENSE` | Selected and copied as a retained curated skill. |
| `skills/curated/pytorch-lightning` | `scientific-skills/pytorch-lightning` | `keep` | `Apache-2.0 license` | Selected and copied as a retained curated skill. |
| `skills/curated/shap` | `scientific-skills/shap` | `keep` | `MIT license` | Selected and copied as a retained curated skill. |
| `skills/curated/scientific-writing` | `scientific-skills/scientific-writing` | `rewrite` | `MIT license` | Selected from upstream, rewritten for CS-specific use, and included in the public curated set. |
| `skills/curated/peer-review` | `scientific-skills/peer-review` | `rewrite` | `MIT license` | Selected from upstream, rewritten for CS-specific use, and included in the public curated set. |
| `skills/curated/latex-posters` | `scientific-skills/latex-posters` | `keep` | `` | Selected and copied as a retained curated skill. |
| `skills/curated/scientific-schematics` | `scientific-skills/scientific-schematics` | `keep` | `MIT license` | Selected and copied as a retained curated skill. |
| `skills/curated/scientific-slides` | `scientific-skills/scientific-slides` | `rewrite` | `MIT license` | Selected from upstream, rewritten for CS-specific use, and included in the public curated set. |
| `skills/curated/venue-templates` | `scientific-skills/venue-templates` | `rewrite` | `MIT license` | Selected from upstream, rewritten for CS-specific use, and included in the public curated set. |
| `skills/curated/get-available-resources` | `scientific-skills/get-available-resources` | `keep` | `MIT license` | Selected and copied as a retained curated skill. |
| `skills/curated/modal` | `scientific-skills/modal` | `keep` | `Apache-2.0 license` | Selected and copied as a retained curated skill. |
| `skills/curated/stable-baselines3` | `scientific-skills/stable-baselines3` | `keep` | `MIT license` | Selected and copied as a retained curated skill. |
| `skills/curated/statistical-analysis` | `scientific-skills/statistical-analysis` | `keep` | `MIT license` | Selected and copied as a retained curated skill. |
| `skills/curated/statsmodels` | `scientific-skills/statsmodels` | `keep` | `BSD-3-Clause license` | Selected and copied as a retained curated skill. |
| `skills/curated/markitdown` | `scientific-skills/markitdown` | `keep` | `MIT license` | Selected and copied as a retained curated skill. |
| `skills/curated/markdown-mermaid-writing` | `scientific-skills/markdown-mermaid-writing` | `keep` | `Apache-2.0` | Selected and copied as a retained curated skill. |

## Not copied into the public folder

| Skill | Decision | Reason |
| --- | --- | --- |
| `denario` | `pending` | Interesting multi-agent research system, but too broad and platform-like for immediate inclusion. |
| `docx` | `pending` | Potentially useful, but current licensing terms are proprietary in the upstream skill. |
| `pdf` | `pending` | Potentially useful, but current licensing terms are proprietary in the upstream skill. |
| `pptx` | `pending` | Potentially useful, but current licensing terms are proprietary in the upstream skill. |
| `xlsx` | `pending` | Potentially useful, but current licensing terms are proprietary in the upstream skill. |
| `open-notebook` | `pending` | Useful conceptually, but it is product-like and broader than the immediate curated skill set. |
| `matlab` | `pending` | Potentially useful, but tool licensing and audience breadth need clearer positioning. |
| `pymoo` | `pending` | Relevant to optimization research, but not broad enough for the first public set. |
| `pptx-posters` | `pending` | Useful for a specific poster format, but secondary to the more general poster workflow. |
| `cirq` | `pending` | Relevant to a CS subfield, but niche for the repository core. |
| `pennylane` | `pending` | Relevant to a CS subfield, but niche for the repository core. |
| `qiskit` | `pending` | Relevant to a CS subfield, but niche for the repository core. |
| `paper-2-web` | `pending` | Useful for dissemination, but current licensing is unclear. |
| `hypogenic` | `pending` | Interesting for AI-assisted hypothesis testing, but not yet clearly reusable across CS workflows. |
| `hypothesis-generation` | `pending` | Relevant to research planning, but too generic for direct inclusion without refocusing. |
| `scientific-brainstorming` | `pending` | Potentially useful for ideation, but too generic for direct inclusion as-is. |
| `bgpt-paper-search` | `pending` | Potentially useful, but depends on a specialized MCP service and needs closer validation. |
| `openalex-database` | `pending` | Useful for scholarly search, but upstream frontmatter reports unknown license. |
| `parallel-web` | `pending` | Useful in principle, but tightly coupled to specific external APIs and broader than the core repository scope. |
| `perplexity-search` | `pending` | Useful in principle, but tightly coupled to specific external APIs. |
| `research-lookup` | `pending` | Useful in principle, but currently coupled to specific external search backends. |
| `uspto-database` | `pending` | Potentially useful for prior-art analysis, but licensing is unclear and it is not core to the repository. |
| `pufferlib` | `pending` | Relevant but more niche and specialized than the first public RL selection. |
| `simpy` | `pending` | Relevant to systems and simulation work, but not broad enough for the first public set. |
| `geopandas` | `pending` | Useful for geospatial computing, but not broad enough for the core CS research workflow set. |
| `aeon` | `pending` | Relevant to time-series ML, but not broad enough for the first public set. |
| `timesfm-forecasting` | `pending` | Relevant to time-series forecasting, but not broad enough for the first public set. |
| `pymc` | `pending` | Relevant to Bayesian modeling, but more specialized than the first public statistical set. |

This table records provenance for the public curated set. Repository-level licensing for original project-authored materials is documented in `LICENSE`, while upstream-derived entries remain subject to their own source licenses.
