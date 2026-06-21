# Chi-Square Test Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chi-square-test-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chi-square-test-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chi-square-test-engine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Run exact Chi-Square independence tests on contingency tables local. Get CPU-guaranteed chi² statistics and p-values for categorical analysis.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chi-Square Test Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is there a statistically significant relationship between user gender and subscription tier?"

**🤖 AI Agent:**
> The Chi-Square test returns chi² = 8.42, df = 2, p-value = 0.015. Since p < 0.05, there is a statistically significant relationship between gender and subscription tier.

---

**👤 You:**
> "Check if the distribution of customer complaints varies by product category."

**🤖 AI Agent:**
> The p-value is 0.32. We cannot reject the null hypothesis — the complaint distribution appears independent of product category.

---

**👤 You:**
> "Run a chi-square test on this survey data to see if education level affects voting preference."

**🤖 AI Agent:**
> Chi² = 15.8, df = 6, p-value = 0.015. The result is statistically significant — education level and voting preference are not independent.


## Installation & Usage

To install and use the **Chi-Square Test Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chi-square-test-engine](https://vinkius.com/mcp/chi-square-test-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
