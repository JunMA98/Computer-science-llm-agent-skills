---
name: venue-templates
description: Adapt computer science papers, posters, rebuttals, and submission packages to venue-specific templates and style expectations. Use when targeting ACM, IEEE, USENIX, NeurIPS, ICML, ICLR, CVPR, ICCV, ECCV, EMNLP, ACL, NAACL, AAAI, IJCAI, KDD, WWW, CHI, UIST, ICSE, FSE, ASE, SOSP, OSDI, NSDI, or similar CS venues.
---

# Venue Templates

Use this skill to make a submission fit a target computing venue. Focus on official template compliance, section emphasis, reviewer expectations, and formatting risk.

## Start With Exact Submission Context

Identify:
- venue name and year
- track or paper type
- anonymous vs camera-ready stage
- page limits and appendix policy
- whether artifact, reproducibility, ethics, or broader-impact statements are required
- whether the user needs paper, poster, rebuttal, or supplementary material support

If the user has an official template, treat that as the source of truth. Local assets in this skill are scaffolding and examples, not a substitute for the venue's current official package.

## CS-Focused Reference Order

Read only what matches the venue:
- `references/cs_conference_style.md` for general CS conference expectations
- `references/ml_conference_style.md` for ML-heavy venues
- `references/conferences_formatting.md` for page, figure, anonymity, and bibliography checks
- `references/reviewer_expectations.md` for what reviewers usually look for
- `references/venue_writing_styles.md` for tone and section emphasis
- `references/posters_guidelines.md` for poster adaptation

Ignore medical, grant, and nature-style references unless the user explicitly asks for them.

## Local Assets Worth Reusing

Useful CS-oriented assets include:
- `assets/journals/neurips_article.tex`
- `assets/examples/neurips_introduction_example.md`
- `assets/posters/beamerposter_academic.tex`

Do not default to:
- `assets/grants/*`
- `assets/examples/medical_structured_abstract.md`
- `assets/examples/cell_summary_example.md`
- `assets/journals/nature_article.tex`
- `assets/journals/plos_one.tex`

Those remain in the folder as inherited upstream material but are outside the core CS workflow.

## Common Venue Adaptation Tasks

Use this skill when the user needs to:
- reshape an introduction for a venue's expected framing
- compress a draft to page limits without deleting core evidence
- adjust figures, tables, or appendices for anonymity or space
- convert a project report into conference-paper structure
- prepare rebuttal or response formatting
- turn a paper into a poster or short talk handout

## Output Structure

When adapting content, work at two levels:

### Structural fit
- required sections present
- contribution framing matches venue norms
- evidence appears in the sections reviewers will scrutinize most
- optional content moved to appendix or supplement when needed

### Formatting fit
- template file and bibliography style match
- anonymity rules are respected
- figure sizing, float behavior, and captions are compliant
- page budget is spent on evidence, not throat-clearing

## Local Scripts

Use local scripts when they help with deterministic checks:
- `scripts/query_template.py`
- `scripts/validate_format.py`
- `scripts/customize_template.py`

Validate the draft after significant formatting edits rather than assuming compliance.

## Default Deliverables

When the user asks for venue adaptation without a strict format, return:
1. the inferred venue requirements
2. a template or asset recommendation
3. section-level revision advice
4. formatting risks and compliance checks
5. any open items that require the official venue package