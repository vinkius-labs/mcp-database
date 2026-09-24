# Repeat Order Rate Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repeat-order-rate-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Calculate customer loyalty and repeat purchase rates.

## Description
This MCP server provides tools to analyze customer retention and loyalty. Use `get_repeat_order_rate` to find the percentage of returning customers within a timeframe, `get_customer_loyalty_tiers` to group users by order volume, `get_customer_order_history` to inspect individual customer activity, and `get_period_over_period_growth` to compare retention trends across different time periods.


## Available Tools (4)
- **get_customer_loyalty_tiers**: Categorizes customers into loyalty groups based on their total number of lifetime orders
- **get_customer_order_history**: Retrieves the specific order count and frequency for a single identified customer
- **get_period_over_period_growth**: Compares the repeat order rate of the current period against a previous period
- **get_repeat_order_rate**: Calculates the percentage of customers who have ordered more than once


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repeat Order Rate Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was our repeat order rate between 2024-01-01 and 2024-03-31?"

**🤖 AI Agent:**
> The repeat order rate for the period from January 1st to March 31st, 2024, was 15.5%, with 155 repeat customers out of 1,000 total customers.

---

**👤 You:**
> "How many customers have at least 5 orders?"

**🤖 AI Agent:**
> There are 42 customers who fall into the loyalty tier requiring a minimum of 5 orders.

---

**👤 You:**
> "Check the status of customer ID 'cust_98765'."

**🤖 AI Agent:**
> Customer cust_98765 has placed 3 total orders and is classified as a repeat customer.


## ❓ FAQ

**Q: How is the repeat order rate calculated?**
The rate is calculated by dividing the number of customers with two or more orders by the total number of unique customers in the specified timeframe.

**Q: Can I compare retention between two different months?**
Yes, you can use `get_period_over_period_growth` to compare the repeat order rate of a current period against a previous one.

**Q: What information is available for a specific customer?**
By using `get_customer_order_history`, you can retrieve the total order count and whether they are classified as a repeat customer.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repeat-order-rate-analytics](https://vinkius.com/en/ai-agent-connect/repeat-order-rate-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repeat Order Rate Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repeat-order-rate-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repeat Order Rate Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repeat-order-rate-analytics": {
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
