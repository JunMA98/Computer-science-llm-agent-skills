# Capability Gap Analysis

This document identifies important workflow capabilities that were missing from the initial public skill set and records the additional skills created to fill them.

| Missing capability | Why it matters for CS research | Previous state | New skill created |
| --- | --- | --- | --- |
| Research planning and task decomposition | CS projects often fail from vague scope, not lack of tooling. | Missing | `research-planning` |
| Benchmark design | Many papers need stronger evaluation design before implementation. | Missing | `benchmark-design` |
| Experiment tracking and result synthesis | Repeated runs, seeds, and ablations need structured logging. | Missing | `experiment-tracking` |
| Code reproduction | Reproducing papers and baselines is central to credible research. | Missing | `code-reproduction` |
| Reviewer response and rebuttal | Review writing existed, but response strategy did not. | Missing | `reviewer-response` |
| Agent system engineering | The curated set had LLM/model tools but no workflow skill for building agents. | Missing | `agent-coding` |
| Repository cleanup | Public release quality depends on structure and hygiene, not only code. | Missing | `repo-cleanup` |
| GitHub release preparation | Release readiness needs docs, legal checks, examples, and blocker tracking. | Missing | `github-release-prep` |
| Paper-to-code translation | Researchers frequently need to implement from papers. | Missing | `paper-to-code` |
| Code-to-paper translation | Researchers also need to turn prototypes into publishable papers. | Missing | `code-to-paper` |

## Remaining non-trivial gaps

The largest remaining gaps are no longer workflow gaps, but policy or scope gaps:

- proprietary document-format skills such as `pdf`, `docx`, `pptx`, and `xlsx`
- unclear-license research search skills such as `openalex-database` and `paper-2-web`
- vendor-coupled search wrappers such as `research-lookup` and `perplexity-search`
- niche but potentially valuable subfield skills such as `aeon`, `pymc`, `qiskit`, and `cirq`

## Design principle used for new skills

The new skills were created where the repository needed **workflow intelligence** rather than more library wrappers. This is why the additions focus on planning, evaluation discipline, translation between research artifacts, agent engineering, and public-release readiness.