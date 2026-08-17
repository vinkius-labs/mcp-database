# Futures Volume & Open Interest Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/futures-volume-open-interest-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze trend strength and direction using price, volume, and Open Interest momentum.

## Description
This MCP server provides a deterministic analysis engine for futures markets. It synthesizes price action, volume surges, and Open Interest (OI) momentum to distinguish between trend initiation and exhaustion. Use `analyze_market_momentum` to identify high-conviction BUY or SELL signals, `calculate_market_health_metrics` to detect institutional concentration and OI divergence, and `get_trend_summaries` for a high-level overview of market trends and volatility.


## Available Tools (3)
- **analyze_market_momentum**: 
- **calculate_market_health_metrics**: Quantifies market structural composition
- **get_trend_summaries**: Provides high-level trend and volatility overview


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Futures Volume & Open Interest Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the current market momentum for these series: price [50000, 50500, 51000], volume [1000, 1200, 2000], and OI [60000, 62000, 65000] with an avgVolume20 of 1000."

**🤖 AI Agent:**
> The market is in a Strong Uptrend. Signal: BUY. Confidence: High.

---

**👤 You:**
> "Check the market health metrics for the following data: OI [60000, 61000, 60500], price [50000, 51000, 52000], volume [1000, 1100, 1050], and topTraderOi 15000."

**🤖 AI Agent:**
> OI Concentration: 24.79%. Speculative Intensity: 0.017. OI Divergence: true.

---

**👤 You:**
> "Provide a trend summary for price [45000, 44000], volume [5000, 8000], and OI [70000, 75000]."

**🤖 AI Agent:**
> Price Trend: Down. OI Trend: Up. Volume Ratio: 1.6.


## ❓ FAQ

**Q: How are BUY and SELL signals generated?**
A BUY signal is generated during a Strong Uptrend when price is above the 20-day MA, OI is > 50,000, OI change is ≥ 1%, and volume is ≥ 1.5x the 20-day average. A SELL signal is generated during a Strong Downtrend under similar liquidity and momentum thresholds.

**Q: What is the purpose of the `calculate_market_health_metrics` tool?**
It quantifies market structure by calculating OI concentration of top traders, speculative intensity, and detecting OI divergence where price makes new highs without corresponding OI growth.

**Q: Can I use this with Claude Desktop or Cursor?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/futures-volume-open-interest-strategy](https://vinkius.com/ai-agent-connect/futures-volume-open-interest-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Futures Volume & Open Interest Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `futures-volume-open-interest-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Futures Volume & Open Interest Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "futures-volume-open-interest-strategy": {
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
