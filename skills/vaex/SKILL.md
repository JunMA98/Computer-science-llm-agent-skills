---
name: vaex
description: Process very large tabular data for CS experiments and engineering logs without loading everything into RAM. Use when working with massive result tables, telemetry, predictions, feature exports, ranking data, or other large CSV, HDF5, Arrow, or Parquet files that need fast lazy aggregation and filtering.
---

# Vaex

Use this skill when dataset size exceeds comfortable in-memory workflows but you still want DataFrame-style analysis.

## Common CS Uses

- analyze large experiment logs or sweep outputs
- inspect ranking or retrieval results at scale
- aggregate telemetry, latency, or failure-event tables
- process feature exports or prediction dumps too large for RAM
- build lightweight big-table analysis pipelines

## Local References

- `references/core_dataframes.md`
- `references/data_processing.md`
- `references/io_operations.md`
- `references/performance.md`
- `references/visualization.md`
- `references/machine_learning.md`

## Working Rules

- Keep transformations lazy as long as possible.
- Materialize only the slices needed for downstream modeling or plotting.
- Use Vaex for big-table filtering and aggregation, then hand smaller outputs to plotting or modeling tools.
- Be explicit about file formats and column types early to avoid costly conversions.

## Default Output

When the user asks for Vaex help without more detail, return:
1. recommended data-loading strategy
2. likely lazy operations to use
3. performance and memory notes
4. downstream handoff advice