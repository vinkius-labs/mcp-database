# DeFi Options Strategy Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/defi-options-strategy-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic volatility trading signals for DeFi options protocols.

## Description
This MCP server provides a deterministic decision engine for generating volatility-based trading signals. It connects AI agents to DeFi options protocols to evaluate if volatility is overvalued or undervalued. Using `analyze_volatility_regime`, agents can determine the IV rank and volatility signal. The `generate_trade_execution_plan` tool filters these signals against liquidity and catalyst constraints, while `calculate_risk_metrics` provides essential parameters like delta hedge and gamma exposure for position management.


## Available Tools (3)
- **analyze_volatility_regime**: Evaluates the current volatility environment and determines the primary volatility signal
- **calculate_risk_metrics**: Computes the secondary risk parameters required for managing the position
- **generate_trade_execution_plan**: Determines the specific trade structure and filters signals based on liquidity and market catalysts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DeFi Options Strategy Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the current volatility regime with IV at 45%, min 10%, max 60%, straddle price 50, and expected move 40."

**🤖 AI Agent:**
> The IV rank is 0.62, and since the straddle price is higher than the expected move, the volatility signal is SELL.

---

**👤 You:**
> "Check if a BUY signal with IV rank 15, $50M liquidity, 500 open interest, and an upcoming earnings event is actionable."

**🤖 AI Agent:**
> The trade is actionable as it meets the low IV rank, high liquidity, and catalyst requirements.

---

**👤 You:**
> "Calculate the risk metrics for an option with underlying price 100, IV 0.30, 30 days to expiry, delta 0.5, gamma 0.02, and theta -0.05."

**🤖 AI Agent:**
> The expected move is 2.74, the required delta hedge is -0.5, the gamma exposure is 0.02, and the daily theta decay is -0.05.


## ❓ FAQ

**Q: How does the engine determine if volatility is expensive?**
The engine uses `analyze_volatility_regime` to calculate the IV rank. If the IV rank is above 80 and the straddle price exceeds the expected move, it generates a SELL signal.

**Q: What safety filters are applied to trades?**
The `generate_trade_execution_plan` tool ensures SELL signals only trigger if IV rank > 70 and protocol liquidity > $10M, and BUY signals require IV rank < 30 and an upcoming catalyst.

**Q: Can I calculate risk parameters for my position?**
Yes, you can use `calculate_risk_metrics` to obtain the delta hedge, gamma exposure, and theta decay for your specific option position.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/defi-options-strategy-engine](https://vinkius.com/ai-agent-connect/defi-options-strategy-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DeFi Options Strategy Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `defi-options-strategy-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DeFi Options Strategy Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "defi-options-strategy-engine": {
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
