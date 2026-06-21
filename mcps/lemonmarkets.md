# lemon.markets MCP Server

Trade European stocks and ETFs and access real-time market data via lemon.markets.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/lemonmarkets)

## Overview
**Category:** data-analytics
**Tools Count:** 8

## Description
Connect your **lemon.markets** account to any AI agent to automate your stock trading and market analysis. This MCP server enables your agent to search for instruments, retrieve real-time quotes, and manage your brokerage orders directly.

### What you can do

- **Market Discovery** — Search for European stocks and ETFs by name or ISIN across major exchanges
- **Real-time Pricing** — Get the latest bid/ask quotes and price data for any tradable instrument
- **Portfolio Oversight** — List your active positions and retrieve detailed account balance information
- **Order Execution** — Place, activate, and cancel buy or sell orders directly from natural language
- **Trading History** — Monitor your order status and transaction history to track your investment performance

### How it works

1. Subscribe to this server
2. Enter your lemon.markets API Key
3. Start trading and analyzing the market from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Individual Investors** — Quickly check quotes and manage your portfolio via natural language commands
- **Financial Analysts** — Automate the retrieval of real-time market data for research and reporting
- **Developers** — Integrate stock trading and market data retrieval into custom trading bots or applications


## Available Tools
- **get_brokerage_account**: markets trading account.

Get trading account information
- **activate_pending_order**: Activate a placed order to execute it
- **cancel_open_order**: Cancel an open order
- **get_latest_quote**: Get the latest bid/ask prices for an instrument
- **list_brokerage_orders**: List recent trading orders
- **place_new_order**: Note: Orders must usually be activated after creation.

Place a new buy or sell order
- **list_active_positions**: List all currently held portfolio positions
- **search_market_instruments**: g., "Apple", "Tesla", or a specific ISIN).

Search for stocks or ETFs on lemon.markets


## Installation & Usage

To install and use the **lemon.markets** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lemonmarkets](https://vinkius.com/mcp/lemonmarkets)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
