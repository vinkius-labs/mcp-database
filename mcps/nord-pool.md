# Nord Pool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nord-pool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access European electricity market data via Nord Pool — query day-ahead prices, auction volumes, cross-border flows, and consumption forecasts from any AI agent.

## Description
Tap into the heartbeat of the European power market with **Nord Pool** — the continent's leading electricity exchange operating across 16 countries.

### What you can do

- **Day-Ahead Prices** — Retrieve clearing prices for any bidding zone (NO1, SE3, DK1, DE-LU, FR, NL, and more) in 15-minute Market Time Units
- **Yearly Price Trends** — Analyze long-term electricity price patterns and year-over-year performance for any delivery area
- **Auction Volumes** — Query traded volumes (MWh) per area to understand market depth and liquidity
- **Transmission Capacities** — Inspect Available Transmission Capacity (ATC) between interconnected bidding zones
- **Cross-Border Flows** — Track commercial auction flows and scheduled physical power transfers between regions
- **Flow-Based Constraints** — Access flow-based market coupling parameters for Core and Nordic domains
- **Consumption Forecasts** — Pull load forecasts that drive trading strategies and grid balancing decisions
- **Subscription Validation** — Verify which data products are available on your API account

### How it works

1. Subscribe to this server
2. Enter your Nord Pool API Client ID and Client Secret
3. Start querying live European electricity market data from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes a real-time energy market analyst — no spreadsheets, no manual data exports, no switching between dashboards.

### Who is this for?

- **Energy Traders** — instantly pull day-ahead clearing prices and cross-border capacity to inform intraday positions
- **Portfolio Managers** — compare yearly price trends across multiple bidding zones without leaving the conversation
- **Grid Operators and Analysts** — access consumption forecasts and transmission capacities for operational planning
- **Research Teams** — automate the extraction of historical auction data for market modeling and forecasting


## Available Tools
- **get_auction_flows**: Requires both source and destination area codes. Flows reflect the scheduled energy exchange determined during the day-ahead market coupling process. Optionally filter by delivery date (YYYY-MM-DD).

Retrieve auction flows between two delivery areas
- **get_auction_volumes**: Use standard bidding zone codes separated by commas. Optionally filter by delivery date (YYYY-MM-DD). Volumes indicate the total cleared energy quantity per Market Time Unit in each area.

Retrieve day-ahead auction volumes for specified delivery areas
- **get_transmission_capacities**: Requires both source and destination area codes (e.g. NO1 to SE3). ATC represents the maximum commercial power transfer capacity allocated for the day-ahead market coupling. Optionally filter by delivery date (YYYY-MM-DD).

Retrieve Available Transmission Capacities (ATC) between two delivery areas
- **get_consumption_forecasts**: These forecasts represent the expected electricity consumption (load) for each Market Time Unit within a delivery area. Use standard bidding zone codes separated by commas. Optionally filter by delivery date (YYYY-MM-DD). Consumption forecasts are essential for production planning, trading strategy, and grid balancing decisions.

Retrieve power consumption forecasts by delivery area
- **get_day_ahead_prices**: Delivery areas are standard European bidding zone codes such as NO1, NO2, SE1, SE2, SE3, SE4, DK1, DK2, FI, EE, LV, LT, DE-LU, AT, FR, NL, BE, PL. You can pass multiple areas separated by commas. Optionally filter by a specific delivery date (YYYY-MM-DD) and currency (EUR, NOK, SEK, DKK, PLN, GBP). Prices are returned in 15-minute Market Time Units (MTU) by default since the transition to 15-min resolution in SDAC.

Retrieve day-ahead auction prices for specified delivery areas
- **get_flow_based_constraints**: Flow-based constraints define the allowable power transfer limits in flow-based market coupling regions (e.g. Core, Nordic). The domain parameter specifies which regional coupling zone to query. Optionally filter by delivery date (YYYY-MM-DD).

Retrieve flow-based constraints for a market coupling domain
- **get_scheduled_physical_flows**: These flows represent the planned physical cross-border electricity transfers, including both commercial exchanges and loop flows. Requires source and destination area codes. Optionally filter by delivery date.

Retrieve scheduled physical flows between two delivery areas
- **get_user_subscriptions**: Use this tool to verify which data products (Day-Ahead, Intraday, Power System Data, etc.) are available to the current credentials before attempting to query specific endpoints.

List the active API data subscriptions for the authenticated account
- **get_yearly_prices**: Use standard bidding zone codes (e.g. NO1, SE3, DE-LU). Optionally filter by year (YYYY) and currency. Useful for long-term price trend analysis and year-over-year comparisons.

Retrieve yearly aggregated auction prices for a delivery area
- **get_yearly_volumes**: Useful for analyzing annual energy consumption and trading patterns within a specific bidding zone.

Retrieve yearly aggregated auction volumes for a delivery area


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nord Pool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the day-ahead electricity prices for Norway zone NO1 and Sweden zone SE3 for tomorrow?"

**🤖 AI Agent:**
> I have retrieved the day-ahead clearing prices for NO1 and SE3. Norway NO1 shows an average of 42.15 EUR/MWh with a peak at 67.80 EUR/MWh between 17:00-18:00. Sweden SE3 averages 39.20 EUR/MWh, with converging prices in off-peak hours. The spread between zones is approximately 2.95 EUR/MWh. Would you like me to also pull the transmission capacity between NO1 and SE3?

---

**👤 You:**
> "Show me the cross-border transmission capacity from Denmark DK1 to Germany DE-LU for today."

**🤖 AI Agent:**
> Here is the Available Transmission Capacity (ATC) from DK1 to DE-LU. The interconnector shows 1,700 MW of available capacity during off-peak hours and drops to 1,200 MW during peak demand between 08:00-20:00. The capacity utilization rate is running at approximately 78%. Shall I overlay the actual auction flows for the same corridor so you can compare scheduled transfers against available capacity?

---

**👤 You:**
> "Compare the yearly electricity prices for Finland and the Baltic states for the last two years."

**🤖 AI Agent:**
> I have pulled the yearly aggregate data for four zones. Finland (FI): 2024 averaged 51.30 EUR/MWh, 2025 dropped to 43.80 EUR/MWh (-14.6%). Estonia (EE): dropped from 62.10 to 48.90 EUR/MWh (-21.3%). Latvia (LV): from 59.40 to 47.20 EUR/MWh. Lithuania (LT): from 58.80 to 46.50 EUR/MWh. All Baltic zones converged closer to Finnish levels over the period. Shall I also get the corresponding volume data to see if consumption patterns shifted?


## ❓ FAQ

**Q: How do I get started with Nord Pool market data?**
Subscribe, enter your API credentials (Client ID and Client Secret from the **Nord Pool Developer Portal** at developers.nordpoolgroup.com), and you are ready. Your AI agent can immediately start pulling day-ahead prices, auction volumes, and consumption forecasts across all 16 European markets. No code, no SDK, no webhooks — just connect and start analyzing electricity data through your AI agent. It takes exactly 30 seconds — no complex OAuth apps, no manual logging, and no approval processes required. Your token is encrypted at rest and injected securely at runtime.

**Q: Can my AI agent compare electricity prices across multiple European bidding zones in a single request?**
Absolutely. Pass multiple bidding zone codes (like NO1,SE3,DK1,DE-LU) separated by commas, and your agent returns the full day-ahead price curve for each zone side by side. You can filter by specific delivery dates and currencies — perfect for spotting price spreads, identifying arbitrage opportunities, and benchmarking regional tariffs without opening a single spreadsheet.

**Q: What happens when I need to analyze cross-border transmission capacity or energy flows between countries?**
Simply tell your AI agent the source and destination bidding zones (e.g. NO1 to SE3, or DK1 to DE-LU). It will pull Available Transmission Capacities (ATC), commercial auction flows, and scheduled physical power transfers for the specified interconnection — all in a single conversation. No need to navigate the data portal, download CSVs, or run custom scripts. Your agent handles the complete cross-border analysis workflow end to end.

**Q: Can I use this for long-term analysis and portfolio management across multiple markets?**
Yes. Beyond real-time day-ahead data, the server provides yearly aggregated price and volume tools that let you compare entire years of clearing prices side by side for any delivery area. Combined with consumption forecast tools, your AI agent can build a comprehensive market overview spanning 16 European countries — ideal for energy portfolio managers, utility analysts, and research teams tracking price volatility, seasonal patterns, and demand-supply fundamentals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nord-pool](https://vinkius.com/mcp/nord-pool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nord Pool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nord-pool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nord Pool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nord-pool": {
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
