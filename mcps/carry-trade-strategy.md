# Carry Trade Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/carry-trade-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic forex carry trade strategy using interest rate differentials and volatility filters.

## Description
This MCP server provides tools to execute a deterministic forex carry trade strategy. It identifies trading opportunities by calculating the interest rate differential between currency pairs and filtering for trend confirmation using moving averages. The strategy uses `analyze_carry_signals` to generate BUY, SELL, or HOLD signals, ensuring trades are only entered when the positive carry is not offset by excessive volatility. It also includes `get_pair_metadata` to restrict trading to major pairs and `calculate_volatility_risk` to ensure market fluctuations remain within safe thresholds.


## Available Tools (3)
- **analyze_carry_signals**: Generates trading signals (BUY, SELL, HOLD) and calculates carry-related metrics for a given historical price series
- **get_pair_metadata**: Validates if a specific currency pair is eligible for the carry strategy
- **calculate_volatility_risk**: Determines if the current market volatility exceeds the allowable risk threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Carry Trade Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the carry signals for EUR/USD with a base rate of 5%, a quote rate of 2%, and these ATR values: [0.005, 0.006, 0.005]."

**🤖 AI Agent:**
> The signal for EUR/USD is BUY. The entry price is 1.0850, with a stop-loss at 1.0785 and a take-profit based on trend reversal.

---

**👤 You:**
> "Is USD/JPY a major pair for this strategy?"

**🤖 AI Agent:**
> Yes, USD/JPY is a major pair.

---

**👤 You:**
> "Check if the current volatility for EUR/USD is acceptable given an ATR of 0.01 and a price of 1.08."

**🤖 AI Agent:**
> The volatility risk is acceptable.


## ❓ FAQ

**Q: What currency pairs are supported?**
The strategy is restricted to major pairs: EUR/USD, USD/JPY, GBP/USD, and AUD/USD.

**Q: How is the volatility risk assessed?**
Risk is assessed using `calculate_volatility_risk`, which checks if the annualized volatility derived from ATR exceeds 15%.

**Q: What triggers a BUY signal?**
A BUY signal is triggered via `analyze_carry_signals` when the interest rate differential is greater than 2% and the price is above the 50-day Moving Average.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/carry-trade-strategy](https://vinkius.com/ai-agent-connect/carry-trade-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Carry Trade Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `carry-trade-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Carry Trade Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "carry-trade-strategy": {
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
