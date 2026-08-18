# Sentiment vs Fundamental Divergence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sentiment-vs-fundamental-divergence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Identify arbitrage opportunities by detecting divergences between social hype and on-chain utility.

## Description
This MCP server provides deterministic trading signals by analyzing the statistical divergence between social media sentiment and on-chain fundamental metrics. By calculating Z-scores for both social volume and fundamental activity, it identifies 'Speculative Bubbles' (high hype, low utility) and 'Accumulation' phases (low hype, high utility). Use `calculate_divergence_signal` to generate BUY or SELL signals, `validate_stop_loss` to manage risk with a 15% threshold, and `get_historical_performance` to backtest the strategy against historical datasets.


## Available Tools (3)
- **get_historical_performance**: Backtests the divergence strategy against historical data
- **calculate_divergence_signal**: Evaluates current market conditions to determine if a BUY or SELL signal is generated
- **validate_stop_loss**: Checks if a current position has reached the maximum allowable risk threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sentiment vs Fundamental Divergence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the current divergence for a crypto asset with a market price of 0.5, social volume of 100, fundamental metric of 50, and historical data provided."

**🤖 AI Agent:**
> The current signal is SELL because the social Z-score is 2.5 (high hype) while the fundamental Z-score is -0.5 (declining utility).

---

**👤 You:**
> "Check if my BUY position at 0.8 is still valid if the current price is 0.68."

**🤖 AI Agent:**
> The stop-loss has been triggered. The price movement is 15% below your entry price.

---

**👤 You:**
> "What is the historical win rate for this strategy using the provided dataset?"

**🤖 AI Agent:**
> The strategy has a historical win rate of 62% across 145 total signals generated.


## ❓ FAQ

**Q: How are the trading signals generated?**
Signals are generated using `calculate_divergence_signal`, which compares the Z-score of social volume against the Z-score of fundamental metrics to find extreme divergences.

**Q: What is the risk management strategy?**
The strategy uses a strict 15% stop-loss. You can use `validate_stop_loss` to check if a position should be exited based on adverse price movement.

**Q: Can I backtest this strategy?**
Yes, the `get_historical_performance` tool allows you to run the divergence strategy against historical snapshots to calculate the win rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sentiment-vs-fundamental-divergence](https://vinkius.com/ai-agent-connect/sentiment-vs-fundamental-divergence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sentiment vs Fundamental Divergence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sentiment-vs-fundamental-divergence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sentiment vs Fundamental Divergence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sentiment-vs-fundamental-divergence": {
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
