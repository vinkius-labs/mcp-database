# Revenue Per Customer Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/revenue-per-customer-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze average revenue per customer across timeframes and segments.

## Description
This MCP server provides business intelligence tools to calculate and analyze Revenue Per Customer (RPC). It allows you to monitor overall average revenue using `get_total_rpc`, break down performance by customer segments with `get_segmented_rpc`, track historical trends via `get_rpc_trend`, and identify high-value individuals using `get_top_contributing_customers`.


## Available Tools (4)
- **get_rpc_trend**: Get the trend of revenue per customer over time
- **get_segmented_rpc**: An optional segment name can be provided to filter.

Get the revenue per customer broken down by segments
- **get_top_contributing_customers**: An optional limit can be provided.

Get the customers contributing the highest revenue
- **get_total_rpc**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Revenue Per Customer Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the overall average revenue per customer between 2023-01-01 and 2023-12-31?"

**🤖 AI Agent:**
> The average revenue per customer for the period was $150.00, with a total revenue of $15,000.00 from 100 unique customers.

---

**👤 You:**
> "Show me the revenue per customer trend for the last month, broken down daily."

**🤖 AI Agent:**
> The daily RPC trend for the last month shows a steady increase from $120.00 on the 1st to $145.00 on the 30th.

---

**👤 You:**
> "Who are the top 3 customers by revenue contribution in 2023?"

**🤖 AI Agent:**
> The top 3 customers are: Customer_ID_99 ($5,000), Customer_ID_42 ($3,500), and Customer_ID_12 ($2,100).


## ❓ FAQ

**Q: How is the revenue per customer calculated?**
It is calculated by dividing the total revenue within a specific period by the number of unique customers who contributed to that revenue in the same period.

**Q: Can I filter the analysis by specific customer segments?**
Yes, you can use `get_segmented_rpc` to view revenue per customer for specific segments like Platinum or North America.

**Q: How do I see if my RPC is improving over time?**
You can use the `get_rpc_trend` tool to view the revenue per customer trend at daily or monthly intervals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/revenue-per-customer-analytics](https://vinkius.com/en/ai-agent-connect/revenue-per-customer-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Revenue Per Customer Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `revenue-per-customer-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Revenue Per Customer Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "revenue-per-customer-analytics": {
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
