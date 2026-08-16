# Momentum Strategy Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/momentum-strategy-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic multi-factor momentum strategy for generating actionable trading signals.

## Description
This MCP server provides a deterministic engine for executing multi-factor momentum strategies. It uses Rate of Change (ROC) calculations across multiple timeframes to identify trends and generate precise trading signals. Users can utilize `calculate_signals` to determine buy, sell, or hold actions based on dual-timeframe alignment, `rank_assets` to compare momentum strength across a portfolio using weighted composite scores, and `analyze_persistence` to evaluate the stability of an asset's upward trend. The engine incorporates risk management features like swing-low based stop-losses and momentum weakness filters.


## Available Tools (3)
- **analyze_persistence**: Determines the stability of a price trend by measuring how long momentum has remained positive
- **calculate_signals**: Generates actionable buy, sell, or hold signals for a provided set of asset price data
- **rank_assets**: Ranks multiple assets based on a weighted composite momentum score


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Momentum Strategy Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate trading signals for these assets: [{'assetId': 'AAPL', 'prices': [150, 155, 160, 158, 165]}] with a 21-day short term and 252-day long term period."

**🤖 AI Agent:**
> The signal for AAPL is BUY with an entry price of 165 and a stop-loss at 158.

---

**👤 You:**
> "Rank these assets by momentum: [{'assetId': 'BTC', 'prices': [40000, 42000, 45000]}, {'assetId': 'ETH', 'prices': [2000, 2100, 2050]}] using weights {'m12': 0.5, 'm6': 0.3, 'm3': 0.2}."

**🤖 AI Agent:**
> BTC has a momentum score of 12.5 and ETH has a momentum score of 2.5. BTC is ranked first.

---

**👤 You:**
> "How stable is the trend for this price series: [100, 105, 110, 115, 120] with a 1-month interval?"

**🤖 AI Agent:**
> The momentum persistence count is 4.


## ❓ FAQ

**Q: How are trading signals generated?**
Signals are generated using `calculate_signals`, which triggers a BUY when both long-term and short-term ROC are positive, and a SELL when long-term ROC falls below -10%.

**Q: Can I rank multiple assets at once?**
Yes, the `rank_assets` tool allows you to compare multiple assets by calculating a weighted composite momentum score for each.

**Q: What is momentum persistence?**
Momentum persistence is the measure of how many consecutive periods an asset's ROC has remained positive, which can be checked using `analyze_persistence`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/momentum-strategy-engine](https://vinkius.com/mcp/momentum-strategy-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Momentum Strategy Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `momentum-strategy-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Momentum Strategy Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "momentum-strategy-engine": {
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
