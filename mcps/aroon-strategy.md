# Aroon Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aroon-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic Aroon trend detection for precise BUY/SELL signals.

## Description
This MCP server provides deterministic trend detection using the Aroon indicator. It identifies strong market shifts by monitoring the timing of recent highs and lows. Use `calculate_aroon_metrics` to analyze trend strength and age, `generate_trading_signals` to receive precise BUY, SELL, or HOLD instructions with stop-loss and take-profit levels, and `get_trend_summary` for a qualitative view of market momentum.


## Available Tools (3)
- **calculate_aroon_metrics**: Compute core Aroon indicators and trend characteristics
- **generate_trading_signals**: Interpret Aroon metrics and identify BUY, SELL, or HOLD signals
- **get_trend_summary**: Provide a high-level qualitative summary of the current market state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aroon Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these high and low prices for a 25-period Aroon strategy: highs=[150, 152, 155, 153, 158], lows=[148, 149, 150, 151, 152]"

**🤖 AI Agent:**
> The current market state shows a Strong Uptrend with an oscillator value of 45.0.

---

**👤 You:**
> "Generate a trading signal for the current Aroon metrics: Up=100, Down=20, Oscillator=80"

**🤖 AI Agent:**
> BUY signal detected at entry price 158.0 with a stop-loss at 152.0.

---

**👤 You:**
> "Is the market currently sideways?"

**🤖 AI Agent:**
> No, the market is currently in a trending state.


## ❓ FAQ

**Q: What triggers a BUY signal?**
A BUY signal is triggered when Aroon Up crosses above Aroon Down, both values are above 70, and Aroon Up is exactly 100.

**Q: How is the stop-loss determined?**
The stop-loss is set at the most recent significant swing low for BUY signals or the recent swing high for SELL signals within the lookback period.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aroon-strategy](https://vinkius.com/ai-agent-connect/aroon-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aroon Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aroon-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aroon Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aroon-strategy": {
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
