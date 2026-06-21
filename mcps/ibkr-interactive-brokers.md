# IBKR (Interactive Brokers) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ibkr-interactive-brokers)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage your Interactive Brokers account — execute trades, monitor portfolio ledgers, and fetch real-time market data via the Client Portal API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IBKR (Interactive Brokers)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get a market data snapshot for ConId 265598."

**🤖 AI Agent:**
> I've retrieved the market data for ConId 265598 (AAPL). The last price is $185.92 with a daily change of +1.2%.

---

**👤 You:**
> "Show me the account summary for account U1234567."

**🤖 AI Agent:**
> For account U1234567, your Net Liquidation Value is $50,230.45, with a Total Cash Balance of $12,400.10 and Maintenance Margin of $15,000.00.

---

**👤 You:**
> "Cancel order 1001 for account U1234567."

**🤖 AI Agent:**
> I have successfully sent a cancellation request for order ID 1001 on account U1234567. The status is now 'Cancelled'.


## ❓ FAQ

**Q: How do I prevent my IBKR API session from timing out?**
You can use the `tickle_session` tool. It is designed to maintain the Client Portal API session by sending a heartbeat, preventing timeouts due to inactivity.

**Q: Can I retrieve historical trade reports through this server?**
Yes. First, use `send_flex_request` with your Flex Query ID to generate a report. Then, use the returned Reference Code with `get_flex_statement` to download the data.

**Q: How do I check my current buying power and margin requirements?**
Use the `get_account_summary` tool with your Account ID. It returns a comprehensive summary of equity, margin, and other key financial metrics for the specified account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibkr-interactive-brokers](https://vinkius.com/mcp/ibkr-interactive-brokers)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IBKR (Interactive Brokers)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ibkr-interactive-brokers` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IBKR (Interactive Brokers)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ibkr-interactive-brokers": {
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
