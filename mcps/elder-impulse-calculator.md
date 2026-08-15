# Elder Impulse Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/elder-impulse-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic technical analysis for Elder Impulse signals.

## Description
This MCP server provides deterministic technical analysis tools based on the Elder Impulse System. It identifies market regimes by analyzing the convergence of EMA trends and MACD histogram momentum. Use `calculate_impulse_signals` to generate the full sequence of GREEN, RED, and BLUE signals. Use `get_signal_summary` to aggregate signal frequencies and `evaluate_trade_triggers` to pinpoint specific buy and sell entry indices based on strict momentum rules.


## Available Tools (3)
- **calculate_impulse_signals**: Generates the core impulse signal sequence for a provided price series and momentum data
- **evaluate_trade_triggers**: Identifies specific entry points based on strict impulse rules
- **get_signal_summary**: Provides a high-level overview of signal frequency and regime changes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Elder Impulse Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the impulse signals for these close prices: [150, 152, 151, 153, 155] and MACD histogram: [0.1, 0.2, 0.1, 0.3, 0.4]."

**🤖 AI Agent:**
> The signals generated are: [BLUE, GREEN, BLUE, GREEN, GREEN].

---

**👤 You:**
> "Summarize these signals: [{'color': 'GREEN', 'isChange': true, 'persistence': 1}, {'color': 'GREEN', 'isChange': false, 'persistence': 2}, {'color': 'RED', 'isChange': true, 'persistence': 1}]."

**🤖 AI Agent:**
> Total Green: 2, Total Red: 1, Total Blue: 0, Total Changes: 1.

---

**👤 You:**
> "Find the buy and sell entries for these signals: [{'color': 'GREEN', 'isChange': true, 'persistence': 1}, {'color': 'RED', 'isChange': true, 'persistence': 1}]."

**🤖 AI Agent:**
> Buy entries at index: 0. Sell entries at index: 1.


## ❓ FAQ

**Q: What are the different impulse signals?**
The system produces GREEN (bullish), RED (bearish), and BLUE (neutral) signals based on whether the EMA and MACD histogram are aligned or conflicting.

**Q: How do I identify trade entries?**
You can use `evaluate_trade_triggers` to find specific bar indices where a GREEN signal indicates a buy entry and a RED signal indicates a sell entry.

**Q: Can I customize the EMA period?**
Yes, the `calculate_impulse_signals` tool allows you to specify an `emaPeriod`, which defaults to 13.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/elder-impulse-calculator](https://vinkius.com/mcp/elder-impulse-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Elder Impulse Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `elder-impulse-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Elder Impulse Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "elder-impulse-calculator": {
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
