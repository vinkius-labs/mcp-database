# Statistical Arbitrage Pairs Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/statistical-arbitrage-pairs-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Execute deterministic pairs trading using cointegration tests and z-score signals.

## Description
This MCP server provides a deterministic engine for statistical arbitrage. It identifies mean-reverting relationships between two assets by calculating the logarithmic spread and performing an Augmented Dickey-Fuller (ADF) test. Users can use `analyze_pairs_cointegration` to verify if a pair is suitable for trading, `generate_trading_signals` to identify entry and exit points based on z-score thresholds, and `calculate_position_metrics` to determine precise target prices and stop-loss levels. The engine enforces strict filters, such as requiring a half-life of mean reversion under 30 days, to ensure high-quality trading opportunities.


## Available Tools (3)
- **analyze_pairs_cointegration**: Evaluates whether two assets exhibit a stable, mean-reverting relationship suitable for trading
- **generate_trading_signals**: Determines specific entry, exit, and stop-loss triggers for a pair based on z-score thresholds and cointegration filters
- **calculate_position_metrics**: Provides detailed trade execution parameters for a specific signal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Statistical Arbitrage Pairs Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if these two assets are cointegrated: Asset A prices [100, 101, 102, 101, 100] and Asset B prices [50, 51, 52, 51, 50]."

**🤖 AI Agent:**
> The assets are cointegrated with a p-value of 0.02 and a half-life of 12 days, making them suitable for the strategy.

---

**👤 You:**
> "Generate trading signals for Asset A [10, 11, 12, 11, 10] and Asset B [20, 22, 24, 22, 20] with an entry z-score of 2.0."

**🤖 AI Agent:**
> A BUY spread signal was generated at bar index 2 with entry prices A: 12.0 and B: 24.0, using a hedge ratio of 2.0.

---

**👤 You:**
> "Calculate the trade metrics for a spread with mean 0, std dev 1, hedge ratio 1.5, and entry prices A: 100, B: 50."

**🤖 AI Agent:**
> The target spread is 0.0, with stop-loss prices calculated at A: 97.0 and B: 48.5 based on the z-score limit.


## ❓ FAQ

**Q: How does the engine determine if a pair is tradeable?**
The engine uses `analyze_pairs_cointegration` to check if the spread is stationary via an ADF test. A pair is only considered tradeable if the p-value is below 0.05 and the half-life of mean reversion is less than 30 days.

**Q: What information is provided for each trade signal?**
By using `generate_trading_signals`, you receive the bar index, signal type (BUY/SELL/EXIT), entry prices for both assets, the hedge ratio, and specific stop-loss and target prices.

**Q: Can I customize the entry and exit thresholds?**
Yes, when calling `generate_trading_signals`, you can specify custom `entryZScore`, `exitZScore`, and `stopLossZScore` parameters to match your specific risk profile.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/statistical-arbitrage-pairs-strategy](https://vinkius.com/ai-agent-connect/statistical-arbitrage-pairs-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Statistical Arbitrage Pairs Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `statistical-arbitrage-pairs-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Statistical Arbitrage Pairs Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "statistical-arbitrage-pairs-strategy": {
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
