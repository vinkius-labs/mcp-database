# Basket Trading Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/basket-trading-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Execute deterministic basket trading by evaluating correlated asset groups against a benchmark.

## Description
This MCP server provides a deterministic quantitative trading system that treats a group of correlated assets as a single unit. By comparing the aggregate performance of a basket against a benchmark index, it identifies high-probability trade signals. Use `calculate_basket_performance` to derive metrics like tracking error and information ratio, `evaluate_trading_signal` to determine BUY, SELL, or HOLD actions based on trend and spread, and `get_basket_composition` to inspect asset weights and correlation. It includes built-in risk management like concentration filters and stop-loss logic.


## Available Tools (3)
- **calculate_basket_performance**: Calculates core performance metrics for the basket and the benchmark
- **evaluate_trading_signal**: Determines the specific trade action (BUY, SELL, HOLD)
- **get_basket_composition**: Provides a summary of the basket composition and its relation to the benchmark


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Basket Trading Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the performance metrics for a tech basket including AAPL and MSFT against the NASDAQ."

**🤖 AI Agent:**
> The basket return is 1.2%, the benchmark return is 0.8%, resulting in a spread of 0.4%. The tracking error is 0.05 and the information ratio is 8.0.

---

**👤 You:**
> "Should I buy the current basket based on these returns and prices?"

**🤖 AI Agent:**
> The signal is BUY. The spread is positive and the basket is trending above its 20-day Moving Average with a correlation of 0.85.

---

**👤 You:**
> "Show me the current composition and correlation for my trading basket."

**🤖 AI Agent:**
> The basket consists of AAPL (25%), MSFT (25%), and GOOGL (50%). However, the signal is HOLD because GOOGL exceeds the 30% concentration limit.


## ❓ FAQ

**Q: How does the system determine a BUY signal?**
A BUY signal is generated when the basket's spread is positive and the basket price is above its 20-day Moving Average, provided the correlation with the benchmark is above 0.8 and no single asset exceeds 30% weight.

**Q: What is the purpose of the concentration filter?**
The concentration filter prevents excessive risk by forcing a HOLD signal if any single asset in the basket accounts for more than 30% of the total weight.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, this MCP server can be connected to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/basket-trading-strategy](https://vinkius.com/ai-agent-connect/basket-trading-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Basket Trading Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `basket-trading-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Basket Trading Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "basket-trading-strategy": {
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
