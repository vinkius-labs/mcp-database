# Social Sentiment & On-Chain Confluence Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/social-sentiment-on-chain-confluence-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Synthesize social sentiment and on-chain data to generate high-confidence trading signals.

## Description
This MCP server provides a deterministic decision engine that connects AI agents to real-time market intelligence. By analyzing the confluence of social sentiment, social volume, and on-chain network health, it generates actionable BUY, SELL, or HOLD signals. Use `analyze_confluence_signals` to evaluate primary trading signals, `calculate_market_health_metrics` to identify market exhaustion or strength, and `get_signal_confidence` to assess the reliability of current market states.


## Available Tools (3)
- **analyze_confluence_signals**: 
- **calculate_market_health_metrics**: 
- **get_signal_confidence**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Social Sentiment & On-Chain Confluence Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the current market confluence using the latest price, sentiment, and on-chain data."

**🤖 AI Agent:**
> The current confluence score is 4. With sentiment at 75 and rising active addresses, the signal direction is BUY with High confidence.

---

**👤 You:**
> "Check if there is any on-chain divergence occurring right now."

**🤖 AI Agent:**
> No on-chain divergence detected. Price and active addresses are currently trending in the same direction.

---

**👤 You:**
> "What is the current social hype index?"

**🤖 AI Agent:**
> The social hype index is 1.45, indicating a significant spike in social volume compared to the historical average.


## ❓ FAQ

**Q: How are the trading signals generated?**
Signals are generated using a confluence score that aggregates sentiment, active addresses, exchange net flow, and social volume. A BUY signal requires a maximum confluence score of 4 sustained for 3 days.

**Q: What is the purpose of the market health metrics?**
The `calculate_market_health_metrics` tool identifies secondary indicators like sentiment momentum and on-chain divergence to detect potential market exhaustion.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/social-sentiment-on-chain-confluence-strategy](https://vinkius.com/ai-agent-connect/social-sentiment-on-chain-confluence-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Social Sentiment & On-Chain Confluence Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `social-sentiment-on-chain-confluence-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Social Sentiment & On-Chain Confluence Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "social-sentiment-on-chain-confluence-strategy": {
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
