# Export Parity Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/export-parity-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/export-parity-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/export-parity-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the net farm-gate price for grain exports by accounting for logistics and taxes.

## Description
This MCP server provides tools to determine the profitability of exporting commodities like grains. By using `get_transportation_rate`, you can find the cost per kilometer for different transport modes. The `calculate_farm_gate_parity` tool computes the final net price at the farm after subtracting freight, port fees, and export taxes from the international FOB price. Finally, use `analyze_market_opportunity` to compare this parity price against domestic market prices to decide whether to export or sell locally.


## Available Tools
- **calculate_farm_gate_parity**: Calculate the net price received at the farm after logistics costs
- **analyze_market_opportunity**: Analyze if export or domestic market is more profitable
- **get_transportation_rate**: Get the transport rate per km for a specific mode


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Export Parity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the transport rate for a truck?"

**🤖 AI Agent:**
> The `get_transportation_rate` tool returns the cost per km and currency for the selected mode.

---

**👤 You:**
> "Calculate parity: FOB $500, Rate 5.2, Distance 500km, Mode truck, Port Fees 100, Taxes 50."

**🤖 AI Agent:**
> Using `calculate_farm_gate_parity`, the tool will compute the net farm-gate price after all deductions.

---

**👤 You:**
> "Should I export if my parity is 2500 and domestic price is 2400?"

**🤖 AI Agent:**
> The `analyze_market_opportunity` tool will recommend 'EXPORT' because the parity price is higher.


## Installation & Usage

To install and use the **Export Parity Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/export-parity-calculator](https://vinkius.com/mcp/export-parity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
