# Normality Test Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/normality-test-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/normality-test-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/normality-test-engine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Test whether your data is normally distributed using Skewness and Kurtosis analysis local. Essential pre-check before running parametric statistical tests.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Normality Test Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this residuals array is normally distributed before I run my regression."

**🤖 AI Agent:**
> The Jarque-Bera test returns p = 0.42. We fail to reject the normality hypothesis — your residuals appear normally distributed. Proceed with the regression.

---

**👤 You:**
> "Is this sensor data normally distributed or should I use a non-parametric test?"

**🤖 AI Agent:**
> The data shows significant positive skewness (1.8) and high kurtosis (5.2). The Jarque-Bera p-value is 0.001 — the data is not normally distributed. Use a non-parametric test.

---

**👤 You:**
> "Run a normality test on the 'Revenue' column before I calculate confidence intervals."

**🤖 AI Agent:**
> Normality test passed (p = 0.61). Skewness is 0.3 and kurtosis is 2.9 — both close to normal parameters. Your confidence intervals will be valid.


## Installation & Usage

To install and use the **Normality Test Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/normality-test-engine](https://vinkius.com/mcp/normality-test-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
