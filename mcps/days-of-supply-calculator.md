# Days of Supply Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/days-of-supply-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/days-of-supply-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/days-of-supply-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Monitor inventory health by calculating stock coverage and identifying supply risks.

## Description
This MCP server provides specialized tools for inventory management. Use `get_sku_supply_metrics` to analyze individual items, `get_category_health_summary` to assess group performance, and `calculate_financial_exposure_by_tier` to identify capital tied up in overstock or at risk of stockout.


## Available Tools
- **get_category_health_summary**: Provides an aggregated view of inventory health for a specific group of items
- **calculate_financial_exposure_by_tier**: Calculates the total monetary value of inventory held within different coverage levels
- **get_sku_supply_metrics**: Calculates the specific supply duration and risk status for a single item


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Days of Supply Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the supply metrics for SKU 'S123' with 50 units in stock and a daily demand of 5."

**🤖 AI Agent:**
> The `get_sku_supply_metrics` tool shows that SKU 'S123' has 10 days of supply, which is considered a stable level.

---

**👤 You:**
> "Calculate the financial exposure for my inventory list."

**🤖 AI Agent:**
> The `calculate_financial_exposure_by_tier` tool has processed your items and identified the total value in critical, stable, and excess tiers.

---

**👤 You:**
> "Summarize the health of category 'Electronics'."

**🤖 AI Agent:**
> Using `get_category_health_summary`, the Electronics category shows 5 items at risk of stockout and 2 items in overstock.


## Installation & Usage

To install and use the **Days of Supply Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/days-of-supply-calculator](https://vinkius.com/mcp/days-of-supply-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
