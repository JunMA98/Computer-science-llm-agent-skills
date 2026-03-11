---
name: torch-geometric
description: Build graph neural network workflows with PyTorch Geometric for CS research. Use when training GNNs for citation networks, knowledge graphs, recommender graphs, code graphs, program analysis, heterogeneous graphs, node or graph classification, or link prediction with scalable mini-batching and graph transforms.
---

# PyTorch Geometric

Use this skill when the task is graph representation learning rather than general graph analytics.

## Common CS Uses

- node classification on citation or dependency graphs
- graph classification for program, document, or interaction structures
- link prediction for recommendation or knowledge graph completion
- heterogeneous graph learning
- graph mini-batching, sampling, and transform pipelines

## Local Resources

- `references/datasets_reference.md`
- `references/layers_reference.md`
- `references/transforms_reference.md`
- `scripts/create_gnn_template.py`
- `scripts/benchmark_model.py`
- `scripts/visualize_graph.py`

## Working Rules

- Define graph construction and supervision targets explicitly.
- Check whether edge direction, heterogeneity, and sampling strategy affect the conclusion.
- Compare against strong non-GNN baselines when appropriate.
- Use graph visualization only to clarify structure, not as proof of performance.

## Default Output

When the user asks for PyG help without more detail, return:
1. task formulation
2. suitable model family or layer choices
3. data pipeline considerations
4. evaluation and baseline notes