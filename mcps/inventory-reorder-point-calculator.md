# Inventory Reorder Point Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/inventory-reorder-point-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Calculate precise reorder points and replenishment quantities to prevent stockouts.

## Description
This MCP server provides essential inventory management tools to maintain optimal stock levels. Use `calculate_reorder_point` to determine when to trigger new orders based on sales velocity and lead time, and `calculate_reorder_quantity` to find the exact number of units needed to reach your target stock level. It also includes tools to `get_demand_during_lead_time` and `analyze_stockout_risk` to ensure your supply chain remains resilient.


## Available Tools (4)
- **analyze_stockout_risk**: Evaluates if current inventory levels are sufficient based on demand and lead time
- **calculate_reorder_point**: Determines the inventory threshold at which a replenishment order must be placed
- **calculate_reorder_quantity**: Determines the specific amount of stock to purchase when the reorder point is reached
- **get_demand_during_lead_time**: Calculates the total expected sales during the period a supplier is processing and delivering an order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Inventory Reorder Point Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my reorder point if I sell 10 units a day and it takes 5 days for new stock to arrive, with a safety stock of 20 units?"

**🤖 AI Agent:**
> Your reorder point is 70 units.

---

**👤 You:**
> "I have reached my reorder point of 50 units. I want to reach a target stock level of 200 units. How many should I order?"

**🤖 AI Agent:**
> You should order 150 units.

---

**👤 You:**
> "I have 30 units in stock. I sell 5 units a day and my lead time is 10 days. Am I at risk of a stockout?"

**🤖 AI Agent:**
> Yes, you are at risk of a stockout. You have 6 days of sales remaining.


## ❓ FAQ

**Q: How do I know when to reorder stock?**
You can use the `calculate_reorder_point` tool. By providing your average daily sales and supplier lead time, the tool calculates the exact inventory level that signals a need for replenishment.

**Q: Can I calculate how much stock to buy?**
Yes, the `calculate_reorder_quantity` tool determines the specific number of units to order to reach your desired target stock level once the reorder point is hit.

**Q: How can I check if I am about to run out of items?**
The `analyze_stockout_risk` tool evaluates your current stock against demand and lead time to tell you if you are at risk and how many days of sales remain.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/inventory-reorder-point-calculator](https://vinkius.com/en/ai-agent-connect/inventory-reorder-point-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Inventory Reorder Point Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `inventory-reorder-point-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Inventory Reorder Point Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "inventory-reorder-point-calculator": {
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
