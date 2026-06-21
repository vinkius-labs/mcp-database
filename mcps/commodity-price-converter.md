# Commodity Price Converter MCP Server

Convert commodity prices across units and currencies instantly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/commodity-price-converter)

## Overview
**Category:** finance
**Tools Count:** 3

## Description
This MCP server provides specialized tools for agricultural financial analysis. It allows AI agents to perform complex mass-equivalence conversions between units like saca, arroba, bushel, and tonne, while handling currency shifts between BRL and USD using real-time exchange rates. With `convert_price_units`, you can expand a single price point into a full market overview. Use `calculate_cost_per_hectare` to determine production costs based on land productivity, and `get_historical_market_trends` to analyze seasonal price fluctuations from historical datasets.


## Available Tools
- **calculate_cost_per_hectare**: You need the current market price, its unit type, the yield (productivity) of the land, and the unit of that yield.

Calculates the total production cost in BRL per hectare based on commodity price and land productivity
- **convert_price_units**: It will return a full list of converted prices.

Converts a commodity price from one unit and currency to all other supported units and currencies
- **get_historical_market_trends**: Retrieves the recorded historical price extremes and averages for a specific month and year


## Installation & Usage

To install and use the **Commodity Price Converter** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/commodity-price-converter](https://vinkius.com/mcp/commodity-price-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
