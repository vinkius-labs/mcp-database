# Opening Range Breakout Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opening-range-breakout-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A deterministic intraday strategy that identifies price breakouts from the initial market opening range.

## Description
This MCP server provides a deterministic intraday trading strategy focused on the Opening Range Breakout (ORB). It identifies high-probability entry signals by calculating the price boundaries established during the market opening. The strategy uses `calculate_orb_parameters` to define the range, `evaluate_breakout_signals` to detect volume-confirmed breakouts, and `track_trade_lifecycle` to manage active trades via automated stop-loss and take-profit logic. It includes built-in volatility filters using ATR to avoid unstable market conditions.


## Available Tools (3)
- **calculate_orb_parameters**: Determines the core boundaries and characteristics of the opening range
- **evaluate_breakout_signals**: Analyzes price action and volume to identify specific Buy or Sell entry signals
- **track_trade_lifecycle**: Monitors ongoing trades to determine if they have hit a Take-Profit, a Stop-Loss, or if they should be held/closed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Opening Range Breakout Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the opening range parameters for this session data."

**🤖 AI Agent:**
> The opening range high is 150.50, the low is 148.20, and the width is 2.30. The session is valid.

---

**👤 You:**
> "Check if there is a breakout signal based on the current price and volume."

**🤖 AI Agent:**
> A BUY signal has been generated at 150.60 with a breakout strength of 0.13.

---

**👤 You:**
> "Monitor the status of my active trades with the current price of 152.00."

**🤖 AI Agent:**
> The trade has been closed because the price hit the take-profit level of 152.15.


## ❓ FAQ

**Q: How does the strategy confirm a breakout?**
A breakout is confirmed when the price moves beyond the ORB High or Low with a volume surge exceeding 1.5 times the average opening volume.

**Q: What is the volatility filter?**
The strategy uses an ATR filter; if the ORB width is greater than twice the 20-day ATR, the session is marked as too volatile and trades are skipped.

**Q: How are stop-loss and take-profit levels determined?**
Stop-loss is set at the ORB midpoint or the opposite boundary, while take-profit is set at 1.5 times the ORB width.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opening-range-breakout-strategy](https://vinkius.com/mcp/opening-range-breakout-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Opening Range Breakout Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `opening-range-breakout-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Opening Range Breakout Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opening-range-breakout-strategy": {
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
