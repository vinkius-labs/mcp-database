# Position Trading Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/position-trading-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A deterministic trading system combining technical momentum, fundamental value, and sector strength.

## Description
This MCP server provides a deterministic position trading strategy that synthesizes technical momentum, fundamental valuation, and sector strength. It uses `get_trading_signals` to evaluate technical trends like Golden Crosses and fundamental metrics like P/E ratios and earnings growth. It also provides `calculate_position_metrics` to determine precise stop-loss, take-profit, and position quality scores, and `validate_market_regime` to ensure the macro environment is risk-on based on SPY trends.


## Available Tools (3)
- **validate_market_regime**: Determines if the macro environment permits active trading
- **calculate_position_metrics**: Determines risk parameters and quality score for a trade
- **get_trading_signals**: Evaluates technical and fundamental criteria to generate a signal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Position Trading Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Should I buy this stock based on its current technical and fundamental data?"

**🤖 AI Agent:**
> The current signal is BUY. The price is above the 200-day MA, a Golden Cross has formed, and the P/E ratio is attractive relative to the sector.

---

**👤 You:**
> "What is the risk management plan for my current position?"

**🤖 AI Agent:**
> Your stop-loss is set at $145.00 and your trailing take-profit is set at $172.50 based on the recent peak.

---

**👤 You:**
> "Is the current market environment suitable for trading?"

**🤖 AI Agent:**
> Yes, the market is currently in a risk-on regime as the SPY is trading above its 200-day Moving Average.


## ❓ FAQ

**Q: What criteria trigger a BUY signal?**
A BUY signal is triggered when the market is in a risk-on regime, the price is above the 200-day MA, a Golden Cross occurs, the P/E is below the sector average, and earnings growth exceeds 15%.

**Q: How is the stop-loss calculated?**
The stop-loss is determined by the higher value between the 200-day Moving Average and a 15% drop from the entry price.

**Q: How does the system handle market volatility?**
The system uses a trailing stop-loss (take-profit) that triggers if the price drops 10% from its peak, protecting gains during volatile periods.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/position-trading-strategy](https://vinkius.com/mcp/position-trading-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Position Trading Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `position-trading-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Position Trading Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "position-trading-strategy": {
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
