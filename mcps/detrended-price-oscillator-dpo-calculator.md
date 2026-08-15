# Detrended Price Oscillator (DPO) Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/detrended-price-oscillator-dpo-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify price cycles and momentum oscillations by removing trends from price series.

## Description
This MCP server provides a deterministic engine for calculating the Detrended Price Oscillator (DPO). It removes trend components from price data to reveal underlying cycles. Use `calculate_dpo_series` to generate raw oscillator values, `analyze_dpo_signals` to detect zero-line crossings and volatility-based momentum extremes, and `identify_price_cycles` to measure the duration between price peaks and troughs.


## Available Tools (3)
- **analyze_dpo_signals**: Identifies zero-line crossings and momentum extremes within the DPO data
- **calculate_dpo_series**: Computes the raw Detrended Price Oscillator values for a given series of prices
- **identify_price_cycles**: Detects dominant price cycles by measuring distance between local peaks and troughs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Detrended Price Oscillator (DPO) Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the DPO series for these closing prices: [150.2, 152.5, 151.0, 153.4, 155.0, 154.2, 156.8] with a period of 5."

**🤖 AI Agent:**
> The calculated DPO values for the provided series are [1.2, 0.8, -0.5, 2.1, 1.4].

---

**👤 You:**
> "Analyze these DPO values for signals: [0.5, 1.2, -0.3, -1.5, 0.2]."

**🤖 AI Agent:**
> The analysis detected a zero-line crossing at the third value and an extreme momentum signal at the fourth value.

---

**👤 You:**
> "Identify the price cycles in this DPO data: [2.0, 1.5, 0.0, -1.5, -2.0, -1.0, 0.5, 2.5]."

**🤖 AI Agent:**
> The detected cycle length between the primary peak and trough is 4 bars.


## ❓ FAQ

**Q: What is the purpose of the DPO?**
The Detrended Price Oscillator (DPO) is used to identify underlying price cycles by removing the trend component from the price series.

**Q: How are overbought and oversold zones determined?**
Extremes are identified when DPO values exceed the moving standard deviation calculated over a specified lookback period.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, this MCP server can be connected to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/detrended-price-oscillator-dpo-calculator](https://vinkius.com/mcp/detrended-price-oscillator-dpo-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Detrended Price Oscillator (DPO) Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `detrended-price-oscillator-dpo-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Detrended Price Oscillator (DPO) Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "detrended-price-oscillator-dpo-calculator": {
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
