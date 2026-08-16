# MACD Crossover Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/macd-crossover-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic MACD crossover trend-following strategy with momentum confirmation.

## Description
This MCP server provides advanced technical analysis tools for trend-following using the Moving Average Convergence Divergence (MACD) indicator. It identifies early trend reversals by detecting crossovers when the MACD line is below zero for BUY signals and above zero for SELL signals. The strategy includes momentum confirmation via histogram analysis and provides precise risk management parameters including entry prices, stop-loss levels based on ATR, and 3:1 reward-to-risk take-profit targets. Use `calculate_macd_signals` to generate full signal series, `evaluate_signal_quality` to assess trend strength, and `get_volatility_metrics` for risk parameters.


## Available Tools (3)
- **calculate_macd_signals**: Generates a complete series of trading signals based on historical price data
- **get_volatility_metrics**: Computes volatility indicators needed for risk management
- **evaluate_signal_quality**: Provides a detailed breakdown of the strength and reliability of a specific signal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MACD Crossover Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a series of trading signals for these closing prices: [150.2, 151.5, 152.0, 151.8, 153.5, 155.0, 154.5]."

**🤖 AI Agent:**
> The analysis shows a BUY signal at the 5th bar with an entry price of 153.5, a stop-loss of 151.8, and a take-profit of 158.6.

---

**👤 You:**
> "What is the current signal quality for a MACD line of 0.5, previous MACD of 0.2, and a histogram of 0.3 at a price of 100?"

**🤖 AI Agent:**
> The signal quality score is 0.85, indicating strong slope strength and low divergence.

---

**👤 You:**
> "Calculate the volatility metrics for these prices: [10, 12, 11, 13, 15, 14, 16]."

**🤖 AI Agent:**
> The ATR is 1.45, with a recent swing high of 16 and a recent swing low of 10.


## ❓ FAQ

**Q: What triggers a BUY signal?**
A BUY signal is triggered when the MACD line crosses above the Signal line while the MACD is below zero, provided the histogram is increasing.

**Q: How is the stop-loss calculated?**
The stop-loss is determined by taking the greater of the recent price swing or twice the Average True Range (ATR).

**Q: Can I assess the strength of a signal?**
Yes, you can use the `evaluate_signal_quality` tool to get a detailed breakdown of slope strength and divergence scores.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/macd-crossover-strategy](https://vinkius.com/mcp/macd-crossover-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MACD Crossover Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `macd-crossover-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MACD Crossover Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "macd-crossover-strategy": {
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
