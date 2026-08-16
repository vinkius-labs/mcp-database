# Volume Breakout Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/volume-breakout-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify momentum breakouts using price action and volume surge validation.

## Description
This MCP server provides deterministic trading signals by identifying momentum breakouts. It uses `calculate_signals` to detect BUY and SELL opportunities based on price extremes and volume surges. It also includes `analyze_breakout_metrics` to evaluate the strength of a breakout via volume multiples and price gaps, and `get_trade_parameters` to calculate precise entry, stop-loss, and take-profit levels.


## Available Tools (3)
- **analyze_breakout_metrics**: Analyze breakout strength
- **calculate_signals**: 
- **get_trade_parameters**: Get trade execution levels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Volume Breakout Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate trading signals for this price and volume data."

**🤖 AI Agent:**
> The signal for the current bar is BUY with an entry price of 150.50, a stop-loss at 148.20, and a take-profit at 154.25.

---

**👤 You:**
> "How strong was the breakout at index 45?"

**🤖 AI Agent:**
> The breakout at index 45 had a volume multiple of 2.5, a price gap of 0.45, and showed successful follow-through.

---

**👤 You:**
> "Calculate the trade parameters for a BUY signal at 100.00."

**🤖 AI Agent:**
> The trade plan is: Entry at 100.00, Stop-Loss at 98.50, and Take-Profit at 103.00.


## ❓ FAQ

**Q: What triggers a BUY signal?**
A BUY signal is triggered when the closing price exceeds the highest high of the lookback period, volume is greater than the multiplier times the average volume, ADX is above 20, and no news gap is present.

**Q: How are trade levels calculated?**
The `get_trade_parameters` tool calculates entry, stop-loss, and take-profit levels based on ATR and the breakout range.

**Q: Can I analyze the quality of a breakout?**
Yes, use `analyze_breakout_metrics` to get data on volume multiples, price gaps, and follow-through confirmation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/volume-breakout-strategy](https://vinkius.com/ai-agent-connect/volume-breakout-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Volume Breakout Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `volume-breakout-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Volume Breakout Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "volume-breakout-strategy": {
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
