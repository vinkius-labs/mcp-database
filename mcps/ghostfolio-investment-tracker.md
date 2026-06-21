# Ghostfolio (Investment Tracker) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ghostfolio-investment-tracker)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ghostfolio-investment-tracker-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ghostfolio-investment-tracker-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track your wealth and manage investment portfolios via Ghostfolio — monitor holdings, record activities, and analyze performance through AI.

## Description
Connect your **Ghostfolio** instance to any AI agent to monitor your net worth and manage your investment portfolio through natural conversation.

### What you can do

- **Portfolio Performance** — Get high-level summaries of your portfolio's performance and statistics.
- **Holdings & Valuations** — Retrieve detailed lists of current holdings with real-time market valuations.
- **Activity Tracking** — Record new transactions (BUY, SELL, DIVIDEND, INTEREST, FEE) or delete existing ones.
- **Account Management** — List, create, and update your investment accounts directly.
- **Market Data** — Fetch the latest market prices for any asset symbol supported by Ghostfolio.

### How it works

1. Subscribe to this server
2. Enter your Ghostfolio API Key (and optionally your instance URL)
3. Start managing your investments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Individual Investors** — track your net worth and asset allocation without manual spreadsheet updates.
- **Financial Analysts** — quickly query portfolio metrics and market data during research.
- **Wealth Managers** — manage multiple accounts and activities through a streamlined AI interface.


## Available Tools
- **list_accounts**: List all investment accounts
- **list_activities**: ) from Ghostfolio.

Retrieve a list of all activities
- **create_account**: Provide the account details as a JSON payload.

Create a new investment account
- **create_activity**: Create a new investment activity
- **delete_activity**: Delete a specific activity
- **get_market_data_price**: Get the latest price for a specific symbol
- **get_portfolio_holdings**: Get current holdings and their valuations
- **get_portfolio_summary**: Get a summary of the portfolio performance
- **update_account**: Update account details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ghostfolio (Investment Tracker)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a summary of my portfolio performance."

**🤖 AI Agent:**
> I've retrieved your portfolio summary. Your total net worth is $125,430.50, with a total gain of +12.4% ($13,850.20). Your best performing asset is NVIDIA (+45%).

---

**👤 You:**
> "List all my investment accounts in Ghostfolio."

**🤖 AI Agent:**
> You have 3 active accounts: 'Main Brokerage' (USD), 'Crypto Wallet' (BTC), and 'Retirement Fund' (EUR). Which one would you like to inspect?

---

**👤 You:**
> "Record a purchase of 10 shares of AAPL at $185.50 in my Main Brokerage account."

**🤖 AI Agent:**
> I've successfully recorded the BUY activity for 10 shares of AAPL at $185.50. The transaction has been added to your 'Main Brokerage' account.


## Installation & Usage

To install and use the **Ghostfolio (Investment Tracker)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ghostfolio-investment-tracker](https://vinkius.com/mcp/ghostfolio-investment-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
