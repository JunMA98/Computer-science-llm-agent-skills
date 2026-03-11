---
name: citation-management
description: Manage citations and BibTeX for computer science papers, theses, surveys, rebuttals, and project reports. Use when verifying DOI or arXiv metadata, cleaning `.bib` files, deduplicating references, formatting venue-ready citations, or checking that paper, code, and artifact references are consistent.
---

# Citation Management

Use this skill for CS bibliography hygiene. Prefer canonical metadata from DOI, arXiv, DBLP, Crossref, publisher pages, or Zotero exports over hand-copied references.

## Default Workflow

1. Normalize identifiers first: DOI, arXiv ID, URL, title, citation key.
2. Retrieve metadata from the most reliable source available.
3. Validate author order, title casing, venue name, year, and pages.
4. Distinguish preprint, conference, workshop, journal, and software citations.
5. Format clean BibTeX and record unresolved ambiguities.

## CS-Specific Checks

- Distinguish arXiv preprints from the archival conference or journal version.
- Preserve canonical venue names and abbreviations when the target style expects them.
- Use `booktitle` for conference papers and `journal` for journal articles.
- Avoid citing a project page when an actual paper exists, unless the project page is the artifact being referenced.
- Keep software or library citations aligned with what the paper or repo actually used.
- Watch for duplicate entries caused by conference and journal extensions of the same work.

## Local Resources

Use these local tools when they help:
- `scripts/doi_to_bibtex.py`
- `scripts/extract_metadata.py`
- `scripts/format_bibtex.py`
- `scripts/validate_citations.py`
- `assets/bibtex_template.bib`
- `assets/citation_checklist.md`

Read references selectively:
- `references/metadata_extraction.md`
- `references/citation_validation.md`
- `references/bibtex_formatting.md`
- `references/google_scholar_search.md` only when canonical metadata is missing elsewhere

`references/pubmed_search.md` and `scripts/search_pubmed.py` are inherited upstream resources. Ignore them unless the actual task crosses into biomedical literature.

## Default Output

When the user asks for citation help without a strict format, return:
1. cleaned citation entries or BibTeX
2. metadata uncertainties or conflicts
3. duplicates or versioning issues
4. follow-up actions if a citation still needs manual confirmation