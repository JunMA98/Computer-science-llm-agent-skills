---
name: scientific-schematics
description: Create polished technical diagrams for CS papers, slides, posters, demos, and repo documentation. Use when a Mermaid diagram is not enough and the task needs a cleaner architecture figure, system overview, pipeline graphic, benchmark setup diagram, or agent workflow illustration.
---

# Scientific Schematics

Use this skill for polished technical figures, not for routine text-native diagrams. Prefer Mermaid first when editability matters more than appearance.

## Good Fits

- model architecture overviews
- system component diagrams
- agent or tool-call workflows
- training / inference pipelines
- benchmark or evaluation setup figures
- data processing or serving architecture diagrams

## Working Rules

- Start from the message the figure must communicate.
- Label components by role, not by decorative wording.
- Make data flow, control flow, and evaluation boundaries explicit.
- Avoid overloading one figure with both architecture and results.
- Prefer a small number of well-grouped components over exhaustive detail.

## Local Resources

Read `references/best_practices.md` when you need diagram design guidance.

Use local scripts only when the configured image-generation workflow is available and the user actually wants rendered figures:
- `scripts/generate_schematic.py`
- `scripts/generate_schematic_ai.py`

The quick-reference files in `references/` are inherited upstream support material. Use them selectively.

## Relationship to Other Skills

- Use `markdown-mermaid-writing` for editable diagrams in docs and notes.
- Use this skill when the figure is headed into a paper, poster, deck, or polished README.

## Default Output

When the user asks for a diagram without a target format, return:
1. the figure concept
2. required components and labels
3. a recommended diagram structure
4. whether Mermaid or a rendered schematic is the better fit