# Grocery Price Book Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/grocery-price-book-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze unit prices, historical trends, and store comparisons for grocery items.

## Description
The Grocery Price Book Builder transforms raw purchase data into actionable intelligence. It allows AI agents to normalize costs into standard unit prices, track price volatility over time, and compare costs across different retailers. Use `get_best_known_price` to find the lowest historical cost for an item, `analyze_item_unit_prices` to view full price history, `get_price_trend_analysis` to monitor price changes over a specific date range, or `get_store_price_comparison` to identify the cheapest store for a specific product.


## Available Tools (4)
- **get_best_known_price**: Identifies the lowest historical unit price recorded for a specific product
- **get_price_trend_analysis**: Summarizes how the unit price of an item has changed over a specified period
- **analyze_item_unit_prices**: Calculates the normalized unit price for all recorded purchases of a specific item
- **get_store_price_comparison**: Compares the unit prices of a specific product across different stores


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grocery Price Book Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the best price ever recorded for product ID 'milk-123'?"

**🤖 AI Agent:**
> The best price recorded for milk-123 was $2.50 per liter at Store A on 2023-10-12.

---

**👤 You:**
> "Show me the price trend for 'bread-456' between 2024-01-01 and 2024-03-01."

**🤖 AI Agent:**
> Between January and March 2024, the average unit price for bread-456 was $3.00, with a price increase of 5%.

---

**👤 You:**
> "Which store has the cheapest price for 'eggs-789'?"

**🤖 AI Agent:**
> The cheapest average price for eggs-789 is at SuperMart, with a unit price of $0.25 per egg.


## ❓ FAQ

**Q: How are unit prices calculated?**
Unit prices are calculated by dividing the total cost of a purchase by the quantity provided in the record, normalized to the product's standard unit of measure.

**Q: Can I compare prices between different stores?**
Yes, you can use the `get_store_price_comparison` tool to see the average unit prices for a product across all stores in your ledger.

**Q: How do I find the cheapest price ever recorded for an item?**
You can use the `get_best_known_price` tool to identify the lowest historical unit price recorded for a specific product ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/grocery-price-book-builder](https://vinkius.com/en/ai-agent-connect/grocery-price-book-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grocery Price Book Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `grocery-price-book-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grocery Price Book Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grocery-price-book-builder": {
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
