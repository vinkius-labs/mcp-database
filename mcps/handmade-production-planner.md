# Handmade Production Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/handmade-production-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Plan materials, labor, and profitability for artisanal production batches.

## Description
This MCP server provides a comprehensive planning engine for artisanal businesses. It connects AI agents to your production data, allowing them to calculate material needs, estimate labor hours, and predict financial outcomes. Use `get_material_requirements` to find raw material volumes, `get_labor_estimate` to plan staffing, `calculate_production_costs` to find total expenses, `estimate_profitability` to forecast margins, and `check_inventory_availability` to verify stock levels before starting a batch.


## Available Tools (5)
- **check_inventory_availability**: Verifies if enough raw materials are currently in stock to support the planned batch
- **estimate_profitability**: Predicts the financial outcome of a production run based on selling price
- **get_labor_estimate**: Calculates the total human time required to complete a batch
- **get_material_requirements**: Determines the total volume of raw materials needed for a specific production run
- **calculate_production_costs**: Aggregates all expenses including materials, packaging, and labor to find the cost of goods sold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Handmade Production Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many materials do I need to make 50 units of product_001?"

**🤖 AI Agent:**
> To produce 50 units of product_001, you will need 5.0 kg of Clay and 100 units of Glaze.

---

**👤 You:**
> "What is the total labor time for a batch of 10 ceramic mugs?"

**🤖 AI Agent:**
> The total labor required for a batch of 10 ceramic mugs is 15 hours.

---

**👤 You:**
> "Will I make a profit if I sell 20 units of product_002 at $25 each?"

**🤖 AI Agent:**
> Yes, selling 20 units at $25 each will result in a total profit of $150.00 with a profit margin of 30%.


## ❓ FAQ

**Q: How do I know if I have enough materials for a batch?**
You can use the `check_inventory_availability` tool to verify if your current stock can support the requested batch size.

**Q: Can I calculate the profit for a specific order?**
Yes, use the `estimate_profitability` tool by providing the product ID, batch size, and your intended selling price.

**Q: Does this include packaging costs?**
Yes, the `calculate_production_costs` tool aggregates material, packaging, and labor costs into a single total.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/handmade-production-planner](https://vinkius.com/en/ai-agent-connect/handmade-production-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Handmade Production Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `handmade-production-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Handmade Production Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "handmade-production-planner": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
