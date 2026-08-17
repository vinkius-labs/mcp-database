# Futures Options Diagonal Spread Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/futures-options-diagonal-spread-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A deterministic decision engine for executing futures options diagonal spread strategies.

## Description
This MCP server provides a specialized decision engine for executing diagonal spread strategies using futures options. It targets the exploitation of volatility skew and time decay differentials by analyzing the relationship between near-term and far-term options. Users can use `analyze_diagonal_spread` to generate BUY, SELL, or HOLD signals based on implied volatility, delta exposure, and liquidity. The engine also provides `calculate_position_metrics` for detailed risk/reward analysis and `validate_liquidity_and_risk` to ensure trades meet strict gamma and open interest safety thresholds.


## Available Tools (3)
- **analyze_diagonal_spread**: Evaluates a specific diagonal spread setup to determine if a trade signal (BUY, SELL, or HOLD) should be generated
- **calculate_position_metrics**: Calculates the mathematical risk and reward components of a proposed diagonal spread
- **validate_liquidity_and_risk**: Verifies if the specific contract parameters meet the safety and liquidity requirements for trading


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Futures Options Diagonal Spread Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this diagonal spread: call option, near-term strike 4500, far-term strike 4450, near-term premium 150, far-term premium 300, near-term delta 0.3, far-term delta 0.5, near-term IV 40, far-term IV 30, near-term days 30, far-term days 60, near-term OI 500, far-term OI 500."

**🤖 AI Agent:**
> Signal: BUY. Near-term Strike: 4500, Far-term Strike: 4450, Debit: 150, Delta Exposure: 0.2, Max Profit: 300, Max Loss: 150.

---

**👤 You:**
> "Calculate the risk metrics for a put diagonal spread with near-term strike 4200, far-term strike 4300, near-term premium 80, far-term premium 200, near-term delta -0.2, far-term delta -0.4."

**🤖 AI Agent:**
> Diagonal Spread Debit: 120, Delta Exposure: -0.2, Max Profit: 180, Max Loss: 120, Theta Benefit: 12.5.

---

**👤 You:**
> "Check if this trade is safe: near-term OI 100, far-term OI 500, near-term days 10."

**🤖 AI Agent:**
> Trade rejected: Insufficient liquidity (near-term OI below 300) and high gamma risk (near-term days below 14).


## ❓ FAQ

**Q: What is a diagonal spread?**
A diagonal spread is an options strategy involving the simultaneous purchase and sale of options with different strike prices and different expiration dates.

**Q: How does the engine determine a BUY signal?**
A BUY signal is generated via `analyze_diagonal_spread` when near-term IV is higher than far-term IV, near-term expiration is between 14 and 45 days, both options have sufficient Open Interest, and the debit is cost-effective.

**Q: What is the purpose of the liquidity check?**
The `validate_liquidity_and_risk` tool ensures that the options have enough Open Interest (above 300) to avoid slippage and that the position is not exposed to excessive gamma risk.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/futures-options-diagonal-spread-strategy](https://vinkius.com/ai-agent-connect/futures-options-diagonal-spread-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Futures Options Diagonal Spread Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `futures-options-diagonal-spread-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Futures Options Diagonal Spread Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "futures-options-diagonal-spread-strategy": {
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
