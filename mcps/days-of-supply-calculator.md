# Days of Supply Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/days-of-supply-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Monitor inventory health by calculating stock coverage and identifying supply risks.

## Description
This MCP server provides specialized tools for inventory management. Use `get_sku_supply_metrics` to analyze individual items, `get_category_health_summary` to assess group performance, and `calculate_financial_exposure_by_tier` to identify capital tied up in overstock or at risk of stockout.


## Available Tools (3)
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


## ❓ FAQ

**Q: What is the purpose of this MCP?**
It calculates how many days your current stock will last based on daily demand, helping you prevent stockouts and reduce overstock.

**Q: How does it identify stockout risks?**
The tool flags any item where the calculated supply duration is less than 7 days as a critical risk.

**Q: Can I analyze financial impact?**
Yes, using `calculate_financial_exposure_by_tier`, you can see the monetary value of inventory held in different coverage tiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/days-of-supply-calculator](https://vinkius.com/mcp/days-of-supply-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Days of Supply Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `days-of-supply-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Days of Supply Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "days-of-supply-calculator": {
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
