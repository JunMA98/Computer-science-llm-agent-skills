---
name: scientific-visualization
description: Orchestrate publication-ready figures for CS papers, posters, slides, and benchmark reports. Use when assembling multi-panel result figures, harmonizing styles across plots, preparing export settings, or turning experiment outputs into clear visual evidence for submissions and technical communication.
---

# Scientific Visualization

Use this skill when figure quality, consistency, and evidence communication matter more than raw plotting mechanics.

## Typical CS Outputs

- benchmark comparison figures
- ablation summaries
- latency / memory / accuracy tradeoff panels
- error analysis views
- embedding or representation comparison panels
- reproducibility or scaling plots
- poster or slide figure sets with consistent styling

## Workflow

1. Identify the claim each figure must support.
2. Choose the smallest set of plots that makes the comparison interpretable.
3. Standardize colors, labels, scales, and panel conventions.
4. Export in formats appropriate to the destination: paper, slide, poster, or README.

## Local Resources

Assets:
- `assets/publication.mplstyle`
- `assets/presentation.mplstyle`
- `assets/color_palettes.py`
- `assets/nature.mplstyle` as an inherited legacy style, not the default

References:
- `references/publication_guidelines.md`
- `references/color_palettes.md`
- `references/matplotlib_examples.md`
- `references/journal_requirements.md` only when a venue genuinely requires it

Scripts:
- `scripts/figure_export.py`
- `scripts/style_presets.py`

## Working Rules

- Optimize first for truthful comparison, then for polish.
- Use consistent semantics across panels.
- Label uncertainty clearly when seeds, folds, or repeated trials matter.
- Do not overload a paper figure with dashboard-level detail.
- If the figure is exploratory rather than final, use seaborn or plotly directly instead.

## Default Output

When the user asks for figure help without more detail, return:
1. figure set recommendation
2. panel structure and style notes
3. export guidance for the target medium
4. risks that could make the visual misleading