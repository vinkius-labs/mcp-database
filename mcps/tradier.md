# Tradier MCP Server

Trade equities and options, fetch real-time market data, and manage your brokerage accounts directly through any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tradier)

## Overview
**Category:** data-analytics
**Tools Count:** 13

## Description
Connect your **Tradier** brokerage account to any AI agent to streamline your trading workflow and market analysis through natural conversation.

### What you can do

- **Market Data** — Get real-time quotes via `get_quotes`, detailed option chains with `get_option_chains`, and historical price bars using `get_historical_data`.
- **Account Management** — Check balances with `get_account_balances`, view current holdings via `get_account_positions`, and review transaction history with `get_account_history`.
- **Order Execution** — Place, monitor, and cancel equity or option orders using `place_order`, `get_order_status`, and `cancel_order` directly through natural language.
- **Market Insights** — Search for symbols using `search_symbols` and check the market calendar for trading hours and holidays with `get_market_calendar`.

### How it works

1. Subscribe to this server
2. Enter your Tradier Access Token
3. Start trading and analyzing markets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Active Traders** — Execute trades and monitor positions without switching between multiple platforms or browser tabs.
- **Financial Analysts** — Pull historical data and option chains directly into your analysis workflow for instant processing.
- **Developers** — Integrate brokerage capabilities into your AI-driven financial tools and custom trading assistants.


## Available Tools
- **get_account_balances**: Get balances and buying power for a specific account
- **get_account_history**: Review trading history and account activity
- **get_account_positions**: View current holdings in an account
- **cancel_order**: Cancel a pending order
- **create_streaming_session**: Create a session to receive a streaming session ID
- **get_historical_data**: Get historical price bars (daily, weekly, monthly)
- **get_market_calendar**: Get market hours and holidays
- **get_option_chains**: Retrieve option chains for a specific underlying symbol
- **get_order_status**: Check the status of a specific order
- **place_order**: Execute equity or option trades
- **get_quotes**: Fetch real-time or delayed quotes for one or more symbols
- **search_symbols**: Search for symbols by keyword or description
- **get_user_profile**: Retrieve the user profile and linked accounts


## Installation & Usage

To install and use the **Tradier** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tradier](https://vinkius.com/mcp/tradier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
