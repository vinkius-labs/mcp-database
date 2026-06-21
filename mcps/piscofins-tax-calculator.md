# PIS/COFINS Tax Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/piscofins-tax-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/piscofins-tax-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/piscofins-tax-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate PIS and COFINS tax liabilities for cumulative and non-cumulative regimes.

## Description
This MCP server provides specialized tools to calculate Brazilian social contributions (PIS and COFINS). Use `calculate_cumulative_tax` for simplified taxation with fixed rates, `calculate_non_cumulative_tax` to account for input credits in the complex regime, or `evaluate_regime_comparison` to determine the most tax-efficient method based on your revenue and operational costs.


## Available Tools
- **calculate_cumulative_tax**: Calculate PIS and COFINS liability under the cumulative regime
- **calculate_non_cumulative_tax**: Calculate net PIS and COFINS liability under the non-cumulative regime
- **evaluate_regime_comparison**: Compare cumulative and non-cumulative taxation regimes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PIS/COFINS Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my PIS/COFINS for 100,000 BRL revenue in the cumulative regime."

**🤖 AI Agent:**
> The `calculate_cumulative_tax` tool would return a PIS amount of 650.00 and COFINS of 3,000.00, totaling 3,650.00.

---

**👤 You:**
> "Compare regimes for 500,000 BRL revenue with 50,000 BRL in raw material costs."

**🤖 AI Agent:**
> Using `evaluate_regime_comparison`, the tool will analyze both regimes and suggest the one with the lowest net liability based on your input credits.

---

**👤 You:**
> "What is my tax liability if I have 200,000 BRL revenue and 20,000 BRL in energy costs?"

**🤖 AI Agent:**
> By calling `calculate_non_cumulative_tax` with the provided input credits, you can see your net PIS and COFINS balance.


## Installation & Usage

To install and use the **PIS/COFINS Tax Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/piscofins-tax-calculator](https://vinkius.com/mcp/piscofins-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
