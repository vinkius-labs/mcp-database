# Online Order Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/online-order-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Distribute shared order costs, taxes, and discounts proportionally among buyers.

## Description
This MCP server provides precise tools for decomposing shared online purchases into fair, individual obligations. It uses proportional logic to distribute discounts, taxes, and shipping fees based on the value of each item. Use `calculate_splits` to determine what each person owes, `calculate_refund` to handle returns, `validate_order_consistency` to verify payments, and `get_buyer_summary` for individual financial overviews.


## Available Tools (4)
- **validate_order_consistency**: Checks if individual payments match the total amount charged
- **calculate_refund**: Determines how much a specific buyer should receive back when items are returned
- **calculate_splits**: Calculates the final amount each buyer owes for a single order
- **get_buyer_summary**: Provides a high-level overview of a specific buyer's financial responsibility


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Online Order Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Split this order: items are [{itemId: '1', price: 100, buyerId: 'A'}, {itemId: '2', price: 50, buyerId: 'B'}], discount is 15, tax is 10, and shipping is 5."

**🤖 AI Agent:**
> Buyer A owes 63.33 and Buyer B owes 31.67.

---

**👤 You:**
> "How much should Buyer A get back if they return item '1' from the previous split?"

**🤖 AI Agent:**
> Buyer A should receive a refund of 85.00.

---

**👤 You:**
> "Give me a summary for Buyer B for the order with items [{itemId: '1', price: 100, buyerId: 'A'}, {itemId: '2', price: 50, buyerId: 'B'}], discount 15, tax 10, shipping 5."

**🤖 AI Agent:**
> Buyer B contributed 31.67 for 1 item, with an average item cost of 31.67.


## ❓ FAQ

**Q: How are discounts and taxes distributed?**
Costs are distributed proportionally. Every discount, tax, and shipping fee is assigned to an individual based on the ratio of their item's cost to the total order cost.

**Q: Does this tool handle returns?**
Yes, you can use `calculate_refund` to determine the exact amount a buyer should receive back, including their share of the original discount and tax.

**Q: How can I verify if everyone paid the correct amount?**
You can use `validate_order_consistency` to check if the sum of individual payments matches the total amount charged by the merchant.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/online-order-splitter](https://vinkius.com/en/ai-agent-connect/online-order-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Online Order Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `online-order-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Online Order Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "online-order-splitter": {
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
