# Earnings Announcement Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/earnings-announcement-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A deterministic engine to exploit volatility mispricing around earnings events.

## Description
This MCP server provides a deterministic strategy engine that identifies volatility mispricing around earnings announcements. By comparing market-implied expected moves (via straddle prices) against historical realized volatility, it generates precise signals to either sell or buy volatility. Use `analyze_earnings_mispricing` to detect if options are overpricing or underpricing risk, `generate_trade_execution_plan` to obtain specific entry strikes and timing, and `calculate_strategy_performance` to evaluate theoretical outcomes based on actual market moves and IV crush.


## Available Tools (3)
- **analyze_earnings_mispricing**: Determines if current options pricing correctly reflects historical volatility patterns
- **calculate_strategy_performance**: Evaluates the theoretical outcome of the strategy
- **generate_trade_execution_plan**: Provides specific parameters required to execute the identified strategy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Earnings Announcement Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the earnings mispricing for a stock currently at $150 with a straddle price of $5, a historical move of 3%, and an open interest of 500."

**🤖 AI Agent:**
> The expected move is 3.33%. Since this is greater than the historical average move of 3%, the signal is SELL_VOLATILITY. The trade is valid as liquidity requirements are met.

---

**👤 You:**
> "Generate an execution plan for a BUY_VOLATILITY signal on a stock priced at $200 with a straddle price of $4."

**🤖 AI Agent:**
> The expected move is 2.0%. The entry strikes are $198 and $202, with a total premium of $4.00. The target exit is the earnings announcement open.

---

**👤 You:**
> "Calculate the performance for a SELL_VOLATILITY trade with a $5 premium, where the actual move was 1% and the IV crush was 30%."

**🤖 AI Agent:**
> The trade resulted in a net profit due to the low actual move and significant IV crush impact.


## ❓ FAQ

**Q: How does the strategy identify a trade signal?**
The `analyze_earnings_mispricing` tool compares the expected move derived from the straddle price to the historical average move. If the expected move is higher, it signals to sell volatility; if lower, it signals to buy volatility.

**Q: What are the liquidity requirements for a trade?**
A trade is only considered valid if the stock has a market capitalization of at least $500M and the option open interest is greater than 100 contracts.

**Q: When should I exit the position?**
The `generate_trade_execution_plan` tool specifies the target exit time, which is strictly either at the earnings announcement open or the close of the following trading day.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/earnings-announcement-strategy](https://vinkius.com/ai-agent-connect/earnings-announcement-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Earnings Announcement Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `earnings-announcement-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Earnings Announcement Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "earnings-announcement-strategy": {
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
