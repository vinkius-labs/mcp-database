# Normality Test Engine MCP Server

Test whether your data is normally distributed using Skewness and Kurtosis analysis local. Essential pre-check before running parametric statistical tests.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/normality-test-engine)

## Overview
**Category:** developer-tools
**Tools Count:** 1

## Description
Before running t-tests, ANOVA, or linear regression, you need to verify that your data is normally distributed. LLMs cannot eyeball a distribution from raw numbers — they will guess and often guess wrong.

This MCP uses `simple-statistics` to compute exact Skewness and Kurtosis coefficients, then applies a Jarque-Bera test to determine normality. The AI gets a definitive pass/fail verdict with the exact test statistic and p-value.

### The Superpowers

- **Zero Hallucination:** Exact statistical coefficients computed locally.
- **Automated Verdict:** Returns a clear 'normal' or 'not normal' interpretation.
- **Descriptive Statistics:** Also provides exact Mean, Std Dev, Skewness, and Kurtosis.
- **Data Privacy:** Your research data stays entirely on your local machine.


## Available Tools
- **test_normality**: Perform an exact deterministic Jarque-Bera normality test on numeric data without LLM math hallucinations


## Installation & Usage

To install and use the **Normality Test Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/normality-test-engine](https://vinkius.com/mcp/normality-test-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
