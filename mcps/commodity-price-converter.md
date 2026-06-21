# Commodity Price Converter MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/commodity-price-converter)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/commodity-price-converter-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/commodity-price-converter-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Convert commodity prices across units and currencies instantly.

## Description
This MCP server provides specialized tools for agricultural financial analysis. It allows AI agents to perform complex mass-equivalence conversions between units like saca, arroba, bushel, and tonne, while handling currency shifts between BRL and USD using real-time exchange rates. With `convert_price_units`, you can expand a single price point into a full market overview. Use `calculate_cost_per_hectare` to determine production costs based on land productivity, and `get_historical_market_trends` to analyze seasonal price fluctuations from historical datasets.


## Available Tools
- **calculate_cost_per_hectare**: You need the current market price, its unit type, the yield (productivity) of the land, and the unit of that yield.

Calculates the total production cost in BRL per hectare based on commodity price and land productivity
- **convert_price_units**: It will return a full list of converted prices.

Converts a commodity price from one unit and currency to all other supported units and currencies
- **get_historical_market_trends**: Retrieves the recorded historical price extremes and averages for a specific month and year


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Commodity Price Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert 150 BRL per saca to USD using an exchange rate of 5.0."

**🤖 AI Agent:**
> The `convert_price_units` tool has processed the request and returned all equivalent prices in BRL and USD for saca, arroba, bushel, and tonne.

---

**👤 You:**
> "What is the production cost if I produce 60 sacas per hectare at 150 BRL each?"

**🤖 AI Agent:**
> Using `calculate_cost_per_hectare`, the total production cost is calculated as 9000 BRL per hectare.

---

**👤 You:**
> "Show me the market trends for February 2023."

**🤖 AI Agent:**
> The `get_historical_market_trends` tool retrieved the following data: Min BRL 52, Max BRL 62, and Avg BRL 57.


## Installation & Usage

To install and use the **Commodity Price Converter** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/commodity-price-converter](https://vinkius.com/mcp/commodity-price-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
