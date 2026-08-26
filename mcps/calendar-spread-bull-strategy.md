# Calendar Spread Bull Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/calendar-spread-bull-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantitative tool for identifying bull calendar spread signals using z-score and backwardation analysis.

## Description
This MCP server provides deterministic quantitative tools for executing bull calendar spreads in futures markets. By analyzing price compression and market structure, it identifies high-probability entries. Use `analyze_spread_signals` to generate actionable buy/sell signals based on z-score thresholds and backwardation conditions. The `calculate_spread_metrics` tool provides descriptive statistics like absolute width and convergence targets, while `validate_instrument_eligibility` ensures liquidity and underlying asset matching requirements are met before trading.


## Available Tools (3)
- **validate_instrument_eligibility**: Verifies if two futures contracts are suitable for a calendar spread
- **analyze_spread_signals**: Calculates daily spread metrics and generates actionable buy/sell signals
- **calculate_spread_metrics**: Computes descriptive statistics and convergence targets for a spread


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calendar Spread Bull Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these spread signals for the last 30 days."

**🤖 AI Agent:**
> The analysis shows a BUY signal for today because the z-score is -2.4 and the market is in backwardation with sufficient liquidity.

---

**👤 You:**
> "Check if these two contracts are eligible for a calendar spread."

**🤖 AI Agent:**
> Yes, the contracts are eligible because the underlying assets match and both have an Open Interest above 5,000.

---

**👤 You:**
> "What is the current spread width and convergence target?"

**🤖 AI Agent:**
> The absolute width is 2.50, the percentage width is 0.5%, and the estimated convergence target is 0.0.


## ❓ FAQ

**Q: What triggers a BUY signal?**
A BUY signal is triggered when the spread z-score is less than -2.0 and the market is in backwardation (near-term price is higher than far-term price).

**Q: How does the tool handle liquidity?**
The `analyze_spread_signals` tool includes a liquidity filter that only generates signals if both the near-term and far-term Open Interest are greater than 5,000 contracts.

**Q: Can I use this for any futures contract?**
The strategy requires both contracts to have the same underlying asset. You can use `validate_instrument_eligibility` to confirm if your selected contracts are suitable.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/calendar-spread-bull-strategy](https://vinkius.com/ai-agent-connect/calendar-spread-bull-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Calendar Spread Bull Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `calendar-spread-bull-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Calendar Spread Bull Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calendar-spread-bull-strategy": {
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
