---
name: sympy
description: Use symbolic math in Python for CS research and algorithm work. Use when deriving formulas, simplifying objectives, solving recurrences or equations, manipulating matrices symbolically, generating exact expressions, or turning mathematical derivations into executable code.
---

# SymPy

Use this skill when exact symbolic reasoning is more valuable than numerical approximation.

## Common CS Uses

- derive loss functions or gradients
- simplify probabilistic or optimization expressions
- solve recurrences or closed forms in algorithm analysis
- manipulate matrices symbolically
- generate LaTeX for proofs, notes, or papers
- generate code from symbolic expressions

## Local References

- `references/core-capabilities.md`
- `references/matrices-linear-algebra.md`
- `references/code-generation-printing.md`
- `references/advanced-topics.md`
- `references/physics-mechanics.md` only if the task truly needs it

## Working Rules

- Keep expressions symbolic as long as that improves insight.
- Switch to numerical evaluation only after the derivation is stable.
- Prefer exact simplification when comparing formulations.
- Document assumptions on domains, positivity, or integrality when they affect the result.

## Default Output

When the user asks for symbolic help without a specific format, return:
1. the symbolic setup
2. the derived or simplified result
3. assumptions used
4. code or LaTeX if that helps downstream use