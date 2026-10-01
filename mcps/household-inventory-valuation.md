# Household Inventory Valuation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-inventory-valuation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate insurance-ready totals for household belongings by room, category, and value.

## Description
This MCP server provides tools to manage and analyze household asset values for insurance purposes. Use `get_room_summary` to see financial totals for a specific room, `get_category_totals` to aggregate values for item types like Furniture or Electronics, and `get_high_value_items` to identify expensive assets. You can also use `identify_valuation_gaps` to find items missing critical purchase or replacement cost data.


## Available Tools (4)
- **get_category_totals**: Aggregates values across the entire household for specific item types
- **get_room_summary**: Provides a high-level financial overview of all items located within a specific room
- **get_high_value_items**: Identifies the most expensive assets in the household for insurance prioritization
- **identify_valuation_gaps**: Locates items that are missing critical financial data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Inventory Valuation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total replacement value of all items in the Living Room?"

**🤖 AI Agent:**
> The total replacement value for the Living Room is $4,250.00.

---

**👤 You:**
> "Show me all items worth more than $500."

**🤖 AI Agent:**
> The high-value items are: Sony Bravia TV ($1,200), Leather Sofa ($850), and MacBook Pro ($1,500).

---

**👤 You:**
> "Are there any items missing their purchase value?"

**🤖 AI Agent:**
> Yes, there are 3 items missing purchase value: Dining Table, Microwave, and Coffee Maker.


## ❓ FAQ

**Q: How can I see the total value of items in my Kitchen?**
You can use the `get_room_summary` tool and provide 'Kitchen' as the room name to get a full breakdown of purchase and replacement values.

**Q: How do I find items that are missing price information?**
Use the `identify_valuation_gaps` tool and specify whether you are looking for missing 'purchaseValue' or 'replacementValue'.

**Q: Can I list only my most expensive items?**
Yes, use `get_high_value_items` and set a threshold for the minimum replacement value you want to see.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-inventory-valuation](https://vinkius.com/en/ai-agent-connect/household-inventory-valuation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Inventory Valuation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-inventory-valuation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Inventory Valuation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-inventory-valuation": {
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
