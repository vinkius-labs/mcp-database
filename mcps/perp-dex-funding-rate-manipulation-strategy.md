# Perp DEX Funding Rate Manipulation Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/perp-dex-funding-rate-manipulation-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Detect and exploit artificial funding rate spikes in perpetual DEXs.

## Description
This MCP server provides a deterministic engine to identify artificial funding rate spikes in perpetual decentralized exchanges. By analyzing the disconnect between funding rates and price basis, the server identifies market manipulation. Use `detect_manipulation_signals` to find decoupled funding events, `calculate_exploit_opportunities` to filter for high-liquidity setups, and `estimate_trade_metrics` to project income and basis risk for basis-reversion trades.


## Available Tools (3)
- **detect_manipulation_signals**: Identifies intervals where funding rates are decoupled from price basis and accompanied by specific Open Interest movements
- **estimate_trade_metrics**: Provides detailed financial projections for a specific identified exploit
- **calculate_exploit_opportunities**: Filters detected signals to find high-probability, high-liquidity trade setups


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Perp DEX Funding Rate Manipulation Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify any current market manipulation signals in the provided price and funding data."

**🤖 AI Agent:**
> The `detect_manipulation_signals` tool has identified a manipulation event at 14:00 UTC where the funding rate reached 0.6% while the basis was only 0.05%.

---

**👤 You:**
> "Find high-liquidity exploit opportunities with at least $50M in Open Interest."

**🤖 AI Agent:**
> The `calculate_exploit_opportunities` tool found one valid setup: BUY_SPOT_SELL_PERP with an expected funding income of $12,500.

---

**👤 You:**
> "Calculate the expected income and risk for a $100,000 position with a 0.5% funding rate."

**🤖 AI Agent:**
> For a $100,000 position, the `estimate_trade_metrics` tool calculates a funding income of $500 with a basis risk estimate of $150.


## ❓ FAQ

**Q: How does the server detect manipulation?**
It flags intervals where the funding rate is extreme (above 0.5% or below -0.5%) while the basis remains low (below 0.1%) and Open Interest is dropping, indicating a decoupling of price and funding.

**Q: What is a basis-reversion exploit?**
It is a trade where you capture high funding by buying spot and selling the perpetual contract, waiting for the basis to revert to normal levels.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/perp-dex-funding-rate-manipulation-strategy](https://vinkius.com/ai-agent-connect/perp-dex-funding-rate-manipulation-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Perp DEX Funding Rate Manipulation Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `perp-dex-funding-rate-manipulation-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Perp DEX Funding Rate Manipulation Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "perp-dex-funding-rate-manipulation-strategy": {
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
