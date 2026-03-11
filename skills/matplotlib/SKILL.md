---
name: matplotlib
description: Create static, highly customized figures for CS papers, benchmark reports, experiment analysis, and technical documentation. Use when default plotting tools are too limiting, when multi-panel layouts need precise control, or when exporting clean PNG, PDF, or SVG figures for research outputs.
---

# Matplotlib

Use this skill when you need exact control over figure structure, axes, annotations, and export settings.

## Good Fits

- training curves and ablation figures
- resource tradeoff plots: latency, memory, throughput
- confusion matrices and calibration-style figures
- multi-panel paper figures
- custom benchmark visualizations that higher-level libraries do not support well

## Local Resources

- `references/plot_types.md`
- `references/styling_guide.md`
- `references/common_issues.md`
- `references/api_reference.md`
- `scripts/plot_template.py`
- `scripts/style_configurator.py`

## Working Rules

- Prefer the object-oriented API for nontrivial figures.
- Design the figure around the comparison the reader must notice first.
- Keep labels, legends, and tick density readable at paper scale.
- Use seaborn or plotly only when their defaults genuinely save time.
- Use `scientific-visualization` when the task is primarily figure orchestration or publication styling across multiple plots.

## Default Output

When the user asks for plotting help without more detail, return:
1. figure plan
2. recommended plot type and layout
3. styling or export notes
4. code skeleton if implementation is requested