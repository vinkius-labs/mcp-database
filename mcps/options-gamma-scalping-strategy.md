# Options Gamma Scalping Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/options-gamma-scalping-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Simulate delta-neutral gamma scalping with automated hedging and cost analysis.

## Description
This MCP server provides a deterministic modeling engine for delta-neutral gamma scalping. It allows AI agents to simulate the P&L dynamics of long convexity positions by managing directional risk through automated delta hedging. Use `simulate_scalping_strategy` to run full time-series simulations, `analyze_gamma_exposure` to inspect real-time Greek exposures, and `calculate_breakeven_metrics` to determine the volatility required for profitability. It is designed to model the relationship between gamma gains, theta decay, and transaction costs.


## Available Tools (3)
- **analyze_gamma_exposure**: Provides a snapshot of Greek exposures and delta-neutrality status
- **calculate_breakeven_metrics**: Determines the theoretical volatility threshold required for profitability
- **simulate_scalping_strategy**: Executes a deterministic simulation of a gamma scalping strategy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Options Gamma Scalping Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run a gamma scalping simulation with these underlying prices [100, 102, 101, 105] and this option chain data."

**🤖 AI Agent:**
> The simulation completed. The net P&L was $12.50, with a breakeven volatility of 18.5%.

---

**👤 You:**
> "What is the current delta exposure for a portfolio with 10 call options at 0.5 delta and 5 units of the underlying?"

**🤖 AI Agent:**
> The total delta is 10.0 (5.0 from options + 5.0 from underlying).

---

**👤 You:**
> "Calculate the breakeven volatility if I have 50 gamma exposure, 10 theta decay, and 5 transaction costs."

**🤖 AI Agent:**
> The required realized volatility to break even is 30%.


## ❓ FAQ

**Q: What is the purpose of this MCP?**
It provides tools to simulate and analyze gamma scalping strategies, specifically focusing on delta-neutral hedging and the impact of volatility on P&L.

**Q: How do I run a full simulation?**
You can use the `simulate_scalping_strategy` tool by providing arrays of underlying prices and the option chain data.

**Q: Can I check my current Greek exposure?**
Yes, the `analyze_gamma_exposure` tool provides a snapshot of total delta, gamma, and theta for a given portfolio.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/options-gamma-scalping-strategy](https://vinkius.com/ai-agent-connect/options-gamma-scalping-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Options Gamma Scalping Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `options-gamma-scalping-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Options Gamma Scalping Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "options-gamma-scalping-strategy": {
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
