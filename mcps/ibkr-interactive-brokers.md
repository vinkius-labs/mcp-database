# IBKR (Interactive Brokers) MCP Server

Manage your Interactive Brokers account — execute trades, monitor portfolio ledgers, and fetch real-time market data via the Client Portal API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ibkr-interactive-brokers)

## Overview
**Category:** money-moves
**Tools Count:** 9

## Description
Connect your **Interactive Brokers** account to any AI agent to automate your trading workflows and portfolio monitoring through the Client Portal API.

### What you can do

- **Order Management** — Place, modify, and cancel orders for specific accounts using natural language commands.
- **Market Data** — Fetch real-time snapshots for specific contracts (ConIds) to inform your trading decisions.
- **Portfolio Tracking** — Monitor cash balances by currency and view comprehensive account summaries including equity and margin metrics.
- **Advanced Reporting** — Programmatically request and retrieve pre-configured Flex Query reports for deep financial analysis and auditing.
- **Session Maintenance** — Keep your API session active with built-in session management tools.

### How it works

1. Subscribe to this server
2. Enter your IBKR Client Portal API URL and your optional Flex Web Service Token
3. Start managing your brokerage account from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Active Traders** — execute and modify orders quickly without switching between complex trading interfaces
- **Financial Analysts** — automate the retrieval of portfolio ledgers and Flex statements for reporting
- **Developers** — integrate real-time market data and account management directly into your coding environment


## Available Tools
- **get_account_summary**: Get account summary
- **cancel_order**: Cancel an existing order
- **get_flex_statement**: Retrieve a generated Flex Query report
- **get_market_data_snapshot**: Get market data snapshot for contracts
- **modify_order**: Modify an existing order
- **place_order**: Requires a JSON array of order objects.

Place a new order
- **get_portfolio_ledger**: Get portfolio ledger
- **send_flex_request**: Returns a ReferenceCode to be used with get_flex_statement.

Generate a Flex Query report
- **tickle_session**: Maintain Client Portal API session


## Installation & Usage

To install and use the **IBKR (Interactive Brokers)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibkr-interactive-brokers](https://vinkius.com/mcp/ibkr-interactive-brokers)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
