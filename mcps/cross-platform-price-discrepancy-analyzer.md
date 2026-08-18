# Cross-Platform Price Discrepancy Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/cross-platform-price-discrepancy-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate exact net arbitrage profit and capital requirements across prediction markets.

## Description
This MCP server provides deterministic analysis for prediction market arbitrage. It calculates effective prices by adjusting listed prices for platform-specific fee structures, identifies directional arbitrage opportunities, and determines the minimum trade size needed to overcome fixed transaction costs. Use `analyze_arbitrage_opportunity` to find profitable spreads between Polymarket, PredictIt, and Kalshi, or `calculate_lockup_and_liquidity` to project capital lockup duration and break-even requirements.


## Available Tools (3)
- **analyze_arbitrage_opportunity**: 
- **calculate_lockup_and_liquidity**: Project the time-based and scale-based constraints of an arbitrage setup
- **compare_platform_costs**: Evaluate the cost-efficiency of different platforms for a single specific transaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cross-Platform Price Discrepancy Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is there an arbitrage opportunity between Polymarket (Yes: 0.60, Fee: 2%), PredictIt (Yes: 0.55, Fee: 10%), and Kalshi (Yes: 0.58, Fee: 1%) with $5 in gas fees?"

**🤖 AI Agent:**
> Yes, a profitable arbitrage exists. Buy Yes on PredictIt at an effective price of 0.495 and Buy No on Polymarket at an effective price of 0.412. The net profit after $5 gas fees is $12.40 with a 15% return.

---

**👤 You:**
> "Calculate the minimum trade size for an arbitrage with a $10 fixed fee and a 5% expected spread."

**🤖 AI Agent:**
> The minimum trade size required to cover the $10 fixed fee with a 5% spread is $200.

---

**👤 You:**
> "How long will my capital be locked up if the event resolves in 10 days and withdrawal takes 3 days?"

**🤖 AI Agent:**
> Your capital will be locked up for a total of 13 days.


## ❓ FAQ

**Q: How is the effective price calculated?**
The effective price is the listed platform price adjusted by the platform's fee rate. For example, if a price is 0.50 and the fee is 2%, the effective price is 0.49.

**Q: What does `analyze_arbitrage_opportunity` return?**
It returns the direction of the trade, the cheapest and most expensive platforms, the net profit percentage, absolute profit, capital lockup days, and the minimum trade size.

**Q: How do I account for gas fees?**
Include all one-time fixed costs, such as network gas fees, in the `fixedTransactionFees` parameter when calling the analysis tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/cross-platform-price-discrepancy-analyzer](https://vinkius.com/ai-agent-connect/cross-platform-price-discrepancy-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cross-Platform Price Discrepancy Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cross-platform-price-discrepancy-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cross-Platform Price Discrepancy Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cross-platform-price-discrepancy-analyzer": {
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
