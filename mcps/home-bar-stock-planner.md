# Home Bar Stock Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/home-bar-stock-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Plan cocktail events by calculating exact ingredient, ice, and glassware needs.

## Description
The Home Bar Stock Planner is a precision engine for hosting perfect cocktail events. It analyzes cocktail recipes to determine the exact volumes of spirits, mixers, and garnishes required for your guest count. By using `calculate_total_requirements`, you can determine the bulk needs for any event, and `compare_requirements_to_stock` helps you generate a precise shopping list by checking your current inventory. Whether you need to check your current supplies with `get_stock_status` or find a specific recipe with `get_cocktail_recipe`, this tool ensures you never run out of ingredients mid-party.


## Available Tools (4)
- **get_cocktail_recipe**: Retrieves the detailed ingredient list and glassware requirements for a specific cocktail
- **get_stock_status**: Provides a summary of the current inventory levels to help the user understand their starting point
- **calculate_total_requirements**: Calculates the absolute volume and quantity of every item needed for a planned event
- **compare_requirements_to_stock**: Identifies exactly what needs to be purchased by comparing the event requirements against what is currently in the bar


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Home Bar Stock Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm hosting 10 people and want to serve Margaritas. How much tequila and lime juice do I need?"

**🤖 AI Agent:**
> For 10 guests, you will need 500ml of Tequila and 250ml of Lime Juice.

---

**👤 You:**
> "What is my current stock of spirits?"

**🤖 AI Agent:**
> You currently have 750ml of Vodka, 500ml of Gin, and 350ml of Tequila in stock.

---

**👤 You:**
> "I want to make Old Fashioneds for 5 people. What do I need to buy?"

**🤖 AI Agent:**
> You need to purchase 150ml of Bourbon and 50ml of Angostura Bitters.


## ❓ FAQ

**Q: How do I know what I need to buy for a party?**
Use `calculate_total_requirements` to find the total needs for your guest count, then use `compare_requirements_to_stock` to see what is missing from your current bar inventory.

**Q: Can I check my current bar inventory?**
Yes, you can use `get_stock_status` to view your current levels of spirits, mixers, garnishes, or glassware.

**Q: Does this tool account for ice and glassware?**
Yes, the planning engine calculates the necessary volume of ice and the specific count of glassware required for the selected cocktails.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/home-bar-stock-planner](https://vinkius.com/en/ai-agent-connect/home-bar-stock-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Home Bar Stock Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `home-bar-stock-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Home Bar Stock Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "home-bar-stock-planner": {
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
