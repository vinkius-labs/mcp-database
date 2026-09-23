# Food Order Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/food-order-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Splits shared food orders equally among diners.

## Description
This MCP server provides tools to manage group dining expenses. It allows you to calculate individual totals, identify shared items, get a group summary, and validate order integrity. Use `calculate_individual_totals` to find out exactly what each person owes, or `get_group_summary` to see the total cost and number of participants.


## Available Tools (4)
- **calculate_individual_totals**: Determines exactly how much each person owes based on their specific items and their share of shared items
- **get_group_summary**: Provides a high-level overview of the entire order, including total cost and participation counts
- **identify_shared_items**: Isolates and lists only the items that are meant to be shared by the whole group
- **validate_order_integrity**: Checks if the provided order data is logically sound before processing splits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Food Order Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the split for this order: items are [{"name": "Pizza", "price": 20, "owner": null, "quantity": 1}, {"name": "Soda", "price": 5, "owner": "Alice", "quantity": 1}] and diners are ["Alice", "Bob"]."

**🤖 AI Agent:**
> Alice owes $12.50 and Bob owes $12.50.

---

**👤 You:**
> "What are the shared items in this order: [{"name": "Fries", "price": 4, "owner": null, "quantity": 1}, {"name": "Burger", "price": 12, "owner": "Charlie", "quantity": 1}]?"

**🤖 AI Agent:**
> The shared item is Fries.

---

**👤 You:**
> "Give me a summary of this order: items are [{"name": "Tacos", "price": 15, "owner": null, "quantity": 3}] and diners are ["Dave", "Eve"]."

**🤖 AI Agent:**
> The total order cost is $45, there are 2 diners, and 1 shared item.


## ❓ FAQ

**Q: How does the splitting logic work?**
Individual items are assigned to specific diners, while shared items are divided equally among all participants in the group.

**Q: Can I validate my order before splitting?**
Yes, you can use the `validate_order_integrity` tool to ensure all prices, quantities, and owners are correctly recorded.

**Q: What happens if a diner is not in the list?**
The `calculate_individual_totals` tool will return an error if an item owner is not included in the provided list of diners.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/food-order-splitter](https://vinkius.com/en/ai-agent-connect/food-order-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Food Order Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `food-order-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Food Order Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "food-order-splitter": {
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
