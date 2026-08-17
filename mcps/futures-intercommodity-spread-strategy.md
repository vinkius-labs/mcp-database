# Futures Intercommodity Spread Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/futures-intercommodity-spread-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic ratio-based trading signals for commodity spreads.

## Description
This MCP server provides deterministic trading signals for executing ratio-based spreads between different commodity futures. By analyzing the relationship between two assets, it calculates the spread ratio, z-score, and mean reversion characteristics. It uses `get_daily_spread_signals` to identify BUY and SELL opportunities based on statistical deviations and fundamental drivers, while `get_spread_statistics` provides historical context like min/max ratios and half-life. The strategy includes built-in liquidity and correlation filters to ensure high-quality trade execution.


## Available Tools (2)
- **get_daily_spread_signals**: 
- **get_spread_statistics**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Futures Intercommodity Spread Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the daily spread signals for Gold and Silver with current prices of 2000 and 25 respectively, open interest of 15000 for both, a correlation of 0.8, and a bullish macro driver."

**🤖 AI Agent:**
> The spread ratio is 80.0. With a z-score of -2.5 and a bullish driver, the signal is BUY (Long Gold, Short Silver).

---

**👤 You:**
> "Get the historical statistics for a Copper and Gold spread using these price series: [4.0, 4.1, 3.9] and [1800, 1850, 1820]."

**🤖 AI Agent:**
> The historical min ratio is 0.0021, the max ratio is 0.0023, and the mean reversion half-life is 12.5 days.

---

**👤 You:**
> "Check the spread signal for Crude Oil and Natural Gas where correlation is 0.4."

**🤖 AI Agent:**
> NO SIGNAL. The correlation coefficient is below the required 0.6 threshold.


## ❓ FAQ

**Q: What kind of commodity pairs can I analyze?**
You can analyze any pair of highly correlated commodity futures, such as Gold/Silver or Copper/Gold, provided they meet the liquidity and correlation requirements defined in the tool.

**Q: How are trading signals generated?**
Signals are generated using `get_daily_spread_signals` when the z-score indicates a significant deviation and the fundamental driver supports the direction.

**Q: What filters are applied to the signals?**
The strategy filters for liquidity (Open Interest > 10,000), correlation (coefficient > 0.6), and significant spread movement (> 10% change in 60 days).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/futures-intercommodity-spread-strategy](https://vinkius.com/ai-agent-connect/futures-intercommodity-spread-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Futures Intercommodity Spread Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `futures-intercommodity-spread-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Futures Intercommodity Spread Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "futures-intercommodity-spread-strategy": {
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
