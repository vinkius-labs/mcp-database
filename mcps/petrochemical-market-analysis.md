# Petrochemical Market Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/petrochemical-market-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze global petrochemical supply-demand, operating rates, and price outlooks.

## Description
This MCP server provides deep analytical insights into the petrochemical industry. It allows AI agents to calculate the `analyze_supply_demand_balance` for specific products and regions, monitor industry efficiency via `calculate_operating_rates`, and predict market movements using `forecast_price_outlook`. Additionally, it can `map_trade_flows` to track how products move between geographic zones, helping to understand regional imbalances and global trade dynamics.


## Available Tools (4)
- **forecast_price_outlook**: Forecasts the expected price direction for a product
- **analyze_supply_demand_balance**: Analyzes the supply-demand balance for a specific petrochemical product in a region
- **calculate_operating_rates**: Calculates the current operating rate for a specific product in a region
- **map_trade_flows**: Maps the trade flows of a product between two regions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Petrochemical Market Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the supply-demand balance for Ethylene in North America for 2025?"

**🤖 AI Agent:**
> The supply-demand balance for Ethylene in North America for 2025 is a surplus of 1.2 million metric tons, with an operating rate of 92%.

---

**👤 You:**
> "Is the price outlook for Propylene in Europe bullish or bearish for the next 6 months?"

**🤖 AI Agent:**
> The price outlook for Propylene in Europe for the next 6 months is Bullish, with a confidence score of 0.85, primarily driven by New Capacity.

---

**👤 You:**
> "How efficient is the Benzene production in Asia-Pacific right now?"

**🤖 AI Agent:**
> The current operating rate for Benzene in Asia-Pacific is 88%, and the capacity trend is stable.


## ❓ FAQ

**Q: What products can I analyze?**
You can analyze primary building blocks like Ethylene and Propylene, as well as Aromatics like Benzene and Toluene.

**Q: How accurate are the price forecasts?**
Price directions are derived from real-time supply-demand balances and capacity trends, providing a confidence score for every forecast.

**Q: Can I track trade between specific regions?**
Yes, the `map_trade_flows` tool allows you to see how supply moves from an origin region to a destination region.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/petrochemical-market-analysis](https://vinkius.com/en/ai-agent-connect/petrochemical-market-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Petrochemical Market Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `petrochemical-market-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Petrochemical Market Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "petrochemical-market-analysis": {
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
