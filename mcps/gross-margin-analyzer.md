# Gross Margin Analyzer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gross-margin-analyzer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gross-margin-analyzer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gross-margin-analyzer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate product gross margins, identify underperforming products against industry benchmarks, and simulate COGS reduction impact.

## Description
The Gross Margin Analyzer is a financial diagnostic tool designed to evaluate product profitability. It allows you to compute gross margins for multiple products using `calculate_product_margins`, identify which items are falling below industry-specific thresholds with `detect_underperforming_products` (supporting SaaS, Marketplace, and Hardware benchmarks), and forecast the impact of cost optimization strategies via `simulate_cogs_savings_impact`.


## Available Tools
- **calculate_product_margins**: Compute the current profitability margin for a provided list of products
- **detect_underperforming_products**: Identify products failing to meet industry minimum profitability thresholds
- **simulate_cogs_savings_impact**: Forecast projected gross margin improvement from COGS reduction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gross Margin Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate margins for products A and B with revenue 100/cogs 30 and revenue 200/cogs 50."

**🤖 AI Agent:**
> Product A: 70.0%, Product B: 75.0%

---

**👤 You:**
> "Which of these products are underperforming in the SaaS industry? Margins: A (80%), B (65%)."

**🤖 AI Agent:**
> Product B is at risk because its margin of 65% is below the SaaS threshold of 70%.

---

**👤 You:**
> "If I reduce COGS by 10% for a product with 50 revenue and 40 COGS, what is the new margin?"

**🤖 AI Agent:**
> The projected gross margin will be 64.0%, an increase of 4.0 percentage points.


## Installation & Usage

To install and use the **Gross Margin Analyzer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gross-margin-analyzer](https://vinkius.com/mcp/gross-margin-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
