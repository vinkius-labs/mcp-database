# Bollinger Band Squeeze Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/bollinger-band-squeeze-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify market volatility contractions and breakout signals using Bollinger Bands and Keltner Channels.

## Description
This MCP server provides a deterministic technical analysis engine to detect market volatility squeezes. By monitoring when Bollinger Bands move inside Keltner Channels, the engine identifies periods of low volatility. It then triggers precise BUY or SELL signals when price breaks out of these bands, confirmed by volume spikes. Use `analyze_squeeze_signals` to evaluate historical data, `get_current_volatility_metrics` for risk assessment, and `validate_breakout_conditions` to verify signal validity.


## Available Tools (3)
- **analyze_squeeze_signals**: Evaluates historical price, volume, and volatility data to identify squeeze periods and subsequent breakout signals
- **validate_breakout_conditions**: A specialized validator to check if a specific price action meets the strict criteria for a squeeze breakout
- **get_current_volatility_metrics**: Calculates specific volatility indicators (ATR and BB width) for a given set of prices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bollinger Band Squeeze Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these closing prices and volumes for squeeze signals: [150, 151, 150, 149, 150, 152, 155, 160] and [1000, 1100, 1050, 1000, 1050, 1200, 2500, 2800]."

**🤖 AI Agent:**
> A BUY signal was detected at the final bar. The price broke above the upper Bollinger Band after a 5-bar squeeze, with volume confirmed at 2800 (exceeding the 1.5x average threshold).

---

**👤 You:**
> "What are the current volatility metrics for these prices: [100, 102, 101, 103, 102]?"

**🤖 AI Agent:**
> The current volatility metrics show an ATR of 1.2, a BB width of 4.5, and a middle band of 101.6.

---

**👤 You:**
> "Is this breakout valid? Squeeze length: 6, isSqueezed: true, currentVolume: 5000, avgVolume: 2000."

**🤖 AI Agent:**
> Yes, the breakout is valid because the squeeze lasted more than 5 bars and the volume is significantly higher than the average.


## ❓ FAQ

**Q: What is a volatility squeeze?**
A squeeze occurs when Bollinger Bands contract inside the Keltner Channels, indicating a period of extremely low volatility that often precedes a significant price breakout.

**Q: How are breakout signals confirmed?**
Breakouts are confirmed when the price closes outside the Bollinger Bands after a squeeze of at least 5 bars, accompanied by volume that is at least 1.5 times the 20-day average.

**Q: Can I customize the volatility parameters?**
Yes, you can adjust the Bollinger Band period, standard deviation, Keltner Channel period, and ATR multiplier using the `analyze_squeeze_signals` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/bollinger-band-squeeze-strategy](https://vinkius.com/ai-agent-connect/bollinger-band-squeeze-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bollinger Band Squeeze Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bollinger-band-squeeze-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bollinger Band Squeeze Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bollinger-band-squeeze-strategy": {
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
