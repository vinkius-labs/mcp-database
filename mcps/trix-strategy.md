# TRIX Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/trix-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic momentum trading strategy using Triple EMA and signal line analysis.

## Description
This MCP server provides a deterministic momentum trading strategy based on the Triple Exponential Moving Average (TRIX). It allows AI agents to calculate advanced momentum indicators and generate precise trading signals. Using `calculate_trix_metrics`, agents can derive the TRIX oscillator, signal line, and momentum acceleration. The `generate_trading_signals` tool identifies BUY and SELL entries by analyzing TRIX crossings and histogram trends, while `analyze_signal_performance` evaluates the historical accuracy of these signals against price data.


## Available Tools (3)
- **analyze_signal_performance**: Evaluates the historical accuracy and quality of the generated signals
- **calculate_trix_metrics**: Calculates the raw TRIX oscillator, signal line, and secondary momentum indicators
- **generate_trading_signals**: Analyzes TRIX metrics to identify specific BUY, SELL, or HOLD entry and exit signals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TRIX Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the TRIX metrics for these closing prices: [150.2, 152.5, 151.8, 153.0, 154.5]"

**🤖 AI Agent:**
> The TRIX oscillator value is 0.45, the signal line is 0.32, and the current slope is 0.13.

---

**👤 You:**
> "Generate trading signals using these TRIX metrics and ATR values."

**🤖 AI Agent:**
> A BUY signal was generated at price 154.5 with a stop-loss at 152.0 and a take-profit at 158.0.

---

**👤 You:**
> "What was the performance of the signals given these prices?"

**🤖 AI Agent:**
> The strategy achieved a win rate of 65% with an average profit per trade of 2.4% and a maximum drawdown of 5.2%.


## ❓ FAQ

**Q: What is the TRIX strategy?**
It is a momentum strategy that uses a Triple Exponential Moving Average to smooth price data and identify trend reversals through signal line crossings.

**Q: How are BUY signals generated?**
A BUY signal is triggered when TRIX crosses above the signal line while below zero, provided the TRIX histogram has been rising for at least two bars.

**Q: Can I evaluate my strategy's success?**
Yes, you can use the `analyze_signal_performance` tool to calculate win rates, average profit, and maximum drawdown based on historical price data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/trix-strategy](https://vinkius.com/ai-agent-connect/trix-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TRIX Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `trix-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TRIX Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "trix-strategy": {
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
