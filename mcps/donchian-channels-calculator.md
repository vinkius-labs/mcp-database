# Donchian Channels Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/donchian-channels-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic Donchian Channels and breakout signal calculator for Turtle Traders.

## Description
This MCP server provides a deterministic toolset for calculating Donchian Channels and breakout signals based on Turtle Trader methodologies. It allows AI agents to analyze market volatility and trend shifts using tools like `calculate_channel_values` to find channel boundaries, `detect_breakout_signals` to identify long or short entries, and `analyze_volatility_and_recency` to assess volatility regimes and breakout recency.


## Available Tools (3)
- **analyze_volatility_and_recency**: Provides context on current market volatility and the timing of the last trend shift
- **calculate_channel_values**: Calculates the primary Donchian Channel components for a specific point in a price series
- **detect_breakout_signals**: Identifies if the current price action constitutes a Long or Short entry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Donchian Channels Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Donchian Channel values for these prices: highs [10, 12, 15, 14, 16], lows [8, 7, 9, 8, 10], and closes [9, 11, 14, 13, 15] with a period of 3."

**🤖 AI Agent:**
> The upper channel is 15, the lower channel is 8, the middle channel is 11.5, and the channel width is 7.

---

**👤 You:**
> "Is there a breakout signal if the upper channel is 150, the lower channel is 140, and the current close is 155?"

**🤖 AI Agent:**
> Yes, a long entry signal has been triggered because the current close is greater than the upper channel.

---

**👤 You:**
> "What is the volatility percentile for a current width of 5 given historical widths [2, 3, 4, 5, 6, 7, 8]?"

**🤖 AI Agent:**
> The volatility percentile is 0.4286.


## ❓ FAQ

**Q: What are Donchian Channels?**
Donchian Channels are technical indicators that use the highest high and lowest low over a specific period to define price boundaries and volatility.

**Q: How do I detect a breakout?**
You can use the `detect_breakout_signals` tool to determine if the current closing price has crossed the upper or lower channel boundaries.

**Q: Can I customize the lookback period?**
Yes, the `calculate_channel_values` tool allows you to specify a custom period, which defaults to 20.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/donchian-channels-calculator](https://vinkius.com/mcp/donchian-channels-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Donchian Channels Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `donchian-channels-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Donchian Channels Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "donchian-channels-calculator": {
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
