# Photo Print Order Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/photo-print-order-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate costs, shipping, and recipient distribution for photo print orders.

## Description
This MCP server provides a complete planning engine for personalized photo print orders. It handles complex calculations including product costs for prints, albums, and frames, shipping fees based on weight, and distribution logic to split orders among multiple recipients. Use `calculate_print_costs` to find base totals, `distribute_to_recipients` to plan gift distribution, `calculate_shipping_fee` for logistics, and `estimate_final_total` to determine the final customer price after discounts.


## Available Tools (4)
- **calculate_shipping_fee**: Determines the shipping cost based on the physical characteristics of the order
- **distribute_to_recipients**: Calculates the required quantity of products per recipient to satisfy a total order requirement
- **estimate_final_total**: Provides the final amount the customer must pay, including products, shipping, and discounts
- **calculate_print_costs**: Determines the total cost for specific print items based on their quantities and types


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Photo Print Order Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for 5 premium albums at $20 each?"

**🤖 AI Agent:**
> The total base cost for 5 premium albums is $100.

---

**👤 You:**
> "If I have 10 prints and 2 recipients, how many does each person get?"

**🤖 AI Agent:**
> Each recipient will receive 5 prints.

---

**👤 You:**
> "Calculate the final total for a $50 order with $5 shipping and a $10 discount."

**🤖 AI Agent:**
> The grand total is $45.


## ❓ FAQ

**Q: How do I calculate the total cost of my prints?**
You can use the `calculate_print_costs` tool by providing a JSON array of your items, including their product IDs, quantities, and unit prices.

**Q: Can I split an order between multiple people?**
Yes, the `distribute_to_recipients` tool calculates how many items each person should receive to ensure an equal distribution.

**Q: How is shipping calculated?**
Shipping is determined using `calculate_shipping_fee`, which combines a base rate with the total weight of all products in the order.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/photo-print-order-planner](https://vinkius.com/en/ai-agent-connect/photo-print-order-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Photo Print Order Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `photo-print-order-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Photo Print Order Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "photo-print-order-planner": {
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
