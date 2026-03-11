---
name: markitdown
description: Convert papers, slide decks, reports, office files, and mixed-format project materials into Markdown for CS research and engineering workflows. Use when turning PDFs, PPTX, DOCX, HTML, JSON, CSV, or similar inputs into LLM-friendly text for literature review, repo cleanup, release prep, or paper-to-code analysis.
---

# MarkItDown

Use this skill when document conversion is the bottleneck. The goal is to turn source files into clean markdown that can be searched, compared, summarized, or fed into other skills.

## Common CS Workflows

- convert papers or supplements for reading and note extraction
- convert slide decks into reviewable markdown outlines
- normalize mixed repo docs before GitHub release
- extract benchmark tables or structured notes from reports
- convert exported issue logs, HTML docs, or API pages into text

## Working Rules

- Convert first, then clean structure and headings.
- Preserve tables, code blocks, and lists where possible.
- Treat OCR or AI-enhanced descriptions as fallback, not default.
- If a document contains diagrams or equations, note possible fidelity loss.
- For scanned PDFs or image-heavy files, explicitly warn about extraction quality.

## Local Resources

Use these when they help:
- `scripts/batch_convert.py`
- `scripts/convert_literature.py`
- `scripts/convert_with_ai.py` only when standard conversion is insufficient
- `references/file_formats.md`
- `references/api_reference.md`
- `assets/example_usage.md`

## Recommended Outputs

Pick the output based on the task:
- paper markdown for downstream summarization
- cleaned note file for a literature matrix
- repo documentation conversion batch
- markdown bundle for release preparation

## Default Output

When the user asks to convert material without more detail, return:
1. the converted markdown or conversion result
2. any fidelity issues
3. suggested cleanup steps before using the output downstream