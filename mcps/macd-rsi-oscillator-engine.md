# MACD & RSI Oscillator Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/macd-rsi-oscillator-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Calculate exact MACD and Relative Strength Index (RSI) technical indicators local for quantitative analysis.

## Description
The Relative Strength Index (RSI) and Moving Average Convergence Divergence (MACD) are complex oscillators that require multiple passes of exponential averages. Asking an LLM to compute RSI over 100 days is a guaranteed failure. This engine integrates institutional-grade TS indicator math into the Vinkius edge runtime, providing autonomous trading and analysis agents with perfect signals.


## Available Tools (1)
- **calculate_macd_rsi**: Provide data array and configuration parameters.

Calculates MACD or RSI technical oscillators from a price array


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MACD & RSI Oscillator Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the 14-period RSI for this daily stock price array. Tell me if the final day is below 30 (Oversold)."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "Run the MACD calculator. Check the last 3 days and tell me if the MACD line has crossed above the Signal line (bullish)."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "I see the price making a new high here. Calculate the RSI and tell me if the RSI is making a lower high (bearish divergence)."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.


## ❓ FAQ

**Q: What does RSI indicate?**
RSI ranges from 0 to 100. Traditionally, a value above 70 indicates an asset is Overbought, and below 30 indicates it is Oversold.

**Q: What are the MACD parameters?**
It uses the standard 12-period Fast EMA, 26-period Slow EMA, and 9-period Signal line to generate exact histograms.

**Q: Is this for crypto or stocks?**
Both. Technical oscillators are mathematically agnostic and work on any sequential numeric data array, regardless of the asset class.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/macd-rsi-oscillator-engine](https://vinkius.com/mcp/macd-rsi-oscillator-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MACD & RSI Oscillator Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `macd-rsi-oscillator-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MACD & RSI Oscillator Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "macd-rsi-oscillator-engine": {
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
