---
name: statsmodels
description: Fit statistical models with detailed inference and diagnostics for CS experiments, telemetry, time series, and structured evaluations. Use when you need OLS, GLM, mixed models, logistic regression, count models, or time-series analysis with coefficient tables, residual checks, and interpretable model summaries.
---

# Statsmodels

Use this skill when the task requires explicit statistical modeling and interpretable diagnostics rather than black-box prediction.

## Good Fits

- regression on experimental factors or system settings
- logistic or count models for outcome analysis
- mixed models for repeated measurements or participant-level data
- time-series analysis for latency, throughput, or operational logs
- inference-heavy analyses where coefficient interpretation matters

## Local References

- `references/linear_models.md`
- `references/glm.md`
- `references/discrete_choice.md`
- `references/stats_diagnostics.md`
- `references/time_series.md`

## Working Rules

- Match the model family to the data-generating process.
- Inspect residuals and diagnostics before trusting coefficients.
- Prefer simpler models when interpretation is the goal.
- Use `statistical-analysis` first if the main task is test selection rather than model fitting.

## Default Output

When the user asks for modeling help without more detail, return:
1. model family recommendation
2. required variables and assumptions
3. diagnostics to inspect
4. how to report the results clearly