---
name: get-available-resources
description: Detect available CPU, GPU, memory, and disk resources before compute-heavy CS work. Use when planning model training, large-scale evaluation, embedding generation, experiment sweeps, dataset processing, log analysis, or reproduction runs where hardware limits affect the workflow.
---

# Get Available Resources

Use this skill early in a CS workflow when hardware constraints may change the implementation plan.

## Typical Triggers

- choosing between in-memory and out-of-core data processing
- checking whether a model fits on available GPU memory
- sizing parallel workers for preprocessing or evaluation
- deciding whether to run locally, distribute with Dask, or move to Modal
- estimating whether a reproduction or benchmark sweep is realistic on the current machine

## Workflow

1. Run `scripts/detect_resources.py` to collect CPU, GPU, memory, and disk information.
2. Save or inspect the generated JSON report.
3. Translate the report into execution choices.
4. State the constraints explicitly before proposing a heavy workflow.

## CS-Focused Decisions

Map resource findings to concrete tool choices:
- fits in RAM: prefer `polars`, `pandas`, or standard PyTorch workflows
- exceeds RAM on one machine: consider `dask` or `vaex`
- limited local GPU but scalable remote need: consider `modal`
- multi-GPU or long training runs: plan around `pytorch-lightning` or distributed tooling
- low disk headroom: avoid materializing large intermediate checkpoints or duplicated datasets

## What to Report

By default, summarize:
- CPU cores and whether high parallelism is realistic
- available GPUs, VRAM, and likely model-size limits
- total RAM and whether dataset / checkpoint loading is safe
- free disk space and likely pressure points
- practical recommendations for the current task

## Default Output

When no exact format is requested, return:
1. a concise resource summary
2. the main bottlenecks
3. recommended execution strategy
4. any risk to training, evaluation, or large-file processing