# Token Bonding Curve Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/token-bonding-curve-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic trading signals based on mathematical bonding curve deviations.

## Description
This MCP server provides deterministic trading signals by evaluating token price deviations from a mathematical bonding curve. It identifies undervalued entry points and overvalued exit opportunities by comparing market prices to the theoretical fair value. Use `calculate_trading_signals` to generate BUY, SELL, or HOLD signals based on liquidity, volume, and curve progress. You can also use `get_curve_metrics` to analyze the mathematical state of the curve or `evaluate_liquidity_safety` to check if the reserve balance and daily volume meet risk thresholds.


## Available Tools (3)
- **calculate_trading_signals**: Analyzes current market state against the bonding curve to generate specific BUY, SELL, or HOLD signals
- **evaluate_liquidity_safety**: Determines if the current pool has enough depth to permit trading based on predefined risk thresholds
- **get_curve_metrics**: Provides pure mathematical insights into the curve's state without generating trade signals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Token Bonding Curve Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the current trading state for a token with an initial price of 0.01, a slope of 0.0005, max supply of 1,000,000, current supply of 500,000, reserve balance of 200,000, current price of 0.24, daily volume of 60,000, and rising volume."

**🤖 AI Agent:**
> The current price is $0.24, the fair value is $0.26, and the curve progress is 50%. The signal is BUY.

---

**👤 You:**
> "What are the current curve metrics for a token with initial price 0.01, slope 0.0005, max supply 1,000,000, and current supply 950,000?"

**🤖 AI Agent:**
> The fair value is $0.485, the curve progress is 95%, and the price at max supply will be $0.51.

---

**👤 You:**
> "Is the liquidity safe for a token with a reserve balance of 50,000 and daily volume of 10,000?"

**🤖 AI Agent:**
> No, the liquidity is not safe. The risk level is HIGH.


## ❓ FAQ

**Q: How are BUY signals generated?**
A BUY signal is triggered when the current price is at least 5% below the fair value, the curve is at least 10% complete, daily volume exceeds $50,000, volume is rising, and the reserve balance is above $100,000.

**Q: When does the tool suggest a SELL signal?**
The tool suggests a SELL signal if the current price is more than 5% above the fair value or if the curve progress has exceeded 90%.

**Q: What is the purpose of `evaluate_liquidity_safety`?**
The `evaluate_liquidity_safety` tool checks if the current reserve balance and daily volume meet the minimum safety requirements to ensure trades can be executed without excessive risk.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/token-bonding-curve-strategy](https://vinkius.com/ai-agent-connect/token-bonding-curve-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Token Bonding Curve Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `token-bonding-curve-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Token Bonding Curve Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "token-bonding-curve-strategy": {
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
