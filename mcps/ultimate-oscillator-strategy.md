# Ultimate Oscillator Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ultimate-oscillator-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic Larry Williams Ultimate Oscillator strategy for high-probability signals.

## Description
This MCP server provides a deterministic implementation of the Larry Williams Ultimate Oscillator (UO) strategy. It connects AI agents to advanced momentum analysis by identifying bullish and bearish divergences across multiple timeframes. Use `analyze_uo_strategy` to generate actionable buy and sell signals with precise entry prices, stop-loss levels, and take-profit targets. You can also use `calculate_uo_metrics` to inspect UO strength and alignment, or `detect_divergence` to isolate momentum shifts in price action.


## Available Tools (3)
- **analyze_uo_strategy**: Executes the full deterministic strategy logic to generate buy, sell, or hold signals
- **detect_divergence**: Identifies whether a bullish or bearish divergence exists between price and the UO
- **calculate_uo_metrics**: Provides raw diagnostic data regarding the current state of the oscillator


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ultimate Oscillator Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these prices for a buy signal: Highs [105, 104, 103], Lows [95, 94, 93], Closes [100, 98, 96]."

**🤖 AI Agent:**
> BUY signal detected. Entry Price: 96.0, Stop-Loss: 93.0, Take-Profit: 100.0.

---

**👤 You:**
> "Check the current UO metrics for these price arrays."

**🤖 AI Agent:**
> Current UO value is 25.0, indicating oversold conditions with a strength of 75.0 and bullish divergence detected.

---

**👤 You:**
> "Is there a bearish divergence in this data?"

**🤖 AI Agent:**
> No bearish divergence detected at this time.


## ❓ FAQ

**Q: How do I generate a trading signal?**
You can use the `analyze_uo_strategy` tool by providing arrays of high, low, and close prices. It will return a signal, entry price, stop-loss, and take-profit.

**Q: What is the difference between the tools?**
The `analyze_uo_strategy` tool provides full trade signals, while `calculate_uo_metrics` provides diagnostic data like strength and alignment, and `detect_divergence` focuses specifically on price-momentum divergences.

**Q: Does this support multi-timeframe analysis?**
Yes, the strategy uses three distinct periods (7, 14, and 28) to ensure momentum alignment before confirming a signal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ultimate-oscillator-strategy](https://vinkius.com/ai-agent-connect/ultimate-oscillator-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ultimate Oscillator Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ultimate-oscillator-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ultimate Oscillator Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ultimate-oscillator-strategy": {
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
