# Coinbase MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coinbase)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Get real-time cryptocurrency prices, exchange rates and currency info — BTC, ETH, SOL and more.

## Description
Connect to **Coinbase** and access real-time cryptocurrency market data through natural conversation — no API key needed for public price data.

### What you can do

- **Buy/Sell Prices** — Get current buy and sell prices for any trading pair
- **Spot Prices** — Get mid-market spot prices (historical prices supported)
- **Multi-Asset Prices** — Get prices for multiple pairs in one call
- **Currencies** — Browse all supported cryptocurrencies and fiat currencies
- **Exchange Rates** — Get exchange rates from any base currency
- **Payment Methods** — View available payment methods on your account

### How it works

1. Subscribe to this server
2. No API key needed for public price data
3. Start exploring crypto prices from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Traders** — check real-time buy/sell prices and spreads before trading
- **Investors** — track crypto prices, compare exchange rates and monitor market data
- **Developers** — integrate crypto price data into apps and dashboards


## Available Tools
- **get_buy_price**: Returns the total price including Coinbase fees. Common pairs: BTC-USD, ETH-USD, SOL-USD, USDC-USD. Prices update in real-time and are only valid for seconds.

Get the current buy price for a cryptocurrency pair
- **get_currencies**: Returns currency codes, names, min/max precision, sort order and whether the currency is a cryptocurrency or fiat.

Get all supported cryptocurrencies and fiat currencies
- **get_exchange_rates**: Returns rates for crypto and fiat currencies. Useful for currency conversion.

Get current exchange rates for a currency
- **get_payment_methods**: Returns bank accounts, debit cards and other payment options with their IDs, types, limits and verification status.

Get available payment methods
- **get_public_prices**: Provide comma-separated pairs (e.g. "BTC-USD,ETH-USD,SOL-USD"). Useful for comparing prices across multiple assets quickly.

Get buy, sell and spot prices for multiple cryptocurrency pairs at once
- **get_sell_price**: Returns the total price you would receive including Coinbase fees. Common pairs: BTC-USD, ETH-USD, SOL-USD.

Get the current sell price for a cryptocurrency pair
- **get_spot_price**: This is the mid-market price without buy/sell spread. Optional date parameter for historical prices (YYYY-MM-DD UTC).

Get the current spot (market) price for a cryptocurrency pair
- **get_time**: Useful for synchronizing requests and verifying API connectivity.

Get the current Coinbase API server time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coinbase** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the current Bitcoin price?"

**🤖 AI Agent:**
> BTC-USD: Buy $104,250 | Sell $103,890 | Spot $104,070. Spread: $360 (0.35%).

---

**👤 You:**
> "Compare prices for BTC, ETH and SOL."

**🤖 AI Agent:**
> BTC-USD: Buy $104,250 / Sell $103,890 | ETH-USD: Buy $3,245 / Sell $3,210 | SOL-USD: Buy $185.50 / Sell $183.20.

---

**👤 You:**
> "What was the Bitcoin price on January 1st 2024?"

**🤖 AI Agent:**
> BTC-USD spot price on 2024-01-01: $42,650. Current price: $104,070. Change: +144.0% since Jan 1 2024.


## ❓ FAQ

**Q: Do I need an API key for price data?**
No! Public price endpoints (buy, sell, spot prices, currencies, exchange rates) are completely free and open. No authentication required.

**Q: What trading pairs are supported?**
Common pairs: BTC-USD, ETH-USD, SOL-USD, USDC-USD, BCH-USD, LTC-USD, DOGE-USD, ADA-USD, DOT-USD, LINK-USD and many more. Use getCurrencies to see the full list.

**Q: Can I get historical prices?**
Yes! Use get_spot_price with the date parameter (YYYY-MM-DD format) to get historical spot prices for any pair.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coinbase](https://vinkius.com/mcp/coinbase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coinbase** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `coinbase` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coinbase** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coinbase": {
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
