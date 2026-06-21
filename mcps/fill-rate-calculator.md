# Fill Rate Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fill-rate-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fill-rate-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fill-rate-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Calculate Order, Line, and Unit Fill Rate metrics along with stockout costs.

## Description
This MCP server provides essential logistics performance tools to measure supply chain efficiency. Use `calculate_fill_rate_metrics` to determine Order, Line, and Unit Fill Rates from raw fulfillment data. The `estimate_stockout_impact` tool quantifies the financial loss and potential NPS degradation caused by unfulfilled orders. Additionally, `compare_to_benchmarks` allows you to evaluate your current performance against industry-specific targets for sectors like retail, pharmaceutical, electronics, and food & beverage.


## Available Tools
- **calculate_fill_rate_metrics**: Calculate Order, Line, and Unit Fill Rate metrics
- **compare_to_benchmarks**: Evaluate performance against industry benchmarks
- **estimate_stockout_impact**: Quantify the financial and reputational damage of unfulfilled demand


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fill Rate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my fill rates for 100 total orders, 85 completed orders, 120 total lines, 100 completed lines, 500 units requested, and 450 units delivered."

**🤖 AI Agent:**
> The calculation results are: Order Fill Rate: 85.0%, Line Fill Rate: 83.3%, and Unit Fill Rate: 90.0%.

---

**👤 You:**
> "What is the financial impact of having 10 unfilled orders at a cost of $50 each with a high severity level?"

**🤖 AI Agent:**
> The total estimated stockout cost is $500, and the potential NPS impact is classified as 'high', indicating a significant risk of brand damage.

---

**👤 You:**
> "Compare my current unit fill rate of 85% against the pharmaceutical sector benchmark."

**🤖 AI Agent:**
> For the pharmaceutical sector, the benchmark is higher than your current 85%. Your performance status is 'Critical Failure'.


## Installation & Usage

To install and use the **Fill Rate Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fill-rate-calculator](https://vinkius.com/mcp/fill-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
