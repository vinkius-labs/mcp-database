# Connors RSI Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/connors-rsi-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Connors RSI and identify mean-reversion trading signals.

## Description
This MCP server provides tools to calculate the Connors RSI, a momentum oscillator used to identify extreme overbought or oversold conditions. Use `calculate_connors_rsi` to compute the indicator from price series, `generate_reversion_signals` to detect BUY or SELL opportunities, and `get_indicator_summary` for a natural language overview of market intensity.


## Available Tools (3)
- **calculate_connors_rsi**: Optional parameters for RSI, streak, and rank periods can be provided.

Calculates the current Connors RSI value for a given price series
- **generate_reversion_signals**: Analyzes a Connors RSI value to determine trading signals
- **get_indicator_summary**: Provides a high-level overview of the current market state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Connors RSI Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Connors RSI for these closing prices: [150.2, 152.5, 151.0, 148.5, 147.0, 146.5, 145.0, 144.0, 143.5, 142.0]"

**🤖 AI Agent:**
> The calculated Connors RSI value is 8.42.

---

**👤 You:**
> "Is a Connors RSI of 95 overbought?"

**🤖 AI Agent:**
> Yes, a value of 95 is considered overbought and triggers a SELL signal.

---

**👤 You:**
> "Give me a summary for a Connors RSI of 5."

**🤖 AI Agent:**
> The asset is currently oversold with high intensity.


## ❓ FAQ

**Q: What is Connors RSI?**
Connors RSI is a three-part momentum oscillator that combines RSI, price streaks, and the percentile rank of the rate of change to find extreme market conditions.

**Q: How do I get a BUY signal?**
A BUY signal is generated when the Connors RSI value falls below the oversold threshold, typically 10.

**Q: Can I customize the RSI periods?**
Yes, you can specify custom values for the RSI period, streak period, and rank period using the `calculate_connors_rsi` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/connors-rsi-calculator](https://vinkius.com/mcp/connors-rsi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Connors RSI Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `connors-rsi-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Connors RSI Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "connors-rsi-calculator": {
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
