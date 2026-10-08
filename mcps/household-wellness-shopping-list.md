# Household Wellness & Shopping List MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-wellness-shopping-list)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage household inventory and automate shopping lists based on routine usage.

## Description
This MCP server connects your AI agent to your household inventory management system. It tracks how supplies are consumed during recurring routines like wellness or cleaning, predicts when items will run out using `calculate_depletion_forecast`, and generates optimized shopping lists via `generate_shopping_list`. You can monitor specific item levels with `get_supply_status` or view all your active activities using `list_routines` to ensure your home stays fully stocked.


## Available Tools (4)
- **generate_shopping_list**: Aggregates all supplies that need replenishment
- **get_supply_status**: Provides a detailed snapshot of a specific supply
- **list_routines**: Retrieves all defined household routines
- **calculate_depletion_forecast**: Predicts when a specific supply will run out


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Wellness & Shopping List** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What do I need to buy for my household right now?"

**🤖 AI Agent:**
> You need to purchase: 2 units of Liquid Soap (Critical) and 1 pack of Vitamin Pills (Standard). Total estimated cost is $15.50.

---

**👤 You:**
> "How much laundry detergent do I have left?"

**🤖 AI Agent:**
> You currently have 500ml of laundry detergent in stock. This is enough for your next 2 cleaning routines.

---

**👤 You:**
> "When will I run out of my skincare products?"

**🤖 AI Agent:**
> Based on your current usage, your facial cleanser is estimated to run out in 5 days.


## ❓ FAQ

**Q: How does the shopping list get updated?**
The list is updated by analyzing the current stock against the usage rates defined in your routines. When stock falls below the threshold needed for the next routine, it is added to the list.

**Q: Can I see when my soap will run out?**
Yes, you can use `calculate_depletion_forecast` to predict exactly how many days of stock remain for any specific supply.

**Q: What routines are tracked?**
The system tracks all routines defined in your catalog, such as wellness activities or maintenance tasks, which drive the consumption of your supplies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-wellness-shopping-list](https://vinkius.com/en/ai-agent-connect/household-wellness-shopping-list)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Wellness & Shopping List** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-wellness-shopping-list` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Wellness & Shopping List** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-wellness-shopping-list": {
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
