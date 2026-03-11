---
name: markdown-mermaid-writing
description: Write markdown-first technical documents with Mermaid diagrams for CS research, engineering, and agent workflows. Use when creating design docs, research notes, experiment plans, repo documentation, issue reports, architecture diagrams, workflow descriptions, or text-native visual explanations that should diff cleanly in Git.
---

# Markdown and Mermaid Writing

Use markdown plus Mermaid as the default text-native format for CS documentation. Prefer it when diagrams should remain editable, reviewable, and easy to version-control.

## Good Fits

- system architecture notes
- agent or tool workflow diagrams
- experiment plans and benchmark protocols
- repo documentation and onboarding docs
- issue, PR, or release notes
- research outlines, related-work maps, and slide drafts

## Working Rules

- Keep markdown as the source of truth.
- Use Mermaid when structure matters more than polished graphics.
- Prefer concise diagrams that clarify dependencies, flow, or state changes.
- Use prose for nuance and Mermaid for relationships.
- Avoid diagram types that look impressive but do not change understanding.

## Useful Local Resources

Read only what matches the task:
- `references/markdown_style_guide.md`
- `references/mermaid_style_guide.md`
- `references/diagrams/architecture.md`
- `references/diagrams/flowchart.md`
- `references/diagrams/sequence.md`
- `references/diagrams/state.md`
- `references/diagrams/c4.md`
- `references/diagrams/er.md`

Templates worth reusing:
- `templates/project_documentation.md`
- `templates/research_paper.md`
- `templates/status_report.md`
- `templates/decision_record.md`
- `templates/presentation.md`
- `templates/pull_request.md`

## Relationship to Other Skills

- Use `scientific-writing` for prose-heavy paper drafting.
- Use `scientific-schematics` only when a polished figure is needed beyond Mermaid.
- Use this skill first when a text-native architecture or workflow diagram is enough.

## Default Output

When the user asks for documentation help without specifying a format, return:
1. a suggested markdown structure
2. one or more Mermaid diagrams if they improve clarity
3. naming or organization suggestions for long-term maintenance