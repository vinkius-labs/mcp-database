# Elder Impulse Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/elder-impulse-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic trading signals using EMA and MACD momentum.

## Description
This MCP server implements the Elder Impulse System, a trend-following methodology that synchronizes Exponential Moving Average (EMA) trend direction with MACD histogram momentum. It generates color-coded signals: GREEN for bullish impulse, RED for bearish impulse, and BLUE for neutral transitions. Use `calculate_impulse_signals` to determine the current market color, `generate_trade_signals` to identify actionable entries with calculated stop-loss and take-profit levels, and `analyze_trend_strength` to evaluate trend duration and quality. This tool connects your AI agent to precise, deterministic momentum analysis.


## Available Tools (3)
- **analyze_trend_strength**: Summarizes the current market trend based on the most recent impulse signals
- **calculate_impulse_signals**: Generates core color-coded impulse signals (Green, Red, Blue) for a price series
- **generate_trade_signals**: Evaluates impulse signals to generate actionable BUY/SELL trade entries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Elder Impulse Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the impulse signals for these closing prices: [150.2, 151.5, 152.1, 151.8] and MACD histogram: [0.5, 0.8, 1.2, 0.9]."

**🤖 AI Agent:**
> The impulse signals for the provided data are: [{"color": "GREEN", "emaSlope": 0.4, "histogramSlope": 0.3, "persistence": 1}, {"color": "GREEN", "emaSlope": 0.5, "histogramSlope": 0.4, "persistence": 2}, {"color": "GREEN", "emaSlope": 0.3, "histogramSlope": -0.3, "persistence": 1}, {"color": "BLUE", "emaSlope": -0.1, "histogramSlope": -0.3, "persistence": 1}]

---

**👤 You:**
> "Generate trade signals using the following impulse data: [{"color": "GREEN", "emaSlope": 0.5, "histogramSlope": 0.5, "persistence": 2}] with close prices [100, 102], ATR [1.5], and a reward ratio of 3."

**🤖 AI Agent:**
> {"type": "BUY", "entryPrice": 102.0, "stopLoss": 99.0, "takeProfit": 108.0, "signalQuality": 1.0}

---

**👤 You:**
> "What is the current trend strength for this impulse data: [{"color": "RED", "emaSlope": -0.5, "histogramSlope": -0.5, "persistence": 3}]?"

**🤖 AI Agent:**
> The current trend is RED with a duration of 3 bars and an average quality of -0.5.


## ❓ FAQ

**Q: What are the different signal colors?**
GREEN indicates bullish momentum (rising EMA and MACD), RED indicates bearish momentum (falling EMA and MACD), and BLUE indicates a neutral transition phase.

**Q: How is the stop-loss calculated?**
The stop-loss is determined using either a recent price swing or a multiple of the Average True Range (ATR) via the `generate_trade_signals` tool.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, and any other MCP-compatible client through Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/elder-impulse-strategy](https://vinkius.com/ai-agent-connect/elder-impulse-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Elder Impulse Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `elder-impulse-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Elder Impulse Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "elder-impulse-strategy": {
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
