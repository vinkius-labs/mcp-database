# Price Forecast Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/price-forecast-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Generate energy price trajectories, confidence intervals, and market scenario probabilities.

## Description
This MCP server provides advanced analytical tools for energy market forecasting. It allows AI agents to calculate expected price trajectories using `get_price_trajectory`, assess market uncertainty with `get_price_confidence_intervals`, and determine the likelihood of Bullish or Bearish outcomes via `get_scenario_probabilities`. Additionally, users can identify market mispricing by using `analyze_curve_vs_history` to compare forward curves against historical data.


## Available Tools (4)
- **get_scenario_probabilities**: Determine the likelihood of different market directions (Bullish, Bearish, Neutral) based on supply/demand and macro inputs
- **analyze_curve_vs_history**: Compare current market forward curves against historical price patterns to identify market mispricing or extreme sentiment
- **get_price_confidence_intervals**: Understand the range of potential price outcomes and the level of uncertainty in the forecast
- **get_price_trajectory**: Retrieve the central predicted price path for a specific commodity over a given timeframe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Price Forecast Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected price path for crude oil over the next 12 months?"

**🤖 AI Agent:**
> The expected price for crude oil is projected to follow a steady upward trend, reaching approximately $85 per barrel by month 12.

---

**👤 You:**
> "What is the 95% confidence interval for natural gas prices for a 6-month horizon?"

**🤖 AI Agent:**
> For a 6-month horizon, the 95% confidence interval for natural gas ranges from $2.50 to $4.10 per MMBtu.

---

**👤 You:**
> "How likely is a bearish scenario if there is a significant supply increase?"

**🤖 AI Agent:**
> A significant supply increase shifts the market probability toward a Bearish case, with a calculated likelihood of 65%.


## ❓ FAQ

**Q: What commodities can I forecast?**
The model supports primary energy benchmarks including crude oil, natural gas, and regional commodities like European natural gas or diesel.

**Q: How are the price trajectories calculated?**
Trajectories are calculated by integrating historical prices, forward curves, and supply/demand fundamentals, while accounting for seasonality and mean reversion.

**Q: Can I model specific supply shocks?**
Yes, you can use `get_scenario_probabilities` with the `supplyShockMagnitude` parameter to see how unexpected supply changes affect market probabilities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/price-forecast-model](https://vinkius.com/en/ai-agent-connect/price-forecast-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Price Forecast Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `price-forecast-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Price Forecast Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "price-forecast-model": {
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
