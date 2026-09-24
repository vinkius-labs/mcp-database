# Sales Total Aggregator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sales-total-aggregator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Aggregates and analyzes sales transaction amounts.

## Description
This MCP server provides tools to process and analyze collections of sales transactions. It allows AI agents to calculate total revenue using `calculate_total_sales`, determine mean transaction values with `calculate_average_sale`, extract descriptive statistics via `get_sales_statistics`, and filter significant entries using `identify_large_transactions`.


## Available Tools (4)
- **calculate_average_sale**: Calculates the average value of a sale in a set
- **calculate_total_sales**: Calculates the sum of all provided sales amounts
- **get_sales_statistics**: Provides high-level descriptive statistics for a set of sales
- **identify_large_transactions**: Identifies specific sales that exceed a certain threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sales Total Aggregator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total sum of these sales: 100, 250, 50, 400?"

**🤖 AI Agent:**
> The total sum of the provided sales is 800.

---

**👤 You:**
> "What was the average sale for 10, 20, and 30?"

**🤖 AI Agent:**
> The average sale value is 20.

---

**👤 You:**
> "Which sales are greater than 150 in this list: 50, 200, 300, 10?"

**🤖 AI Agent:**
> The sales exceeding 150 are 200 and 300.


## ❓ FAQ

**Q: How do I calculate the total revenue?**
You can use the `calculate_total_sales` tool by providing a list of transaction amounts.

**Q: Can I find transactions above a specific amount?**
Yes, the `identify_large_transactions` tool allows you to specify a threshold to filter for high-value sales.

**Q: What statistics can be retrieved?**
The `get_sales_statistics` tool provides the total sum, highest sale, lowest sale, and the total count of transactions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sales-total-aggregator](https://vinkius.com/en/ai-agent-connect/sales-total-aggregator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sales Total Aggregator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sales-total-aggregator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sales Total Aggregator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sales-total-aggregator": {
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
