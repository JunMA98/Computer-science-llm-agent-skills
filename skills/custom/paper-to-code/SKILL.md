---
name: paper-to-code
description: Use when implementing a paper, method, or system from a publication and you need to translate claims, methods, and diagrams into an executable implementation plan.
---

# Purpose

Convert a paper into a concrete implementation roadmap without hiding ambiguities.

# When To Use

- implementing a method from a paper or preprint
- turning a paper idea into a prototype or baseline
- extracting architecture, training, and evaluation details from text
- estimating what is missing before starting reproduction or extension work

# Inputs

- paper, notes, figures, appendices, or pseudo-code
- any released repo, checkpoint, or supplemental material if available
- target implementation scope and resource constraints

# Outputs

- implementation map from paper components to code modules
- list of explicit versus inferred details
- dependency order for coding tasks
- acceptance tests tied to paper claims
- list of missing assumptions or ambiguous steps

# Workflow

1. Extract the paper's main claims and component boundaries.
2. Convert each contribution into modules, data flow, and interfaces.
3. Separate paper-stated details from inferred implementation choices.
4. Define a build order that reaches a testable baseline early.
5. Tie implementation milestones back to paper claims and evaluation targets.

# Constraints

- do not present inferred details as if the paper explicitly stated them
- keep reproduction goals separate from extension goals
- prefer the simplest faithful baseline before optimization
- record ambiguities early so they do not disappear into code guesses