# Variable Index Dynamic Average (VIDYA) Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/variable-index-dynamic-average-vidya-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Adaptive technical indicator engine that scales smoothing based on market volatility.

## Description
This MCP server provides advanced adaptive smoothing capabilities using the Variable Index Dynamic Average (VIDYA). By utilizing the Chande Momentum Oscillator (CMO) as a volatility factor, the indicator automatically adjusts its responsiveness to price momentum. Use `calculate_vidya_series` to generate full datasets including slopes and adaptive responses, `get_vidya_summary` for statistical snapshots of specific price ranges, or `detect_vidya_regime` to identify Bullish, Bearish, or Neutral market states.


## Available Tools (3)
- **get_vidya_summary**: Provides a high-level statistical snapshot of the VIDYA behavior over a specific range
- **calculate_vidya_series**: Computes the full series of VIDYA values, slopes, and adaptive responses for a given price dataset
- **detect_vidya_regime**: Identifies the current market regime based on the relationship between price and the VIDYA line


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Variable Index Dynamic Average (VIDYA) Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the VIDYA series for these closing prices: [150.2, 152.5, 151.0, 153.4, 155.0]"

**🤖 AI Agent:**
> [{"index": 0, "vidya": 150.2, "slope": 0, "volatilityResponse": 0}, {"index": 1, "vidya": 151.1, "slope": 0.9, "volatilityResponse": 0.4}, {"index": 2, "vidya": 151.05, "slope": -0.05, "volatilityResponse": 0.2}, {"index": 3, "vidya": 152.1, "slope": 1.05, "volatilityResponse": 0.5}, {"index": 4, "vidya": 153.6, "slope": 1.5, "volatilityResponse": 0.6}]

---

**👤 You:**
> "What is the current market regime for these prices: [100, 102, 104, 103, 105]?"

**🤖 AI Agent:**
> The current regime is a Bullish Trend with a strength of 0.85, as the price is above the VIDYA line and the slope is positive.

---

**👤 You:**
> "Give me a summary of the VIDYA behavior between index 10 and 20 for this price series."

**🤖 AI Agent:**
> In the requested range, the average VIDYA was 450.25, with a maximum slope of 1.2 and a stable volatility trend.


## ❓ FAQ

**Q: What makes VIDYA different from a standard EMA?**
Unlike a standard EMA which uses a constant smoothing factor, VIDYA scales its responsiveness using the Chande Momentum Oscillator (CMO) to adapt to market volatility.

**Q: How can I identify the current market trend?**
You can use the `detect_vidya_regime` tool to identify if the market is in a Bullish Trend, Bearish Trend, or Sideways/Neutral state.

**Q: Can I customize the smoothing sensitivity?**
Yes, you can adjust the `cmoPeriod` for momentum lookback and the `emaPeriod` for the base smoothing factor via the available tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/variable-index-dynamic-average-vidya-calculator](https://vinkius.com/mcp/variable-index-dynamic-average-vidya-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Variable Index Dynamic Average (VIDYA) Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `variable-index-dynamic-average-vidya-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Variable Index Dynamic Average (VIDYA) Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "variable-index-dynamic-average-vidya-calculator": {
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
