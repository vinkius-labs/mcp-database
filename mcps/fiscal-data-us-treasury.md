# Fiscal Data (U.S. Treasury) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fiscal-data-us-treasury)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time U.S. Treasury financial data, including exchange rates, monthly statements, and over 170 fiscal datasets.

## Description
Connect directly to the **U.S. Department of the Treasury's Fiscal Data API** to retrieve authoritative financial information. This server enables AI agents to query a vast library of federal financial data for analysis, reporting, and economic research.

### What you can do

- **Comprehensive Data Access** — Query any of the 170+ available endpoints including debt, interest rates, and federal spending via the `query_dataset` tool.
- **Exchange Rates** — Fetch official Treasury Reporting Rates of Exchange for international currencies using `get_rates_of_exchange`.
- **Monthly Treasury Statements** — Access detailed summaries of federal receipts and outlays through `get_mts_table_1` and `get_mts_table_9`.
- **Advanced Filtering** — Apply precise filters, sorting, and pagination to handle large datasets efficiently directly within your conversation.

### How it works

1. Subscribe to this server
2. (Optional) Enter your Fiscal Data API Key for higher rate limits
3. Start querying federal financial data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Financial Analysts** — instantly retrieve historical exchange rates and federal budget summaries without manual CSV downloads.
- **Data Scientists** — pull clean, structured fiscal data directly into your analysis environment.
- **Policy Researchers** — track government spending and debt metrics through natural language queries.


## Available Tools
- **get_mts_table_1**: Get Monthly Treasury Statement (MTS) Table 1
- **get_mts_table_9**: Get Monthly Treasury Statement (MTS) Table 9
- **get_rates_of_exchange**: Get Treasury Reporting Rates of Exchange
- **query_dataset**: Provide the endpoint path (e.g., v1/accounting/od/rates_of_exchange) and optional filters.

Query any Fiscal Data dataset endpoint


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fiscal Data (U.S. Treasury)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the Treasury exchange rates for the Euro for the last recorded date."

**🤖 AI Agent:**
> I'll fetch the latest exchange rates using `get_rates_of_exchange`. For the Eurozone-Euro, the rate was 0.921 per USD as of the most recent record date.

---

**👤 You:**
> "Show me the summary of federal receipts and outlays from MTS Table 1 for 2023."

**🤖 AI Agent:**
> I'm querying `get_mts_table_1` with a filter for the year 2023. I've found the summary data showing total receipts and outlays for each month of the fiscal year.

---

**👤 You:**
> "Use query_dataset to find data on the 'daily_treasury_statement' for the past week."

**🤖 AI Agent:**
> Accessing the `query_dataset` tool for the endpoint 'v1/accounting/od/daily_treasury_statement'. I've retrieved the daily cash balances and operating totals for the requested period.


## ❓ FAQ

**Q: How can I access specific datasets like the national debt or federal spending?**
You can use the `query_dataset` tool. Simply provide the endpoint path (e.g., 'v1/debt/mspd/mspd_table_1' for the Monthly Statement of the Public Debt) and any optional filters to get the exact data you need.

**Q: Can I filter the financial data by a specific date or currency?**
Yes! All tools like `get_rates_of_exchange` and `get_mts_table_1` support a `filter` parameter. For example, use `record_date:eq:2023-12-31` to get data for a specific day or `country_currency_desc:eq:CANADA-DOLLAR` for specific currency rates.

**Q: What is the difference between Table 1 and Table 9 in the Monthly Treasury Statement?**
The `get_mts_table_1` tool provides a high-level summary of receipts, outlays, and the surplus or deficit. The `get_mts_table_9` tool provides a more granular breakdown of Budgetary Receipts by reporting entity and major source.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fiscal-data-us-treasury](https://vinkius.com/mcp/fiscal-data-us-treasury)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fiscal Data (U.S. Treasury)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fiscal-data-us-treasury` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fiscal Data (U.S. Treasury)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fiscal-data-us-treasury": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
