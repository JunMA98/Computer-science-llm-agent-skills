---
name: github-release-prep
description: Use when preparing a project for public GitHub release and you need to verify docs, licenses, notices, examples, repository hygiene, and release readiness.
---

# Purpose

Prepare a repository for public release without leaking private material or publishing an incoherent project.

# When To Use

- before making a repo public on GitHub
- before tagging a first release or sharing with external users
- when checking whether docs, licensing, and examples are complete
- when converting an internal research repo into a public artifact

# Inputs

- repository state and release target
- current README, docs, notices, and attribution files
- known restrictions on data, checkpoints, credentials, or third-party assets

# Outputs

- release-readiness checklist
- documentation and legal gap list
- example/demo packaging checklist
- release note outline and final blocking issues
- explicit publish versus do-not-publish inventory

# Workflow

1. Verify the project story, audience, and minimal runnable entry point.
2. Check README, docs, examples, and environment instructions.
3. Audit license, notice, attribution, secrets, data, and model assets.
4. Confirm that the visible repository structure matches the public story.
5. Produce final blockers before release instead of assuming readiness.

# Constraints

- do not assume internal code or data is publishable
- treat missing attribution or unclear licensing as blockers
- separate polish issues from hard release blockers
- optimize for public clarity, not internal convenience