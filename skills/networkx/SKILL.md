---
name: networkx
description: Build and analyze graphs in Python for CS research and engineering tasks. Use when working with citation graphs, dependency graphs, call graphs, knowledge graphs, agent tool graphs, communication networks, or any problem involving nodes, edges, graph algorithms, or network structure.
---

# NetworkX

Use this skill for graph analysis that benefits from flexible Python-native data structures and readable algorithms.

## Common CS Uses

- citation or collaboration graph analysis
- package dependency and call-graph analysis
- knowledge graph or heterogeneous relation prototyping
- graph features for downstream ML pipelines
- path analysis in workflows, state machines, or tool graphs
- synthetic graph generation for experiments or teaching

## Workflow

1. Define what nodes and edges represent.
2. Attach attributes only when they affect the analysis.
3. Choose the graph type: directed, undirected, multigraph, weighted, or heterogeneous approximation.
4. Run the algorithms that answer the actual research question.
5. Export or visualize only after the graph semantics are clear.

## Local References

Read only what is needed:
- `references/graph-basics.md`
- `references/algorithms.md`
- `references/io.md`
- `references/generators.md`
- `references/visualization.md`

## Practical Guidance

- Use NetworkX for clarity and experimentation, not maximum scale.
- For very large graphs, use it for prototyping, sampling, or analysis on reduced representations.
- Be explicit about directedness, edge weights, and disconnected components.
- Do not assume a graph metric is meaningful unless it matches the graph semantics.

## Default Output

When the user asks for graph help without a fixed format, return:
1. the graph model being assumed
2. the algorithms or metrics to compute
3. interpretation notes and likely pitfalls