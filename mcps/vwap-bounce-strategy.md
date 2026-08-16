# VWAP Bounce Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vwap-bounce-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify high-probability intraday mean-reversion signals using VWAP interaction and trend filters.

## Description
This MCP server provides deterministic intraday trading signals by analyzing price interactions with the Volume Weighted Average Price (VWAP). It identifies high-probability BUY and SELL opportunities when price pulls back to the VWAP during established trends. The server uses `analyze_vwap_signals` to evaluate OHLC and volume data, ensuring signals meet strict structural requirements like higher highs or lower lows. You can also use `get_vwap_metrics` to monitor the current VWAP slope and distance, or `validate_trend_structure` to confirm market regime integrity.


## Available Tools (3)
- **analyze_vwap_signals**: Evaluates intraday price and volume data to identify specific BUY, SELL, or HOLD signals based on VWAP interaction and trend filters
- **get_vwap_metrics**: Provides a snapshot of the current state of the VWAP level, including its trend, strength, and current price deviation
- **validate_trend_structure**: Determines if the current price action satisfies the structural requirements (Higher Highs/Lower Lows) necessary to qualify for a signal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VWAP Bounce Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the recent intraday data for a BUY signal."

**🤖 AI Agent:**
> BUY signal detected at 150.25. Entry: 150.25, Stop-Loss: 149.85, Take-Profit: 151.05.

---

**👤 You:**
> "What is the current VWAP slope and distance?"

**🤖 AI Agent:**
> The current VWAP slope is 0.02 and the price is 0.45% above the VWAP.

---

**👤 You:**
> "Is the current trend structure valid for a SELL signal?"

**🤖 AI Agent:**
> No, the current price action has not established a lower low to qualify for a SELL signal.


## ❓ FAQ

**Q: What kind of signals does this server provide?**
The server provides BUY, SELL, or HOLD signals based on how price interacts with the VWAP during an established trend.

**Q: How are stop-loss levels determined?**
Stop-loss levels are calculated using 0.5x the Average True Range (ATR) relative to the VWAP.

**Q: Can I check the current trend strength?**
Yes, you can use `get_vwap_metrics` to retrieve the current VWAP slope and distance from the price.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vwap-bounce-strategy](https://vinkius.com/mcp/vwap-bounce-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VWAP Bounce Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vwap-bounce-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VWAP Bounce Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vwap-bounce-strategy": {
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
