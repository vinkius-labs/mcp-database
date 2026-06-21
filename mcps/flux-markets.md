# Flux Markets MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flux-markets)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access energy market data, live pricing, and proprietary trade insights from Flux Markets.

## Description
Connect your **Flux Markets** (Onyx) account to any AI agent to monitor energy markets, track live pricing, and access proprietary 'Commitment of Traders' (COT) data. This MCP server enables you to manage your trading insights directly through natural conversation.

### What you can do

- **Live Tickers** — Get real-time biddable prices and market snapshots for energy contracts.
- **Historical Data** — Retrieve time-series data for backtesting and trend analysis.
- **Trade Insights** — Access Flux’s proprietary COT data and benchmark reports (The Officials).
- **Swap Settlements** — Track daily settlement prices for energy swaps.
- **Market Snapshot** — Get high-level summaries of current market statuses across various energy symbols.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Flux/Onyx API Key (obtained from your account page)
3. Start querying energy market data from Claude, Cursor, or any MCP client

### Who is this for?

- **Energy Traders** — quickly check live prices and market liquidity during active trading hours.
- **Market Analysts** — automate the retrieval of COT data and historical tickers for reports.
- **Risk Managers** — monitor daily settlement prices and market snapshots to manage exposure.


## Available Tools (9)
- **get_account_info**: Get account and API usage details
- **get_cot_data**: Get Commitment of Traders (COT) data
- **get_historical_tickers**: Get historical energy prices
- **get_live_tickers**: Get real-time energy prices
- **get_market_snapshot**: Get current market snapshot
- **get_officials**: Get benchmark reports (The Officials)
- **get_swap_settlements**: Get daily swap settlement prices
- **list_products**: List all energy products
- **list_symbols**: List energy symbols


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flux Markets** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the current live prices for BRENT and WTI oil swaps."

**🤖 AI Agent:**
> Fetching live tickers... Current BRENT price is $82.45 and WTI is $78.12. Market liquidity is currently high.

---

**👤 You:**
> "Get the Commitment of Traders (COT) report for fuel oil."

**🤖 AI Agent:**
> Accessing proprietary COT data... Managed money positions have increased by 5% this week, indicating a bullish sentiment.

---

**👤 You:**
> "List all energy symbols available for trading."

**🤖 AI Agent:**
> Retrieving energy symbols... I found 45 active symbols, including Crude, Gasoline, Heating Oil, and Natural Gas.


## ❓ FAQ

**Q: How do I get an API Key for Flux Markets?**
You can generate an API key from your Flux/Onyx Account page at https://onyxhub.co.

**Q: What energy products are covered?**
Flux Markets covers oil derivatives, crude oil, fuel oil, and various other energy swaps and futures.

**Q: Is real-time data supported?**
Yes, the 'get_live_tickers' tool provides real-time biddable prices and market snapshots.

**Q: Can I use this for risk management?**
Absolutely. You can monitor daily settlement prices and COT data to manage exposure and understand market positioning.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flux-markets](https://vinkius.com/mcp/flux-markets)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flux Markets** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flux-markets` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flux Markets** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flux-markets": {
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
