---
name: umap-learn
description: Reduce and visualize high-dimensional representations for CS experiments. Use when exploring embeddings, hidden states, feature vectors, retrieval spaces, clustering structure, error slices, or representation drift in model outputs and benchmark data.
---

# UMAP-Learn

Use this skill when a lower-dimensional view can reveal structure that summary statistics hide.

## Good Fits

- visualize embedding spaces from NLP, vision, or multimodal models
- inspect class or error clusters
- compare representations across checkpoints or training stages
- preprocess features before clustering or nearest-neighbor analysis
- explore dataset shift or failure slices

## Local References

- `references/api_reference.md`

## Working Rules

- Standardize or normalize inputs when the metric requires it.
- Do not over-interpret 2D layouts as proof of causal structure.
- Compare multiple seeds or parameter settings when the geometry matters.
- Use labels, slices, or metadata overlays to interpret clusters responsibly.

## Default Output

When the user asks for UMAP help without more detail, return:
1. recommended preprocessing
2. parameter considerations
3. visualization and interpretation notes
4. likely pitfalls