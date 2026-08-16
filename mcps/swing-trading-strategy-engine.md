# Swing Trading Strategy Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/swing-trading-strategy-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A deterministic multi-timeframe engine for identifying high-probability swing trading pullbacks.

## Description
This MCP server provides a deterministic multi-timeframe analysis engine designed for swing traders. It identifies high-probability pullbacks by ensuring the macro trend is bullish via a 10-week Moving Average, then triggers entries when daily prices retreat to the 20-day Moving Average while RSI is in a 'resting' state (40-50). The engine includes built-in risk management with automated stop-loss and take-profit calculations, and a specialized `filter_gap_risk` tool to avoid entering trades immediately before earnings announcements. Use `calculate_signals` to generate actionable trade entries and `get_swing_metrics` to evaluate the strength of a setup.


## Available Tools (3)
- **calculate_signals**: Analyzes historical price data to generate a series of Buy, Sell, or Hold signals based on multi-timeframe logic
- **filter_gap_risk**: Evaluates if a specific date is safe to enter a trade based on upcoming corporate news
- **get_swing_metrics**: Provides a detailed breakdown of the strength and characteristics of a specific trading setup


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Swing Trading Strategy Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate trading signals for these closing prices: [150, 152, 148, 147, 149, 155, 158] with a 10-week MA, 20-day MA, 50-day MA, and 14-period RSI."

**🤖 AI Agent:**
> BUY at 149.00, Stop-Loss: 141.55, Take-Profit: 163.90, Swing Quality: 0.85

---

**👤 You:**
> "Evaluate the quality of this setup with price 150, 20-day MA 148, 50-day MA 140, and RSI 45."

**🤖 AI Agent:**
> qualityScore: 0.88, proximityScore: 0.92, momentumScore: 0.75

---

**👤 You:**
> "Is it safe to enter a trade on 2024-05-15 if earnings are scheduled for 2024-05-18?"

**🤖 AI Agent:**
> isSafe: false, daysUntilEarnings: 3


## ❓ FAQ

**Q: How does the engine determine a valid entry?**
A valid entry requires the price to be above the 10-week Moving Average, a pullback to the 20-day Moving Average, and an RSI between 40 and 50, provided no earnings are imminent.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, you can connect this engine to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.

**Q: What is the purpose of the `filter_gap_risk` tool?**
The `filter_gap_risk` tool checks if an upcoming corporate earnings announcement occurs within 5 days of your target entry date to prevent unexpected price gaps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/swing-trading-strategy-engine](https://vinkius.com/mcp/swing-trading-strategy-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Swing Trading Strategy Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `swing-trading-strategy-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Swing Trading Strategy Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "swing-trading-strategy-engine": {
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
