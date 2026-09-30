# Grocery Store Basket Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/grocery-store-basket-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Find the cheapest way to complete your grocery shopping list.

## Description
This MCP server acts as a decision-support engine for grocery shopping. It evaluates the total cost of completing a shopping list across different stores by calculating unit prices, travel expenses, and available discounts. Use `compare_baskets` to find the most economical store, `calculate_store_subtotal` for specific store costs, `evaluate_substitution` to check item replacements, or `get_store_inventory_summary` to see how well a store matches your needs.


## Available Tools (4)
- **compare_baskets**: 
- **calculate_store_subtotal**: 
- **evaluate_substitution**: 
- **get_store_inventory_summary**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grocery Store Basket Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which store is cheapest for my list: 2kg Flour, 1L Milk, and 12 Eggs?"

**🤖 AI Agent:**
> The cheapest store is SuperMart with a total cost of $12.50, saving you $2.10 compared to the most expensive option.

---

**👤 You:**
> "Can I use a substitute for the milk if the brand I want is missing?"

**🤖 AI Agent:**
> Yes, the substitution is valid as the available 1L brand meets your minimum quantity requirement.

---

**👤 You:**
> "How much will I spend at the local Express store?"

**🤖 AI Agent:**
> The subtotal for the Express store is $15.00 before travel fees.


## ❓ FAQ

**Q: How does the tool calculate the cheapest store?**
The `compare_baskets` tool calculates the total cost for each store by summing item prices (adjusted for package size) and adding the specific travel cost for that location.

**Q: What happens if an item is out of stock?**
The engine uses `evaluate_substitution` to check if a valid replacement is available. A store is only considered a valid option if it can fulfill 100% of your list through direct matches or valid substitutions.

**Q: Does it account for travel costs?**
Yes, travel costs are a fixed overhead included in the total cost calculation for every store to ensure you find the true cheapest option.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/grocery-store-basket-comparator](https://vinkius.com/en/ai-agent-connect/grocery-store-basket-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grocery Store Basket Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `grocery-store-basket-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grocery Store Basket Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grocery-store-basket-comparator": {
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
