# Futures Term Structure Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/futures-term-structure-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze futures curve geometry, slope, and curvature to generate deterministic trading signals.

## Description
This MCP server provides deterministic tools to analyze the shape of the futures curve. It allows AI agents to calculate the geometric properties of the term structure, including slope, curvature, and monotonicity. By using `analyze_curve_shape`, agents can identify contango or backwardation states. The `evaluate_trading_signal` tool generates specific BUY, SELL, or HOLD signals based on slope thresholds and moving averages, while `select_optimal_contract` identifies the best risk/reward contract based on liquidity and curve position.


## Available Tools (3)
- **analyze_curve_shape**: Calculates the fundamental geometric properties of the current futures term structure
- **evaluate_trading_signal**: Generates specific BUY, SELL, or HOLD signals based on slope, moving averages, and volatility filters
- **select_optimal_contract**: Identifies the specific contract month that offers the best risk/reward profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Futures Term Structure Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the current futures curve shape using the provided pricing data."

**🤖 AI Agent:**
> The current curve shows a slope of -2.5% per month, indicating steep backwardation, with a curvature of 0.01.

---

**👤 You:**
> "Should I buy the front-month contract based on the current slope and price?"

**🤖 AI Agent:**
> BUY signal: The slope is -2.8% and the front-month price is above its 20-day moving average.

---

**👤 You:**
> "Which contract is the best to trade right now?"

**🤖 AI Agent:**
> The optimal contract is DEC-24 due to high liquidity and favorable roll yield in the current backwardation state.


## ❓ FAQ

**Q: What does the strategy consider a significant signal?**
A signal is considered significant if the change in slope compared to the previous period is greater than 1%.

**Q: How does the tool handle liquidity requirements?**
The `select_optimal_contract` tool requires all candidate contracts to have an Open Interest (OI) greater than 5,000 to ensure sufficient liquidity.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/futures-term-structure-strategy](https://vinkius.com/ai-agent-connect/futures-term-structure-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Futures Term Structure Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `futures-term-structure-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Futures Term Structure Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "futures-term-structure-strategy": {
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
