# ABC-XYZ Inventory Classifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/abc-xyz-inventory-classifier)
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


## ❓ FAQ

**Q: How does the ABC classification work?**
The `classify_abc_priority` tool calculates the total annual consumption value of all SKUs. It then sorts them from highest to lowest and assigns categories: A (top 80% value), B (next 15%), and C (remaining 5%).

**Q: What is the purpose of XYZ analysis?**
The `classify_xyz_stability` tool measures demand volatility. It uses the coefficient of variation (standard deviation divided by the mean) to categorize items as X (stable), Y (variable), or Z (irregular).

**Q: How can I generate management recommendations?**
Use the `get_strategy_matrix` tool by providing the outputs from both ABC and XYZ classifications. It will intersect the results to provide specific policies like 'High precision replenishment' for AX items.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/abc-xyz-inventory-classifier](https://vinkius.com/mcp/abc-xyz-inventory-classifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ABC-XYZ Inventory Classifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `abc-xyz-inventory-classifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ABC-XYZ Inventory Classifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "abc-xyz-inventory-classifier": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
