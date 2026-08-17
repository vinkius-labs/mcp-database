# SOPR & NUPL Bitcoin Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sopr-nupl-bitcoin-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic on-chain signals for Bitcoin market bottoms and tops.

## Description
This MCP server provides deterministic on-chain signals for Bitcoin by analyzing the relationship between realized profitability (SOPR) and unrealized market sentiment (NUPL). Use `analyze_market_signals` to identify market phases like Capitulation or Euphoria and receive BUY/SELL/HOLD signals. Use `get_market_indicators` for technical context like SOPR moving averages and NUPL percentile ranks, or `get_historical_accuracy` to evaluate past performance based on historical capitulation events.


## Available Tools (3)
- **analyze_market_signals**: 
- **get_historical_accuracy**: 
- **get_market_indicators**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SOPR & NUPL Bitcoin Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current Bitcoin market phase and signal?"

**🤖 AI Agent:**
> The current market phase is Accumulation. The signal is HOLD with a position size of 0%.

---

**👤 You:**
> "Check the historical accuracy of the strategy."

**🤖 AI Agent:**
> The average historical return after a capitulation event (SOPR < 0.95 for 7+ days) is 145%.

---

**👤 You:**
> "Give me the technical indicators for the current market."

**🤖 AI Agent:**
> The current SOPR MA(7) is 1.02, the SOPR slope is positive, and the NUPL percentile rank is 45%.


## ❓ FAQ

**Q: How are the BUY signals generated?**
A BUY signal is triggered when SOPR crosses above 1.0, NUPL is below 0, and SOPR has remained below 1.0 for at least 14 consecutive days.

**Q: What is the difference between SOPR and NUPL?**
SOPR measures realized profit or loss of moved coins, while NUPL measures the total unrealized profit or loss in the network.

**Q: Can I use this with Claude Desktop?**
Yes, this server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sopr-nupl-bitcoin-strategy](https://vinkius.com/ai-agent-connect/sopr-nupl-bitcoin-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SOPR & NUPL Bitcoin Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sopr-nupl-bitcoin-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SOPR & NUPL Bitcoin Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sopr-nupl-bitcoin-strategy": {
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
