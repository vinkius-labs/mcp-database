# Pet Product Budgeting MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-product-budgeting)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate total pet ownership costs including food, supplies, and subscriptions.

## Description
This MCP server provides a comprehensive financial overview of pet ownership expenses. It allows AI agents to calculate detailed budgets by aggregating feeding costs, consumable supplies, periodic replacement items, and recurring subscriptions. Use `get_budget_summary` for a complete breakdown of all costs and discounts, or specific tools like `get_feeding_costs` and `get_supply_costs` for granular analysis of individual expense categories.


## Available Tools (4)
- **get_budget_summary**: Provides a complete financial overview of pet expenses including all categories and discounts
- **get_feeding_costs**: Calculates the total cost of food for a specific duration
- **get_subscription_costs**: Calculates the total cost of all active pet subscriptions over a period
- **get_supply_costs**: Calculates the cost of consumable supplies and periodic replacement items


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Product Budgeting** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total budget for my pet (ID: pet_123) for the next 30 days?"

**🤖 AI Agent:**
> The total budget for pet_123 for the next 30 days is $145.50, which includes $80.00 for food, $40.00 for supplies, and $25.50 for subscriptions.

---

**👤 You:**
> "How much will I spend on food for my pet (ID: pet_456) over 90 days?"

**🤖 AI Agent:**
> The total food cost for pet_456 over 90 days is $120.00.

---

**👤 You:**
> "Calculate the supply costs for pet_789 for a 180-day period."

**🤖 AI Agent:**
> The total supply cost for pet_789 over 180 days is $65.00, consisting of $45.00 in consumables and $20.00 for replacement items.


## ❓ FAQ

**Q: How are replacement item costs calculated?**
Replacement costs are calculated by taking the cost of the item and dividing it by its expected lifespan in days, then multiplying by your requested timeframe.

**Q: Can I see a full breakdown of all my pet's expenses?**
Yes, you can use the `get_budget_summary` tool to receive a complete financial overview including feeding, supplies, subscriptions, and applicable discounts.

**Q: Does this include subscription costs?**
Yes, the system accounts for recurring fixed costs like monthly treat boxes or flea prevention shipments through the subscription calculation logic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-product-budgeting](https://vinkius.com/en/ai-agent-connect/pet-product-budgeting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Product Budgeting** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-product-budgeting` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Product Budgeting** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-product-budgeting": {
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
