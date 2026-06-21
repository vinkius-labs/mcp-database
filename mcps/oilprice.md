# OilPrice MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/oilprice)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time and historical oil, gas, and energy commodity prices — WTI, Brent, Natural Gas, Diesel, and 40+ more via OilPriceAPI.

## Description
Connect to **OilPriceAPI** and bring real-time energy commodity intelligence to any AI agent. Access 50+ energy commodities with prices updated every 5 minutes.

### What you can do

- **WTI Crude Oil** — Get current and historical West Texas Intermediate crude prices, the primary US oil benchmark
- **Brent Crude** — Track international crude oil prices, the global benchmark for oil trading
- **Natural Gas** — Monitor Henry Hub natural gas prices updated every 5 minutes
- **Refined Products** — Access diesel, gasoline, heating oil, and jet fuel prices
- **Coal** — Track Newcastle thermal coal benchmarks
- **Latest Prices** — Fetch current spot prices for any or all commodities
- **Intraday Data** — Analyze hourly price movements over the last 24 hours
- **Weekly Trends** — Review daily prices for the last 7 days
- **Monthly Analysis** — Examine daily prices for the last 30 days
- **Historical Data** — Query custom date ranges for long-term trend analysis (paid tier)
- **Commodity Catalog** — Explore all 50+ available energy commodities and their codes

### How it works

1. Subscribe to this server
2. Enter your OilPriceAPI key (free 7-day trial with 10,000 requests available)
3. Start querying energy prices from Claude, Cursor, or any MCP-compatible client

Your AI becomes an energy analyst, helping you track commodity prices, understand market dynamics, and make data-driven decisions.

### Who is this for?

- **Energy Traders** — monitor real-time WTI, Brent, and natural gas prices for trading opportunities
- **Procurement Teams** — track fuel costs (diesel, gasoline, jet fuel) to optimize purchasing timing
- **Researchers & Analysts** — access historical price data for market studies and publications
- **Logistics Managers** — monitor diesel and gasoline prices for fleet cost management
- **Investment Professionals** — integrate commodity price feeds into portfolio analysis
- **Aviation & Shipping** — track jet fuel and diesel prices for operational cost planning


## Available Tools (10)
- **get_brent_price**: Prices update every 5 minutes.

USE WHEN:
- User asks specifically about Brent oil price
- User needs the international crude oil benchmark
- User wants to check European/global oil prices
- User asks "what is Brent price"

EXAMPLES:
- "What is Brent price?" → call with no params
- "Current Brent crude oil price" → call with no params
- "Brent oil benchmark" → call with no params

Get current Brent crude oil price
- **list_commodities**: USE WHEN:
- User wants to explore what commodities are available
- User needs to find commodity codes for querying prices
- User is exploring the API capabilities for the first time
- User asks what energy commodities are supported

AVAILABLE COMMODITY TYPES:
- Crude Oil: WTI_USD, BRENT_CRUDE_USD
- Refined Products: DIESEL_USD, GASOLINE_USD, HEATING_OIL_USD, JET_FUEL_USD
- Natural Gas: NATURAL_GAS_USD
- Coal: COAL_USD
- And 40+ more energy commodities

EXAMPLES:
- "What commodities are available?" → call with no params
- "Show me all commodity codes" → call with no params
- "List all energy products" → call with no params

List all available energy commodities in OilPriceAPI
- **get_diesel_price**: Important for tracking transportation fuel costs and refined product margins.

USE WHEN:
- User asks about diesel fuel prices
- User needs refined product pricing
- User wants to track diesel vs crude crack spreads
- User asks "what is diesel price"

EXAMPLES:
- "What is diesel price?" → call with no params
- "Current ULSD diesel price" → call with no params
- "US diesel fuel cost" → call with no params

Get current US Diesel (Ultra Low Sulfur) price
- **get_historical_prices**: Requires a paid OilPriceAPI subscription.

USE WHEN:
- User asks about historical oil prices for a specific period
- User wants long-term trend analysis or backtesting
- User asks for prices from specific dates

EXAMPLES:
- "WTI prices for Q1 2026" → commodity_code="WTI_USD", start_date="2026-01-01", end_date="2026-03-31"
- "Brent crude last year" → commodity_code="BRENT_CRUDE_USD", start_date="2025-01-01", end_date="2025-12-31"

Get historical price data for a custom date range
- **get_latest_prices**: Prices are updated every 5 minutes for oil, gas, and refined products.

USE WHEN:
- User asks about current oil prices
- User needs the latest commodity prices
- User wants to check current WTI or Brent prices
- User asks what is the price of oil/gas/coal right now

PARAMETERS:
- commodity_code (OPTIONAL): Specific commodity code (e.g. "WTI_USD", "BRENT_CRUDE_USD")

EXAMPLES:
- "What is current oil price?" → call with commodity_code="WTI_USD"
- "Latest Brent crude price" → call with commodity_code="BRENT_CRUDE_USD"
- "Show all latest energy prices" → call with no params

Get the latest spot prices for energy commodities
- **get_natural_gas_price**: Prices update every 5 minutes.

USE WHEN:
- User asks about natural gas prices
- User needs the US natural gas benchmark
- User wants to check Henry Hub prices
- User asks "what is natural gas price"

EXAMPLES:
- "What is natural gas price?" → call with no params
- "Current Henry Hub gas price" → call with no params
- "US natural gas benchmark" → call with no params

Get current US Natural Gas (Henry Hub) price
- **get_past_day_prices**: Perfect for tracking intraday price movements and volatility.

USE WHEN:
- User asks about oil price movements today
- User needs hourly price data for the last day
- User wants to track intraday volatility
- User asks how prices changed in the last 24 hours

PARAMETERS:
- commodity_code (OPTIONAL): Specific commodity code

EXAMPLES:
- "Show WTI price movements today" → call with commodity_code="WTI_USD"
- "Hourly natural gas prices last 24h" → call with commodity_code="NATURAL_GAS_USD"
- "Brent crude intraday prices" → call with commodity_code="BRENT_CRUDE_USD"

Get hourly prices data for the last 24 hours
- **get_past_month_prices**: Great for monthly trend analysis and medium-term price tracking.

USE WHEN:
- User asks about oil price trends this month
- User needs daily prices for the last 30 days
- User wants to track monthly price movements
- User asks how prices changed over the past month

PARAMETERS:
- commodity_code (OPTIONAL): Specific commodity code

EXAMPLES:
- "WTI price trends this month" → call with commodity_code="WTI_USD"
- "Monthly natural gas prices" → call with commodity_code="NATURAL_GAS_USD"
- "Brent crude last 30 days" → call with commodity_code="BRENT_CRUDE_USD"

Get daily price data for the last 30 days
- **get_past_week_prices**: Ideal for weekly trend analysis and short-term price tracking.

USE WHEN:
- User asks about oil price trends this week
- User needs daily prices for the last week
- User wants to track weekly price movements
- User asks how prices changed over the past week

PARAMETERS:
- commodity_code (OPTIONAL): Specific commodity code

EXAMPLES:
- "WTI price trends this week" → call with commodity_code="WTI_USD"
- "Weekly natural gas prices" → call with commodity_code="NATURAL_GAS_USD"
- "Brent crude last 7 days" → call with commodity_code="BRENT_CRUDE_USD"

Get daily price data for the last 7 days
- **get_wti_price**: Prices update every 5 minutes.

USE WHEN:
- User asks specifically about WTI oil price
- User needs the US crude oil benchmark
- User wants to check American oil prices
- User asks "what is WTI price"

EXAMPLES:
- "What is WTI price?" → call with no params
- "Current WTI crude oil price" → call with no params
- "West Texas Intermediate price" → call with no params

Get current WTI (West Texas Intermediate) crude oil price


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OilPrice** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current price of WTI crude oil?"

**🤖 AI Agent:**
> Fetching latest WTI price... Current WTI Crude is trading at $78.45 USD per barrel. The price was last updated 2 minutes ago. WTI has been trading in a $77-79 range this session.

---

**👤 You:**
> "Show me natural gas prices for the last week."

**🤖 AI Agent:**
> Retrieving past week natural gas prices... Henry Hub Natural Gas has traded between $2.72-$2.95/MMBtu over the last 7 days. Current price is $2.85/MMBtu, up 3% from last week. Prices have been supported by increased heating demand and steady LNG export volumes.

---

**👤 You:**
> "Compare WTI and Brent crude prices today."

**🤖 AI Agent:**
> Fetching both benchmarks... WTI Crude is at $78.45/bbl while Brent Crude is at $82.30/bbl. The WTI-Brent spread is currently $3.85, which is within the normal range. Brent's premium reflects tighter global supply and stronger international demand compared to US inventories.


## ❓ FAQ

**Q: How often are oil and gas prices updated?**
Oil, gas, and refined product prices (WTI, Brent, Natural Gas, Diesel, Gasoline, etc.) are updated every 5 minutes during market hours. Coal prices update daily. This ensures you have near real-time data for trading decisions and cost monitoring.

**Q: How do I get an OilPriceAPI key and what does the free trial include?**
Visit https://oilpriceapi.com/ and sign up for a free account. The 7-day free trial includes 10,000 API requests, access to all 50+ commodities, all endpoints (latest, past day, past week, past month), and no credit card required. After the trial, paid plans start at $15/month. Rate limit on free tier: 60 requests/minute.

**Q: What commodity codes are available?**
The API offers 50+ energy commodities. Key codes include: WTI_USD (WTI Crude), BRENT_CRUDE_USD (Brent Crude), NATURAL_GAS_USD (Henry Hub Gas), DIESEL_USD (Ultra Low Sulfur Diesel), GASOLINE_USD (RBOB Gasoline), HEATING_OIL_USD (No. 2 Heating Oil), JET_FUEL_USD (Aviation Fuel/Kerosene), COAL_USD (Newcastle Thermal Coal). Use the `list_commodities` tool to see the full catalog.

**Q: Can I access historical price data for trend analysis?**
Yes! The free tier includes past_day (24h hourly), past_week (7d daily), and past_month (30d daily) endpoints. For custom date ranges beyond 30 days, use the `get_historical_prices` tool which requires a paid subscription. This is ideal for long-term trend analysis, backtesting trading strategies, and academic research.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oilprice](https://vinkius.com/mcp/oilprice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OilPrice** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `oilprice` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OilPrice** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "oilprice": {
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
