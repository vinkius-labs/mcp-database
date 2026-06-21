# Data Analysis Prover MCP Server

A marketing team asked an AI to analyze campaign data. The AI reported 'significant correlation between email frequency and purchase rate (p<0.05).' The team tripled emails. Unsubscribes spiked 340%. Sample: N=47 self-selected respondents, no power analysis. Correlation: observational, no confounders. Distribution: right-skewed but mean used. p=0.043 but Cohen's d=0.12 — trivial. Chart: truncated Y-axis making a 2% difference look enormous. This tool forces five axes: sample validity, causal inference, distribution awareness, significance with effect size, and visualization integrity.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/data-analysis-prover)

## Overview
**Category:** data science
**Tools Count:** 1

## Description
## The Problem

1. **Sample Blindness** — no N, no power analysis, no selection method check.
2. **Correlation Confusion** — causal claims from observational data.
3. **Distribution Ignorance** — mean on skewed data, wrong test choice.
4. **Significance Theater** — p-value without effect size or practical meaning.
5. **Visualization Deception** — truncated axes, dual scales, misleading charts.


## Available Tools
- **validate_data_analysis**: Think like a senior statistician peer-reviewing a paper — every claim must survive scrutiny on sample quality, causal validity, distributional assumptions, practical significance, and visual honesty. You must: (1) validate SAMPLE — report N, conduct power analysis (what effect size can you detect?), describe selection method (random, stratified, convenience), assess representativeness (who is missing?), handle missing data explicitly (listwise deletion, imputation, or sensitivity analysis), (2) test CAUSALITY — name confounders and how they are controlled, test reverse causality, distinguish experimental from observational, check dose-response where applicable. "X causes Y" requires experimental evidence or rigorous causal inference. "X correlates with Y" is the honest claim from observational data, (3) check DISTRIBUTION — visualize shape before choosing tests, identify outliers (>3 SD or IQR method), test normality (Shapiro-Wilk for N<50, K-S for larger), choose parametric vs non-parametric accordingly, report median + IQR for skewed data instead of mean + SD, (4) report SIGNIFICANCE properly — effect size (Cohen's d, r², odds ratio) alongside p-value, 95% confidence intervals, practical significance assessment, Bonferroni or FDR correction for multiple comparisons. p < 0.05 alone is not meaningful without effect size, (5) ensure VISUALIZATION honesty — Y-axis starts at zero (or justified if not), no dual Y-axes (they always mislead), no 3D charts (they distort proportions), lie factor between 0.95-1.05, consistent aggregation periods, no cherry-picked timeframes. If rejected, your analysis has a methodological flaw.

Structured reflection tool for rigorous statistical analysis — senior statistician level. Forces the agent to validate sample quality, prove causal inference, check distributions, report effect sizes alongside p-values, and ensure visualization honesty. Catches Sample Blindness (no N, no power analysis, convenience sampling presented as representative — "we surveyed 12 users" without statistical power to detect meaningful effects), Correlation Confusion (causal claims from observational data — "X causes Y" when confounders are uncontrolled, reverse causality untested, and no experimental design exists), Distribution Ignorance (mean on skewed data, parametric tests on non-normal distributions — reporting "average salary $85K" when median is $52K and distribution is right-skewed), Significance Theater (p < 0.05 without effect size — a statistically significant but trivially small effect is not practically significant. Cohen's d = 0.02 with p = 0.001 means nothing useful), and Visualization Deception (truncated Y-axis, dual scales, 3D charts, cherry-picked timeframes — lie factor >1.05 distorts reader perception of magnitude). Call once per data analysis, statistical claim, or research interpretation


## Installation & Usage

To install and use the **Data Analysis Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/data-analysis-prover](https://vinkius.com/mcp/data-analysis-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
