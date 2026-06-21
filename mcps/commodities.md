# Commodities MCP Server

Access real-time futures prices for 30+ commodities — gold, silver, oil, gas, wheat, coffee, copper, and more via Commodities-API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/commodities)

## Overview
**Category:** data-analytics
**Tools Count:** 12

## Description
Connect to **Commodities-API** and bring real-time futures market intelligence to any AI agent. Access 30+ commodities across precious metals, energy, agriculture, livestock, and industrial metals.

### What you can do

- **Precious Metals** — Get current futures prices for gold, silver, platinum, and palladium (CME/NYMEX)
- **Energy Commodities** — Track WTI crude oil, Brent crude, and natural gas prices (NYMEX/CME)
- **Agriculture** — Monitor wheat, corn, soybean, coffee, cocoa, sugar, cotton, and more (CBOT/CME)
- **Livestock** — Access live cattle, feeder cattle, lean hogs, and Class III milk prices (CME)
- **Industrial Metals** — Track copper and aluminum futures (CME)
- **Individual Quotes** — Get instant price for any specific commodity by code
- **Market Comparison** — Compare prices across multiple commodities simultaneously
- **Exchange Information** — Know which exchange (CME, NYMEX, CBOT) trades each commodity

### How it works

1. Subscribe to this server
2. Enter your Commodities-API key (free tier with 5,000 requests/month)
3. Start querying commodity futures from Claude, Cursor, or any MCP-compatible client

Your AI becomes a commodity analyst, helping you track futures prices, understand market dynamics, and make data-driven decisions.

### Who is this for?

- **Commodity Traders** — monitor real-time futures prices for trading opportunities across metals, energy, and agriculture
- **Procurement Teams** — track input costs (metals, energy, agricultural raw materials) to optimize purchasing timing
- **Researchers & Analysts** — access commodity price data for market studies and publications
- **Farmers & Producers** — monitor agricultural commodity prices for crop planning and hedging
- **Investment Professionals** — integrate commodity price feeds into portfolio analysis and diversification
- **Jewelry & Manufacturing** — track precious and industrial metals prices for cost management


## Available Tools
- **get_agriculture_commodities_prices**: Perfect for tracking agricultural markets.

USE WHEN:
- User asks about agriculture commodity prices
- User wants to see all agricultural commodities at once
- User needs to track food commodity pricing
- User asks "show me agriculture commodity prices"

EXAMPLES:
- "What are agriculture commodity prices?" → call with no params
- "Show me wheat, corn, coffee, cocoa prices" → call with no params
- "Agriculture market today" → call with no params

Get current prices for major agriculture commodities
- **get_brent_crude_oil_price**: Brent is the international oil benchmark used for global pricing.

USE WHEN:
- User asks about Brent oil prices
- User needs the international oil benchmark
- User wants to compare WTI vs Brent spread
- User asks "what is Brent price"

EXAMPLES:
- "What is Brent oil price?" → call with no params
- "Current Brent crude price" → call with no params
- "Brent oil benchmark today" → call with no params

Get current Brent crude oil futures price
- **get_coffee_price**: Coffee is one of the most traded agricultural commodities globally.

USE WHEN:
- User asks about coffee prices
- User needs the soft commodity benchmark
- User wants to track agricultural pricing
- User asks "what is coffee price"

EXAMPLES:
- "What is coffee price?" → call with no params
- "Current coffee futures price" → call with no params
- "Coffee spot price today" → call with no params

Get current coffee futures price
- **get_copper_price**: Copper is known as "Dr. Copper" for its ability to predict economic health.

USE WHEN:
- User asks about copper prices
- User needs the industrial metals benchmark
- User wants to track economic indicators
- User asks "what is copper price"

EXAMPLES:
- "What is copper price?" → call with no params
- "Current copper futures price" → call with no params
- "Copper spot price today" → call with no params

Get current copper futures price
- **get_crude_oil_price**: WTI is the primary US oil benchmark.

USE WHEN:
- User asks about crude oil prices
- User needs the US oil benchmark
- User wants to check WTI pricing
- User asks "what is oil price"

EXAMPLES:
- "What is crude oil price?" → call with no params
- "Current WTI oil price" → call with no params
- "Crude oil futures today" → call with no params

Get current WTI crude oil futures price
- **get_energy_commodities_prices**: Essential for tracking the energy market.

USE WHEN:
- User asks about energy commodity prices
- User wants to see all energy commodities at once
- User needs to compare oil vs gas prices
- User asks "show me energy commodity prices"

EXAMPLES:
- "What are energy commodity prices?" → call with no params
- "Show me oil and gas prices" → call with no params
- "Energy market today" → call with no params

Get current prices for crude oil, Brent crude, and natural gas
- **get_gold_price**: Gold is the primary precious metal benchmark traded globally.

USE WHEN:
- User asks specifically about gold price
- User needs the gold benchmark price
- User wants to check precious metals pricing
- User asks "what is gold price"

EXAMPLES:
- "What is gold price?" → call with no params
- "Current gold futures price" → call with no params
- "Gold spot price today" → call with no params

Get current gold futures price
- **list_all_commodities**: USE WHEN:
- User wants to explore what commodities are available
- User needs to find commodity codes for querying prices
- User is exploring the API capabilities for the first time
- User asks what commodities are supported

CATEGORIES:
- Precious Metals: gold, silver, platinum, palladium (CME/NYMEX)
- Energy: crude_oil, brent_crude_oil, natural_gas (NYMEX/CME)
- Agriculture: wheat, corn, soybean, coffee, cocoa, sugar (CBOT/CME)
- Livestock: live_cattle, feeder_cattle, lean_hogs (CME)
- Industrial Metals: copper, aluminum (CME)

EXAMPLES:
- "What commodities are available?" → call with no params
- "Show me all commodity codes" → call with no params
- "List all commodity exchanges" → call with no params

List all 30+ available commodities with their codes and exchanges
- **get_natural_gas_price**: Natural gas is a key energy commodity for heating and electricity generation.

USE WHEN:
- User asks about natural gas prices
- User needs the natural gas benchmark
- User wants to check energy pricing
- User asks "what is natural gas price"

EXAMPLES:
- "What is natural gas price?" → call with no params
- "Current natural gas futures" → call with no params
- "Natural gas spot price today" → call with no params

Get current natural gas futures price
- **get_precious_metals_prices**: Perfect for tracking the precious metals market comprehensively.

USE WHEN:
- User asks about precious metals prices
- User wants to see all precious metals at once
- User needs to compare gold, silver, platinum, palladium
- User asks "show me precious metals prices"

EXAMPLES:
- "What are precious metals prices?" → call with no params
- "Show me gold, silver, platinum, palladium" → call with no params
- "Precious metals market today" → call with no params

Get current prices for gold, silver, platinum, and palladium
- **get_silver_price**: Silver is the second most traded precious metal after gold.

USE WHEN:
- User asks specifically about silver price
- User needs the silver benchmark price
- User wants to compare gold vs silver ratio
- User asks "what is silver price"

EXAMPLES:
- "What is silver price?" → call with no params
- "Current silver futures price" → call with no params
- "Silver spot price today" → call with no params

Get current silver futures price
- **get_wheat_price**: Wheat is a key agricultural commodity for global food security.

USE WHEN:
- User asks about wheat prices
- User needs the grain benchmark
- User wants to track agricultural commodities
- User asks "what is wheat price"

EXAMPLES:
- "What is wheat price?" → call with no params
- "Current wheat futures price" → call with no params
- "Wheat spot price today" → call with no params

Get current wheat futures price


## Installation & Usage

To install and use the **Commodities** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/commodities](https://vinkius.com/mcp/commodities)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
