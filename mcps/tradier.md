# Tradier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tradier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Trade equities and options, fetch real-time market data, and manage your brokerage accounts directly through any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tradier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current price and daily change for TSLA and MSFT?"

**🤖 AI Agent:**
> I've fetched the quotes for you. TSLA is currently trading at $242.10 (+1.2%) and MSFT is at $415.50 (-0.4%). Would you like to see the historical data for either of these?

---

**👤 You:**
> "Show me all open positions in my account 12345678."

**🤖 AI Agent:**
> In account 12345678, you currently hold 50 shares of AAPL and 10 contracts of SPY Dec 20 Put. Your total market value for these positions is approximately $12,400.

---

**👤 You:**
> "Get the option chain for NVDA expiring on 2025-01-17."

**🤖 AI Agent:**
> I've retrieved the option chain for NVDA for the Jan 17, 2025 expiration. There are 45 strikes available, ranging from $100 to $150. Would you like to filter for specific strikes or see the Greeks for the At-The-Money calls?


## ❓ FAQ

**Q: Can I check real-time prices for multiple stocks at once?**
Yes. Use the `get_quotes` tool and provide a comma-separated list of symbols (e.g., 'AAPL,TSLA,NVDA'). The agent will return the latest market data for all requested tickers.

**Q: Is it possible to view my current portfolio holdings and buying power?**
Absolutely. Use `get_account_positions` to see your current holdings and `get_account_balances` to check your available cash and buying power for a specific account ID.

**Q: Can I place option trades through this integration?**
Yes. The `place_order` tool supports both 'equity' and 'option' asset classes. You can specify the side (e.g., buy_to_open), quantity, and order type to execute your strategy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tradier](https://vinkius.com/mcp/tradier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tradier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tradier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tradier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tradier": {
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
