# Market Breadth Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/market-breadth-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate NH/NL ratios, breadth thrust signals, and market sentiment.

## Description
This MCP server provides deterministic market breadth analysis. It allows AI agents to calculate the ratio between new highs and new lows, identify bullish breadth thrust signals, and classify market sentiment. Use `calculate_breadth_metrics` for immediate counts, `analyze_breadth_trends` to detect moving averages and breakout signals, or `get_market_classification` to determine if the market is bullish, neutral, or bearish.


## Available Tools (3)
- **analyze_breadth_trends**: Analyzes historical breadth data to identify moving averages and specific breakout signals
- **calculate_breadth_metrics**: Provides the core mathematical breakdown of the current market breadth based on immediate counts
- **get_market_classification**: Returns a simplified descriptive status of the market based on the current ratio


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Market Breadth Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the breadth metrics for 150 new highs, 50 new lows, and 1000 total stocks."

**🤖 AI Agent:**
> The NH/NL ratio is 3.0, the difference is 100, and the percentage is 10.0%. The sentiment is bullish.

---

**👤 You:**
> "What is the market sentiment if the current NH/NL ratio is 1.5?"

**🤖 AI Agent:**
> The market sentiment is neutral.

---

**👤 You:**
> "Is there a breadth thrust signal in this history?"

**🤖 AI Agent:**
> No breadth thrust signal has been detected in the provided history.


## ❓ FAQ

**Q: What is a breadth thrust?**
A breadth thrust is a strong bullish signal triggered when the difference between new highs and new lows exceeds 620 after a 50-day period of absence.

**Q: How is market sentiment classified?**
Sentiment is classified by the NH/NL ratio: bullish if > 2, neutral if between 1 and 2, and bearish if < 1.

**Q: Can I calculate moving averages?**
Yes, you can use `analyze_breadth_trends` to calculate the 10-day moving average of the NH/NL ratio.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/market-breadth-analyzer](https://vinkius.com/mcp/market-breadth-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Market Breadth Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `market-breadth-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Market Breadth Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "market-breadth-analyzer": {
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
