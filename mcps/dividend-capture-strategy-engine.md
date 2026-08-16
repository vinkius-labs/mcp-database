# Dividend Capture Strategy Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/dividend-capture-strategy-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify and validate profitable dividend capture opportunities with deterministic modeling.

## Description
This MCP server provides a deterministic analysis engine to identify profitable dividend capture opportunities. It models the timing of trades relative to ex-dividend dates, accounting for price adjustments, transaction costs, and tax implications. Use `analyze_dividend_opportunities` to generate buy/sell signals based on liquidity and yield filters, `calculate_tax_adjusted_returns` to model net profit after tax, and `evaluate_strategy_performance` to aggregate win rates and total returns. It is designed to help investors capture dividends while managing risks like price drops and short interest spikes.


## Available Tools (3)
- **analyze_dividend_opportunities**: Identifies specific buy/sell signals and calculates the financial outcome for every qualifying dividend event
- **calculate_tax_adjusted_returns**: Adjusts the gross profit of a capture opportunity to reflect the specific tax environment
- **evaluate_strategy_performance**: Aggregates all identified signals to provide a high-level summary of the strategy performance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dividend Capture Strategy Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these dividend opportunities for a stock with these prices and schedule."

**🤖 AI Agent:**
> The analysis identified 3 qualifying signals. The most profitable trade occurs on 2024-05-15 with an expected net profit of $0.45 per share.

---

**👤 You:**
> "Calculate the tax-adjusted return for a $500 profit with a 15% tax rate on a qualified dividend."

**🤖 AI Agent:**
> The net profit after tax is $425.00, with a tax amount paid of $75.00.

---

**👤 You:**
> "What was the overall win rate for the provided signals?"

**🤖 AI Agent:**
> The strategy achieved a win rate of 65% with a total net profit of $1,240.50 across 20 trades.


## ❓ FAQ

**Q: What is a dividend capture strategy?**
It is a strategy where an investor buys a stock shortly before the ex-dividend date and sells it shortly after to capture the dividend payment.

**Q: How does the engine handle tax implications?**
You can use the `calculate_tax_adjusted_returns` tool to adjust gross profits based on whether dividends are qualified or non-qualified and the specific tax rate applied.

**Q: What filters are applied to the trade signals?**
The engine filters for liquidity (average daily volume > $5M), minimum annualized yield (> 1%), and low short interest to avoid high borrow costs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/dividend-capture-strategy-engine](https://vinkius.com/ai-agent-connect/dividend-capture-strategy-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dividend Capture Strategy Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dividend-capture-strategy-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dividend Capture Strategy Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dividend-capture-strategy-engine": {
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
