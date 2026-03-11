---
name: exploratory-data-analysis
description: Explore and summarize computer science research data, experiment outputs, benchmark tables, logs, embeddings, predictions, and dataset files. Use when inspecting CSV, JSON, Parquet, NPY, NPZ, HDF5, TXT logs, or similar files to understand structure, quality, anomalies, and next analysis steps before modeling, benchmarking, or paper writing.
---

# Exploratory Data Analysis

Use this skill for CS-oriented exploratory analysis. Prioritize findings that change research decisions: data leakage, broken runs, missing baselines, bad splits, unstable metrics, or misleading aggregates.

## Typical CS Inputs

Handle cases such as:
- dataset tables and metadata exports
- train / validation / test split files
- experiment logs and seed-wise result tables
- benchmark leaderboards or ablation summaries
- model predictions, error cases, and prompt-response pairs
- embeddings, hidden states, graph statistics, or feature arrays
- system measurement logs: latency, throughput, memory, failure counts

## Start by Defining the Unit of Analysis

Before computing summaries, identify what one row, item, run, or file represents:
- sample
- document
- graph
- query
- experiment run
- model checkpoint
- hardware configuration
- user session

Many bad EDA conclusions come from mixing these levels.

## Workflow

### 1. Inspect structure
- file format, size, schema, and obvious parsing issues
- column meanings or tensor shapes
- join keys, IDs, timestamps, seeds, or split labels

Use `scripts/eda_analyzer.py` for an initial scan when it helps, but do not stop at generic summaries.

### 2. Check quality and validity
- missing values and malformed records
- duplicates and near-duplicates
- inconsistent label or split assignments
- impossible values, broken timestamps, or corrupted runs
- class or task imbalance
- train-test leakage or benchmark contamination indicators

### 3. Analyze the distributions that matter
- label frequencies and long-tail behavior
- sequence or prompt length distributions
- metric spread across runs or seeds
- runtime, memory, or throughput variance
- embedding norms, sparsity, or dimensional anomalies
- subgroup or slice behavior that averages may hide

### 4. Look for decision-relevant anomalies
- runs that dominate an average because of one seed
- missing baseline rows in supposedly complete tables
- data slices where the model collapses
- evaluation artifacts caused by filtering, truncation, or deduplication
- suspiciously easy splits or repeated examples across partitions

### 5. Produce next-step guidance
Recommend concrete follow-up actions such as:
- relabel or deduplicate data
- redesign splits
- rerun incomplete experiments
- aggregate by seed with mean and variance
- add subgroup evaluation
- investigate outliers or failure slices
- prepare cleaned tables for paper figures

## Preferred Local Resources

Use these inherited resources selectively:
- `references/general_scientific_formats.md` for common table/array formats
- `assets/report_template.md` when a markdown analysis report is requested
- `scripts/eda_analyzer.py` for quick initial parsing

The bio/chem/imaging references remain available from upstream, but for this curated repo they are secondary. Only load them if the actual data format requires them.

## Output Formats

Choose an output that matches the task:
- concise EDA memo
- benchmark readiness report
- run-quality audit
- dataset issue list
- error analysis summary
- preprocessing plan
- paper-ready results summary with caveats

## Default Output

When the user asks to explore a file or result table without more detail, return:
1. what the data appears to represent
2. the most important structure and quality findings
3. anomalies or risks that affect conclusions
4. recommended next analyses or cleanup steps