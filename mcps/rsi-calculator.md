# RSI Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/rsi-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic Relative Strength Index (RSI) calculator with smoothing and divergence detection.

## Description
This MCP server provides precise technical analysis tools for the Relative Strength Index (RSI). It allows AI agents to calculate RSI values using Wilder's smoothing, SMA, or EMA methods. Beyond simple calculation, it can identify overbought and oversold market conditions using `analyze_rsi_extremes` and detect momentum shifts through `detect_divergence`. It is a reliable bridge for agents performing quantitative financial analysis.


## Available Tools (3)
- **analyze_rsi_extremes**: 
- **calculate_rsi**: 
- **detect_divergence**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RSI Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the RSI for these closing prices: [44.3, 44.8, 45.1, 44.9, 45.5, 46.0, 45.8, 46.2, 46.5, 47.0, 46.8, 47.2, 47.5, 48.0] using wilders smoothing."

**🤖 AI Agent:**
> The calculated RSI for the provided price series using Wilder's smoothing is 68.42.

---

**👤 You:**
> "Is an RSI value of 75 considered overbought?"

**🤖 AI Agent:**
> Yes, an RSI value of 75 is considered overbought as it is strictly greater than 70.

---

**👤 You:**
> "Check if there is a divergence between these prices [100, 105, 110, 108] and these RSI values [50, 55, 52, 54]."

**🤖 AI Agent:**
> A bearish divergence was detected because the price reached a higher peak (110) while the RSI reached a lower peak (55) compared to its previous state.


## ❓ FAQ

**Q: What smoothing methods are supported?**
The server supports Wilder's smoothing, Simple Moving Average (SMA), and Exponential Moving Average (EMA).

**Q: How do I detect market reversals?**
You can use `analyze_rsi_extremes` to find overbought or oversold signals, or `detect_divergence` to find discrepancies between price action and RSI momentum.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, this MCP server can be connected to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/rsi-calculator](https://vinkius.com/ai-agent-connect/rsi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RSI Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rsi-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RSI Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rsi-calculator": {
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
