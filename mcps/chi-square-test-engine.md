# Chi-Square Test Engine MCP Server

Run exact Chi-Square independence tests on contingency tables local. Get CPU-guaranteed chi² statistics and p-values for categorical analysis.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/chi-square-test-engine)

## Overview
**Category:** data-analytics
**Tools Count:** 1

## Description
The Chi-Square test determines whether two categorical variables are independent. Asking an LLM to compute expected frequencies across a matrix and then sum the chi² residuals is a recipe for hallucinated results.

This MCP computes the full test deterministically using `jstat`. The AI sends the observed frequency matrix, and the engine calculates exact expected frequencies, the chi² statistic, degrees of freedom, and the p-value — all locally on your CPU.

### The Superpowers

- **Zero Hallucination:** Exact chi² statistics computed deterministically.
- **Automatic Expected Frequencies:** The engine builds the entire expected matrix internally.
- **Any Matrix Size:** Supports 2x2, 3x3, or larger contingency tables.
- **Data Privacy:** Your survey and business data stays local.


## Available Tools
- **calculate_chi_square**: Perform exact deterministic Chi-Square tests of independence on categorical contingency tables without LLM math hallucinations


## Installation & Usage

To install and use the **Chi-Square Test Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chi-square-test-engine](https://vinkius.com/mcp/chi-square-test-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
