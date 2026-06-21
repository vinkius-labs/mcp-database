# ABC-XYZ Inventory Classifier MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/abc-xyz-inventory-classifier)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/abc-xyz-inventory-classifier-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/abc-xyz-inventory-classifier-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Classify inventory items by value (ABC) and demand stability (XYZ) to optimize management strategies.

## Description
This MCP server provides advanced inventory intelligence by performing multi-dimensional classification of stock items. It intersects ABC analysis (economic impact based on annual consumption value) with XYZ analysis (demand predictability based on historical volatility). By using tools like `classify_abc_priority`, `classify_xyz_stability`, and `get_strategy_matrix`, users can identify high-value, stable items for JIT replenishment and low-value, irregular items that require safety stock buffers. It transforms raw SKU data into actionable management policies.


## Available Tools
- **classify_abc_priority**: Classify SKUs into ABC categories based on cumulative value
- **get_strategy_matrix**: Generate management strategies by intersecting ABC and XYZ results
- **classify_xyz_stability**: Classify SKUs into XYZ categories based on demand volatility


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ABC-XYZ Inventory Classifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Classify these SKUs by value: [{'id': 'SKU001', 'value': 5000}, {'id': 'SKU002', 'value': 100}, {'id': 'SKU003', 'value': 50}]"

**🤖 AI Agent:**
> [{"id": "SKU001", "category": "A"}, {"id": "SKU002", "category": "B"}, {"id": "SKU003", "category": "C"}]

---

**👤 You:**
> "Check the stability of SKU-99 with demand history: [10, 12, 11, 10, 13]"

**🤖 AI Agent:**
> [{"id": "SKU-99", "category": "X"}]

---

**👤 You:**
> "What is the strategy for an item that is Class A in value and Class Z in stability?"

**🤖 AI Agent:**
> For AZ items, the recommended policy is 'High-value, irregular demand: Requires strict control and safety stock buffers to prevent stockouts.'


## Installation & Usage

To install and use the **ABC-XYZ Inventory Classifier** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/abc-xyz-inventory-classifier](https://vinkius.com/mcp/abc-xyz-inventory-classifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
