# Swing Index Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/swing-index-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Welles Wilder's Swing Index and Cumulative Swing Index for market momentum analysis.

## Description
This MCP server provides deterministic technical analysis tools for calculating the Swing Index (SI) and Cumulative Swing Index (CSI) based on Welles Wilder's methodology. It allows AI agents to identify market momentum, trend strength, and price divergence. Use `calculate_swing_metrics` to derive SI and CSI from OHLC data, `analyze_csi_signals` to detect zero-line crosses and trend shifts, and `get_volatility_context` to understand price intensity relative to the limit move.


## Available Tools (3)
- **analyze_csi_signals**: 
- **calculate_swing_metrics**: 
- **get_volatility_context**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Swing Index Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the swing metrics for this price data: [{'open': 100, 'high': 105, 'low': 98, 'close': 103, 'timestamp': '2023-01-01T00:00:00Z'}, {'open': 103, 'high': 108, 'low': 102, 'close': 107, 'timestamp': '2023-01-02T00:00:00Z'}] with a limit move of 5."

**🤖 AI Agent:**
> The calculated Swing Index (SI) for the second period is 12.5 and the Cumulative Swing Index (CSI) is 12.5.

---

**👤 You:**
> "Are there any trend signals in this CSI series: [0.5, 1.2, 2.5, 0.1, -0.5]?"

**🤖 AI Agent:**
> A bearish zero-line cross was detected as the CSI moved from 0.1 to -0.5.

---

**👤 You:**
> "Check the volatility context for these prices: [{'high': 110, 'low': 100, 'close': 105}] with a limit move of 10."

**🤖 AI Agent:**
> The average volatility ratio is 1.0 and the maximum swing intensity is 15.0.


## ❓ FAQ

**Q: What is the Swing Index?**
The Swing Index is a momentum oscillator that quantifies price movement intensity relative to volatility and a predefined limit move.

**Q: How do I detect a trend reversal?**
You can use `analyze_csi_signals` to identify zero-line crosses or divergences that suggest a change in market direction.

**Q: What is the 'limit move' parameter?**
The limit move is a constant representing the maximum theoretical price movement allowed in a single period, used to scale the index.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/swing-index-calculator](https://vinkius.com/ai-agent-connect/swing-index-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Swing Index Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `swing-index-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Swing Index Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "swing-index-calculator": {
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
