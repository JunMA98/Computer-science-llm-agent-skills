---
name: scientific-slides
description: Build and revise computer science research slides for conference talks, paper presentations, defenses, group meetings, demos, and project updates. Use when turning a paper, benchmark, experiment, system design, or research plan into clear slides with strong structure, visual hierarchy, and timing discipline.
---

# Scientific Slides

Use this skill for CS research presentations. Optimize for technical clarity, narrative flow, and audience comprehension under time pressure.

## Start With Talk Constraints

Clarify or infer:
- talk type: conference talk, paper reading, defense, seminar, lab update, demo, tutorial
- audience: subfield experts, broad CS audience, students, industry engineers, reviewers
- duration and Q&A budget
- medium: Beamer, PowerPoint, Markdown-to-slides, or another deck workflow
- whether the deck supports a paper, a project demo, a proposal, or a benchmark report

Read `references/talk_types_guide.md` or `references/presentation_structure.md` when structure needs help.

## Narrative for CS Talks

Most strong computing talks follow this sequence:
1. problem and why it matters
2. why the problem is hard
3. core idea, architecture, or system design
4. how the method / system / study works
5. evaluation setup
6. key results and what they mean
7. limitations, takeaways, and next steps

Do not mirror the paper section-by-section if that hurts comprehension.

## Slide-Level Rules

- Keep one main idea per slide.
- Prefer diagrams, tables, and concise bullets over paragraph text.
- Make architecture, pipeline, benchmark setup, or experimental protocol visually explicit.
- Highlight the comparison that matters; do not dump full result tables when a distilled view is enough.
- Use animations sparingly and only when they reveal structure or sequence.

For result slides, answer three questions fast:
- what is being compared
- what the main result is
- why the result matters

## Visual Content That Matters in CS

Prioritize visuals that clarify technical structure:
- model or system architecture
- data / control flow
- training or inference pipeline
- benchmark composition and evaluation protocol
- ablation summaries
- failure analysis or qualitative examples
- latency / memory / throughput tradeoffs

Read `references/data_visualization_slides.md` and `references/slide_design_principles.md` when revising cluttered result slides.

## Use Local Assets and Scripts

For LaTeX/Beamer work:
- `assets/beamer_template_conference.tex`
- `assets/beamer_template_defense.tex`
- `assets/beamer_template_seminar.tex`
- `references/beamer_guide.md`

For PowerPoint-style work:
- `assets/powerpoint_design_guide.md`
- `assets/timing_guidelines.md`

For production and review:
- `scripts/slides_to_pdf.py`
- `scripts/validate_presentation.py`
- `scripts/pdf_to_images.py`

Only use `scripts/generate_slide_image.py` or `scripts/generate_slide_image_ai.py` if the user explicitly wants synthetic illustration support. Do not default to decorative AI images.

## Review Checklist

Before finalizing a deck, check:
- the first 3 slides establish the problem and context fast
- every result slide has an interpretable takeaway
- fonts and figure labels remain readable at presentation distance
- timing is realistic for the allotted slot
- backup slides exist for details that may come up in Q&A

## Default Deliverables

When the user asks for slide help without specifying format, return:
- a talk outline
- slide-by-slide message plan
- recommendations for figures and tables
- timing notes
- revision priorities for clarity