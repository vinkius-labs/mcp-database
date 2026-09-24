# Order Analytics Connector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/order-analytics-connector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Retrieve total order counts, customer frequency, and status distributions.

## Description
This MCP server provides tools to analyze customer transaction history. You can use `get_total_order_count` to find total orders in a timeframe, `get_customer_order_frequency` to check a specific customer's activity, `get_orders_by_status_distribution` for status breakdowns, and `get_order_volume_by_period` to track volume trends.


## Available Tools (4)
- **get_customer_order_frequency**: Answers how many orders a specific customer has placed
- **get_order_volume_by_period**: Answers the trend of order counts over a specific interval
- **get_orders_by_status_distribution**: g., Completed, Cancelled, Pending) within a timeframe.

Answers the breakdown of orders by their current status
- **get_total_order_count**: Answers how many total orders have been placed in a specific timeframe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Order Analytics Connector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many total orders were placed between 2023-01-01 and 2023-12-31?"

**🤖 AI Agent:**
> There were 1,250 total orders placed between January 1, 2023, and December 31, 2023.

---

**👤 You:**
> "What is the order frequency for customer ID CUST-9982?"

**🤖 AI Agent:**
> Customer CUST-9982 has placed 14 orders.

---

**👤 You:**
> "Show me the breakdown of order statuses for the last month."

**🤖 AI Agent:**
> For the last month, there were 450 Completed orders, 30 Pending orders, and 15 Cancelled orders.


## ❓ FAQ

**Q: How can I see how many orders a specific customer has made?**
Use the `get_customer_order_frequency` tool with the specific customer ID.

**Q: Can I include cancelled orders in my total count?**
Yes, when using `get_total_order_count`, you can set the `includeCancelled` parameter to true.

**Q: How do I view order trends over time?**
You can use `get_order_volume_by_period` to get a time series of order counts by day or month.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/order-analytics-connector](https://vinkius.com/en/ai-agent-connect/order-analytics-connector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Order Analytics Connector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `order-analytics-connector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Order Analytics Connector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "order-analytics-connector": {
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
