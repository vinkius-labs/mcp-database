# Retention Curve Analyzer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/retention-curve-analyzer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/retention-curve-analyzer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/retention-curve-analyzer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [product-management](../categories/product-management.md)

Analyze cohort retention curves to identify stability versus churn and compare against industry benchmarks.

## Description
The Retention Curve Analyzer is a specialized tool for product managers and growth engineers. It helps you understand user engagement by analyzing retention sequences to determine if your curve is `analyze_retention_trend` (flattening) or `classify_curve_pattern` (declining). By using `verify_benchmark_compliance`, you can compare your actual D1, D7, D30, and D90 metrics against hardcoded industry standards for SaaS, Mobile Gaming, and E-commerce. This allows you to identify 'Smiling Curves' that signify healthy long-term retention versus 'Declining Curves' that indicate high churn risk.


## Available Tools
- **analyze_retention_trend**: Determines if a retention sequence is flattening or declining
- **classify_curve_pattern**: Classifies the retention curve pattern
- **verify_benchmark_compliance**: Compares cohort metrics against industry benchmarks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Retention Curve Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is my retention curve flattening or declining? Here are the values: [100, 50, 30, 25, 22]"

**🤖 AI Agent:**
> The retention curve is Flattening. The recent drop from 25 to 22 is minimal, indicating the curve has reached a plateau.

---

**👤 You:**
> "Check if my SaaS product meets D7 benchmarks. My D1 is 40% and D7 is 20%."

**🤖 AI Agent:**
> The compliance report shows that your D7 metric failed to meet the SaaS benchmark.

---

**👤 You:**
> "What pattern does this sequence represent: [100, 80, 60, 40, 20, 5]?"

**🤖 AI Agent:**
> The pattern is classified as Declining because the sequence shows a continuous downward trend approaching zero.


## Installation & Usage

To install and use the **Retention Curve Analyzer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/retention-curve-analyzer](https://vinkius.com/mcp/retention-curve-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
