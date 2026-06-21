# US Depreciation Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-depreciation-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/us-depreciation-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/us-depreciation-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate US asset depreciation using MACRS, Section 179, and Bonus Depreciation rules.

## Description
This MCP server provides AI agents with specialized tools to calculate complex US tax depreciation. Using `get_asset_class_info`, agents can retrieve recovery periods for different asset classes like vehicles or buildings. The `calculate_depreciation_schedule` tool generates a full year-by-year breakdown of expenses, accounting for Section 179 expensing and Bonus Depreciation. Additionally, `calculate_expensing_impact` allows agents to compare the immediate tax benefits of accelerated expensing methods against standard MACRS depreciation.


## Available Tools
- **calculate_depreciation_schedule**: Generate a year-by-year depreciation schedule
- **calculate_expensing_impact**: Compare the impact of Section 179 and Bonus Depreciation against standard MACRS
- **get_asset_class_info**: g., car, residential, commercial).

Get information about a specific asset class


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Depreciation Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the recovery period for a commercial building?"

**🤖 AI Agent:**
> You can find this by calling `get_asset_class_info` with 'commercial' as the asset class name.

---

**👤 You:**
> "Calculate a depreciation schedule for a car costing $30,000 with $5,000 Section 179 expensing."

**🤖 AI Agent:**
> The agent would use `calculate_depreciation_schedule` with 'car', an initial cost of 30000, and a section179Amount of 5000.

---

**👤 You:**
> "Show me the tax benefit impact for a $50,000 asset with 80% bonus depreciation."

**🤖 AI Agent:**
> The agent would use `calculate_expensing_impact` providing the cost, a bonusPercentage of 0.8, and any applicable Section 179 amount.


## Installation & Usage

To install and use the **US Depreciation Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-depreciation-calculator](https://vinkius.com/mcp/us-depreciation-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
