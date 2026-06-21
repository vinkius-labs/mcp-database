# Commodity Price Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/commodity-price-converter)
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


## ❓ FAQ

**Q: How can I convert prices between different units?**
Use the `convert_price_units` tool. Provide the initial price, its unit (e.g., saca), its currency, and the current USD/BRL exchange rate to get a complete list of all supported units.

**Q: Can I calculate production costs per hectare?**
Yes. The `calculate_cost_per_hectare` tool calculates the cost in BRL/ha by processing the commodity price and the land's yield per hectare.

**Q: Does it provide historical data?**
Yes, the `get_historical_market_trends` tool allows you to query minimum, maximum, and average prices for specific months and years stored in our dataset.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/commodity-price-converter](https://vinkius.com/mcp/commodity-price-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Commodity Price Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `commodity-price-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Commodity Price Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "commodity-price-converter": {
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
