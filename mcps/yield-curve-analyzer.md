# Yield Curve Analyzer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yield-curve-analyzer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/yield-curve-analyzer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/yield-curve-analyzer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze interest rate curves, identify spreads, and detect recession signals.

## Description
The Yield Curve Analyzer is a specialized tool for financial professionals to interpret the shape of the yield curve. By using `calculate_curve_metrics`, you can determine if the market is in a Normal, Inverted, Flat, or Humped state and calculate critical spreads like 2s10s and 3m10a. The engine also provides deep insights into economic stability via `examine_recession_risk` to detect potential recessionary signals from yield inversions. Finally, use `get_allocation_guidance` to receive actionable investment strategies and target duration ranges based on the current market environment.


## Available Tools
- **get_allocation_guidance**: Get investment allocation guidance
- **calculate_curve_metrics**: Calculate yield curve metrics
- **examine_recession_risk**: Examine yield curve inversion for recession risk


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yield Curve Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current state of the yield curve if 3m is 4%, 2y is 4.5%, and 10y is 4.2%?"

**🤖 AI Agent:**
> The yield curve is currently classified as Inverted, with a significant spread inversion detected.

---

**👤 You:**
> "Calculate the spreads for these rates: 3m=3.5%, 6m=3.6%, 1y=3.8%, 2y=4.0%, 5y=4.2%, 10y=4.5%, 30y=4.7%."

**🤖 AI Agent:**
> The classification is Normal, with a 2s10s spread of 0.5000% and a 3m10a spread of 1.0000%.

---

**👤 You:**
> "What strategy should I use if the curve is inverted?"

**🤖 AI Agent:**
> For an Inverted curve, you should follow a Short Duration Strategy with a target duration range focused on lower maturity windows.


## Installation & Usage

To install and use the **Yield Curve Analyzer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yield-curve-analyzer](https://vinkius.com/mcp/yield-curve-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
