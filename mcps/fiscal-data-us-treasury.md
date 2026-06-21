# Fiscal Data (U.S. Treasury) MCP Server

Access real-time U.S. Treasury financial data, including exchange rates, monthly statements, and over 170 fiscal datasets.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fiscal-data-us-treasury)

## Overview
**Category:** data-analytics
**Tools Count:** 4

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


## Installation & Usage

To install and use the **Fiscal Data (U.S. Treasury)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fiscal-data-us-treasury](https://vinkius.com/mcp/fiscal-data-us-treasury)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
