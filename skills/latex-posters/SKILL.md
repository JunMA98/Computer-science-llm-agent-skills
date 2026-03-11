---
name: latex-posters
description: Create computer science research posters in LaTeX for conferences, thesis defenses, demos, and lab presentations. Use when converting a CS paper, benchmark result, system design, or project summary into a poster with strong layout, readable figures, and concise technical messaging.
---

# LaTeX Posters

Use this skill for CS poster workflows. Optimize for architecture diagrams, benchmark highlights, readable tables, and fast comprehension in a noisy conference setting.

## Poster Types

Handle cases such as:
- conference poster based on a paper submission
- lab or department poster for ongoing work
- thesis or defense poster
- demo poster for systems, agents, or tools
- recruitment or project-overview poster for a research group

## Content Strategy

A strong CS poster usually prioritizes:
- problem and why it matters
- core method or system architecture
- benchmark setup or experimental protocol
- 1 to 3 key result panels
- limitations or deployment considerations
- QR code or repo / paper link

Do not paste paragraph-heavy paper text into a poster. Compress aggressively.

## Local Assets

Use the existing templates when they help:
- `assets/beamerposter_template.tex`
- `assets/tikzposter_template.tex`
- `assets/baposter_template.tex`
- `assets/poster_quality_checklist.md`

Read references selectively:
- `references/poster_content_guide.md`
- `references/poster_design_principles.md`
- `references/poster_layout_design.md`
- `references/latex_poster_packages.md`

If a shell review is useful, use `scripts/review_poster.sh`.

## CS-Specific Review Checklist

Check that:
- the title states the technical problem clearly
- the method or system diagram is legible from distance
- result panels show the main comparison immediately
- figure captions carry the takeaway, not just labels
- code, dataset, or paper links are easy to find

## Default Output

When the user asks for poster help without specifying format, return:
1. a poster outline
2. a template recommendation
3. section-level content priorities
4. layout and readability risks