# S&P Global Commodity Insights MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sp-global-commodity-insights)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access global commodity price assessments — crude oil, natural gas, power, coal, metals, petrochemicals, and agriculture via S&P Global Platts benchmarks.

## Description
Connect to **S&P Global Commodity Insights API** and bring world-class commodity intelligence to any AI agent. Access over 12,000 daily price assessments from Platts, the industry-standard benchmark for global commodity trading.

### What you can do

- **Crude Oil Prices** — Retrieve daily price assessments for WTI, Brent, Dubai, Mars, WCS and hundreds of crude grades worldwide
- **Natural Gas** — Access Henry Hub, TTF, NBP, JKM and other major gas hub benchmarks with spot and forward prices
- **Electric Power** — Query wholesale electricity prices for PJM, ERCOT, CAISO, European and Asia-Pacific power markets
- **Coal** — Monitor Newcastle, API2, API4 and regional thermal/metallurgical coal benchmarks
- **Refined Products** — Track gasoline (RBOB, Eurobob), diesel (ULSD, Gasoil), jet fuel and fuel oil prices globally
- **Petrochemicals** — Get ethylene, propylene, benzene, toluene and other chemical feedstock prices
- **Metals** — Access base metals (copper, aluminum, zinc), precious metals (gold, silver) and steel/iron ore benchmarks
- **Agriculture** — Query wheat, corn, soybeans, fertilizers (urea, DAP, potash) and other agricultural commodities
- **Energy Transition** — Monitor carbon credits (EUA, RINs), battery metals (lithium, cobalt), RECs and green hydrogen assessments
- **Historical Analysis** — Fetch historical price data with flexible date ranges for trend analysis and backtesting
- **Methodology Access** — Retrieve specification documents and calculation methods for any price assessment
- **Category Exploration** — Browse the complete commodity catalog to discover available benchmarks

### How it works

1. Subscribe to this server
2. Enter your S&P Global Commodity Insights API key (requires active subscription)
3. Start querying global commodity prices from Claude, Cursor, or any MCP-compatible client

Your AI becomes a commodity analyst, helping you track prices, understand market dynamics, and make data-driven trading decisions.

### Who is this for?

- **Energy Traders** — monitor real-time crude, gas, and power prices across global hubs for arbitrage opportunities
- **Procurement Teams** — track input costs (feedstocks, energy, metals) to optimize purchasing timing
- **Researchers & Analysts** — access historical price data and methodology documents for market studies
- **Risk Managers** — monitor commodity exposure and benchmark prices for hedging decisions
- **Investment Professionals** — integrate commodity price feeds into portfolio analysis and due diligence
- **Sustainability Teams** — track carbon credits, battery metals, and energy transition benchmarks for ESG reporting


## Available Tools
- **get_agriculture_prices**: USE WHEN:
- User asks about agriculture commodity prices
- User needs wheat, corn, soybean, or other crop prices
- User wants agricultural market benchmarks
- User asks about food commodity pricing

AVAILABLE COMMODITIES:
- Wheat, Corn, Soybeans, Soybean Meal/Oil
- Rice, Barley, Oats
- Fertilizers (Urea, DAP, Potash)

PARAMETERS:
- date (OPTIONAL): Specific date (YYYY-MM-DD)
- commodity (OPTIONAL): Specific commodity (e.g. "Wheat", "Corn")
- region (OPTIONAL): Region of origin/destination

EXAMPLES:
- "Wheat prices today" → call with commodity="Wheat"
- "Corn prices this week" → call with commodity="Corn"
- "Urea fertilizer prices" → call with commodity="Urea"

Get agriculture commodity price assessments from S&P Global Platts
- **get_assessment_methodology**: USE WHEN:
- User asks about how a specific price is calculated
- User needs the methodology behind a benchmark
- User wants specification details for an assessment
- User asks about market conventions for a commodity

PARAMETERS:
- assessment_code (REQUIRED): Assessment code or symbol (e.g. "WTI_Cushing", "Henry_Hub")

EXAMPLES:
- "How is WTI Cushing price calculated?" → call with assessment_code="WTI_Cushing"
- "Henry Hub methodology" → call with assessment_code="Henry_Hub"
- "Brent assessment specifications" → call with assessment_code="Brent"

Get methodology and metadata for a specific price assessment
- **list_commodity_categories**: USE WHEN:
- User wants to explore what commodity categories are available
- User needs to understand the scope of price assessments
- User is exploring the API capabilities for the first time
- User asks what types of commodities are covered

CATEGORIES INCLUDE:
- Crude Oil, Natural Gas, Electric Power, Coal
- Petrochemicals, Metals, Agriculture
- Energy Transition, Refined Products

EXAMPLES:
- "What commodity categories are available?" → call with no params
- "Show me all commodity types" → call with no params
- "List all price assessment categories" → call with no params

List all available commodity categories in S&P Global Commodity Insights
- **get_coal_prices**: USE WHEN:
- User asks about coal prices
- User needs Newcastle, API2, or other coal benchmark prices
- User wants thermal or metallurgical coal market data
- User asks about coal market trends

AVAILABLE BENCHMARKS:
- Newcastle (Australia), API2 (Rotterdam)
- API4 (Richards Bay), Columbian FOB
- Various regional thermal and coking coal prices

PARAMETERS:
- date (OPTIONAL): Specific date (YYYY-MM-DD)
- type (OPTIONAL): Coal type ("thermal" or "metallurgical")
- benchmark (OPTIONAL): Specific benchmark (e.g. "Newcastle", "API2")

EXAMPLES:
- "Newcastle coal price today" → call with benchmark="Newcastle"
- "Thermal coal prices this week" → call with type="thermal"
- "API2 Rotterdam coal prices" → call with benchmark="API2"

Get coal price assessments from S&P Global Platts
- **get_crude_oil_prices**: Includes spot and forward prices for major crude grades.

USE WHEN:
- User asks about crude oil prices or benchmarks
- User needs WTI, Brent, Dubai, or other crude grade prices
- User wants historical or current oil price assessments
- User asks about oil market pricing

AVAILABLE CRUDE GRADES:
- WTI (West Texas Intermediate), Brent, Dubai/Oman
- Mars, LLS, WCS, Forties, and many regional grades

PARAMETERS:
- date (OPTIONAL): Specific date for assessment (YYYY-MM-DD format, defaults to latest)
- region (OPTIONAL): Filter by region (e.g. "US", "Middle East", "North Sea")
- grade (OPTIONAL): Specific crude grade (e.g. "WTI", "Brent")

EXAMPLES:
- "What is current WTI crude oil price?" → call with grade="WTI"
- "Brent oil prices this week" → call with grade="Brent", date="2026-04-07"
- "Middle East crude assessments" → call with region="Middle East"

Get crude oil price assessments from S&P Global Platts
- **get_energy_transition_data**: USE WHEN:
- User asks about renewable energy prices or markets
- User needs carbon credit or EUA (EU Allowance) prices
- User wants battery metal assessments (lithium, cobalt)
- User asks about energy transition or sustainability metrics

AVAILABLE DATA:
- Carbon credits (EUA, RINs, LCFS)
- Battery metals (Lithium, Cobalt, Graphite)
- Renewable energy certificates (RECs)
- Green hydrogen assessments

PARAMETERS:
- date (OPTIONAL): Specific date (YYYY-MM-DD)
- category (OPTIONAL): Category (e.g. "carbon", "battery_metals", "renewables")

EXAMPLES:
- "Carbon credit prices today" → call with category="carbon"
- "Lithium prices for batteries" → call with category="battery_metals"
- "EU Allowance (EUA) prices" → call with category="carbon"

Get energy transition market data and assessments
- **get_historical_commodity_prices**: Essential for trend analysis, backtesting, and market research.

USE WHEN:
- User asks about historical price trends
- User needs price data over a specific time period
- User wants to compare prices across dates
- User asks for weekly, monthly, or yearly price history

PARAMETERS:
- commodity (REQUIRED): Commodity identifier (e.g. "crude-oil", "natural-gas", "coal")
- start_date (REQUIRED): Start date (YYYY-MM-DD)
- end_date (OPTIONAL): End date (YYYY-MM-DD, defaults to today)
- frequency (OPTIONAL): Data frequency ("daily", "weekly", "monthly")

EXAMPLES:
- "WTI oil prices for last 30 days" → call with commodity="crude-oil", start_date="2026-03-08"
- "Natural gas prices this month" → call with commodity="natural-gas", start_date="2026-04-01"
- "Coal price history last quarter" → call with commodity="coal", start_date="2026-01-01", end_date="2026-03-31"

Get historical price data for a specific commodity with date range
- **get_metals_prices**: USE WHEN:
- User asks about metal prices
- User needs copper, aluminum, zinc, or other base metal prices
- User wants steel or iron ore benchmarks
- User asks about precious metals (gold, silver)

AVAILABLE METALS:
- Base: Copper, Aluminum, Zinc, Nickel, Lead
- Precious: Gold, Silver, Platinum
- Steel, Iron Ore, Tin

PARAMETERS:
- date (OPTIONAL): Specific date (YYYY-MM-DD)
- metal (OPTIONAL): Specific metal (e.g. "Copper", "Aluminum")
- exchange (OPTIONAL): Exchange reference (e.g. "LME", "COMEX")

EXAMPLES:
- "Copper price today" → call with metal="Copper"
- "LME aluminum prices" → call with metal="Aluminum", exchange="LME"
- "Gold price assessment" → call with metal="Gold"

Get metals price assessments from S&P Global Platts
- **get_natural_gas_prices**: USE WHEN:
- User asks about natural gas prices
- User needs Henry Hub, NBP, TTF, or other gas hub prices
- User wants gas market pricing by region or hub
- User asks about LNG prices

AVAILABLE HUBS/INDICES:
- Henry Hub (US), NBP (UK), TTF (Netherlands)
- JKM (Japan/Korea Marker), Alberta (Canada)
- And many regional hubs globally

PARAMETERS:
- date (OPTIONAL): Specific date (YYYY-MM-DD)
- region (OPTIONAL): Region filter (e.g. "US", "Europe", "Asia")
- hub (OPTIONAL): Specific hub (e.g. "Henry Hub", "TTF")

EXAMPLES:
- "Current Henry Hub natural gas price" → call with hub="Henry Hub"
- "European gas prices today" → call with region="Europe", date="2026-04-07"
- "JKM LNG prices this week" → call with hub="JKM"

Get natural gas price assessments from S&P Global Platts
- **get_petrochemicals_prices**: USE WHEN:
- User asks about petrochemical or chemical prices
- User needs ethylene, propylene, benzene, or other chemical prices
- User wants petrochemical feedstock pricing
- User asks about chemical market benchmarks

AVAILABLE CHEMICALS:
- Ethylene, Propylene, Benzene, Toluene
- Xylene, Butadiene, Methanol
- Various polymer and derivative prices

PARAMETERS:
- date (OPTIONAL): Specific date (YYYY-MM-DD)
- region (OPTIONAL): Region (e.g. "US", "Europe", "Asia")
- chemical (OPTIONAL): Specific chemical name

EXAMPLES:
- "Ethylene prices today" → call with chemical="Ethylene"
- "Asian petrochemical prices this week" → call with region="Asia"
- "Benzene price assessments" → call with chemical="Benzene"

Get petrochemicals price assessments from S&P Global Platts
- **get_power_prices**: USE WHEN:
- User asks about electricity or power prices
- User needs wholesale power market prices
- User wants regional electricity benchmarks
- User asks about power trading hubs

AVAILABLE MARKETS:
- US regions (PJM, ERCOT, CAISO, NYISO, etc.)
- European power markets (EPEX, Nord Pool)
- Asia-Pacific power benchmarks

PARAMETERS:
- date (OPTIONAL): Specific date (YYYY-MM-DD)
- region (OPTIONAL): Region or market (e.g. "PJM", "ERCOT", "CAISO")
- hub (OPTIONAL): Specific trading hub

EXAMPLES:
- "PJM electricity prices today" → call with region="PJM", date="2026-04-07"
- "ERCOT power prices for Texas" → call with region="ERCOT"
- "European power prices this week" → call with region="Europe"

Get electric power price assessments from S&P Global Platts
- **get_refined_products_prices**: USE WHEN:
- User asks about gasoline, diesel, or jet fuel prices
- User needs refined product benchmarks (ULSD, RBOB)
- User wants fuel oil or lubricant prices
- User asks about refined product markets

AVAILABLE PRODUCTS:
- Gasoline (RBOB, Eurobob), Diesel (ULSD, Gasoil)
- Jet Fuel, Fuel Oil, Naphtha
- Lubricants, Bitumen, LPG

PARAMETERS:
- date (OPTIONAL): Specific date (YYYY-MM-DD)
- product (OPTIONAL): Specific product (e.g. "Diesel", "Gasoline")
- region (OPTIONAL): Region (e.g. "US", "Europe", "Singapore")

EXAMPLES:
- "Diesel prices today" → call with product="Diesel"
- "RBOB gasoline prices" → call with product="Gasoline"
- "Singapore jet fuel prices" → call with product="Jet Fuel", region="Singapore"

Get refined petroleum products price assessments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **S&P Global Commodity Insights** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current WTI crude oil price?"

**🤖 AI Agent:**
> Fetching latest WTI Cushing crude assessment... Current WTI is assessed at $78.45/bbl for today's session. The benchmark has been relatively stable this week, trading in a $77-79/bbl range. Market participants are monitoring OPEC+ production decisions and US inventory levels.

---

**👤 You:**
> "Show me natural gas prices at Henry Hub and TTF for today."

**🤖 AI Agent:**
> Retrieving gas hub assessments... Henry Hub (US) is currently assessed at $2.85/MMBtu, while TTF (Netherlands) is trading at €28.50/MWh (approximately $8.90/MMBtu). The spread between US and European gas remains elevated due to strong Asian LNG demand and European storage dynamics.

---

**👤 You:**
> "What are current carbon credit prices (EUA)?"

**🤖 AI Agent:**
> Fetching EU Allowance (EUA) carbon credit assessment... Current EUA price is €68.50/tonne CO2. Carbon prices have been volatile this month, ranging between €65-72/tonne as markets digest EU energy policy updates and industrial demand forecasts. The UK ETS is trading at a slight discount at £45.20/tonne.


## ❓ FAQ

**Q: What commodity types and benchmarks are covered?**
The API covers over 12,000 daily price assessments across: Crude Oil (WTI, Brent, Dubai, Mars, WCS + hundreds of grades), Natural Gas (Henry Hub, TTF, NBP, JKM), Electric Power (PJM, ERCOT, CAISO, European markets), Coal (Newcastle, API2, API4), Refined Products (gasoline, diesel, jet fuel), Petrochemicals (ethylene, propylene, benzene), Metals (copper, aluminum, gold, steel), Agriculture (wheat, corn, soybeans, fertilizers), and Energy Transition (carbon credits, battery metals, RECs).

**Q: How do I get an S&P Global Commodity Insights API key?**
API access requires an active S&P Global Commodity Insights subscription. Contact your S&P Global account manager or visit https://www.spglobal.com/commodityinsights to discuss licensing options. Once licensed, you'll receive API credentials through your SSO (Single Sign-On) account. The authentication uses Bearer tokens generated via the /auth/api endpoint with your SSO email and password.

**Q: Are the prices real-time or delayed?**
S&P Global Platts price assessments are published daily based on market activity. Most assessments reflect same-day or next-day values depending on the commodity and market. Some benchmarks (especially power markets) may have intra-day updates. Historical data is available for backtesting and trend analysis with flexible date range queries. The exact publication timing varies by commodity — crude oil and gas benchmarks are typically available by end of trading day.

**Q: Can I query historical prices for trend analysis?**
Yes! Use the `get_historical_commodity_prices` tool with a specific commodity identifier, start date, and optional end date. You can query daily, weekly, or monthly aggregated data. For example, to get WTI crude prices for the last 30 days, use commodity='crude-oil', start_date='2026-03-08'. The API provides extensive historical data suitable for backtesting, trend analysis, and market research.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sp-global-commodity-insights](https://vinkius.com/mcp/sp-global-commodity-insights)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **S&P Global Commodity Insights** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sp-global-commodity-insights` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **S&P Global Commodity Insights** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sp-global-commodity-insights": {
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
