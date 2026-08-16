# Tick Index Cumulative Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tick-index-cumulative-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate cumulative tick indices, momentum, and statistical breadth metrics.

## Description
This MCP server provides a deterministic analytical engine for market breadth analysis. It allows AI agents to calculate cumulative tick indices, momentum, and volatility-adjusted Z-scores. Use `calculate_tick_metrics` to get a full suite of metrics including moving averages and momentum. Use `detect_divergences` to identify bearish discrepancies between price action and cumulative breadth. Finally, use `get_breadth_classification` to determine market states like overbought or oversold and receive mean-reversion signals.


## Available Tools (3)
- **calculate_tick_metrics**: Provides a comprehensive suite of cumulative, momentum, and statistical breadth metrics
- **detect_divergences**: Identifies discrepancies between price action and cumulative breadth trends
- **get_breadth_classification**: Categorizes the current market state based on volatility-adjusted and threshold-based breadth indicators


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tick Index Cumulative Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the tick metrics for these daily indices: [100, 150, -50, 200, 300] with a lookback of 5."

**🤖 AI Agent:**
> The cumulative index is 500, the 10-day moving average is 120, and the momentum is 100.

---

**👤 You:**
> "Is there a bearish divergence if the cumulative tick index hit 5000 but the price only hit 150?"

**🤖 AI Agent:**
> Yes, a bearish divergence is detected because the cumulative tick index reached a new high while the price failed to reach a corresponding new high.

---

**👤 You:**
> "Classify the market state for a Z-score of 2.5 and a tick of 1200."

**🤖 AI Agent:**
> The market is classified as Extreme Positive and the mean-reversion signal is Sell.


## ❓ FAQ

**Q: What is a cumulative tick index?**
It is the running total of daily tick index values, used to visualize long-term market breadth trends.

**Q: How do I detect bearish divergence?**
You can use the `detect_divergences` tool to find instances where the cumulative tick index reaches a new peak but the price series fails to do so.

**Q: What defines an overbought state?**
An overbought state is identified when the current tick index exceeds 1000.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tick-index-cumulative-calculator](https://vinkius.com/mcp/tick-index-cumulative-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tick Index Cumulative Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tick-index-cumulative-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tick Index Cumulative Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tick-index-cumulative-calculator": {
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
