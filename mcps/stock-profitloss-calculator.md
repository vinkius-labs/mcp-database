# Stock Profit/Loss Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stock-profitloss-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate ROI, tax liabilities, and risk metrics for stock trades and options strategies.

## Description
A specialized financial utility for calculating the precise performance, taxation, and risk metrics of individual stock trades and complex multi-leg options strategies. Use `analyze_stock_trade` to determine net profitability and tax liabilities (short-term vs long-term) based on entry/exit prices and transaction costs. Use `evaluate_options_strategy` to estimate maximum profit, maximum loss, break-even points, and risk/reward ratios for single-leg and vertical spread options strategies. Use `plan_position_size` to calculate optimal units to purchase based on your portfolio value and stop-loss distance.


## Available Tools (3)
- **evaluate_options_strategy**: Determines the max profit, max loss, and break-even points for multi-leg options strategies
- **plan_position_size**: Calculates how many units to purchase for a specific risk management plan
- **analyze_stock_trade**: Calculates the net profitability and tax liabilities for a completed stock transaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stock Profit/Loss Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I bought 100 shares of AAPL at $150 on 2023-01-01 and sold them at $180 on 2024-02-01. Commissions were $5 per side and spread cost was $2. My short-term tax rate is 30% and long-term is 15%. What was my net profit?"

**🤖 AI Agent:**
> Your net profit after all fees and taxes is $2,873.00. Your ROI is 19.15% and your annualized return is approximately 14.6%.

---

**👤 You:**
> "Evaluate a vertical spread: Buy 1 CALL at $100 strike for $5 premium, Sell 1 CALL at $110 strike for $2 premium. Current price is $105. Total commission is $1. What is my max profit and break-even?"

**🤖 AI Agent:**
> The maximum profit for this strategy is $7.00 (difference in strikes minus net premium and commissions). The break-even price is $103.00.

---

**👤 You:**
> "I have a $50,000 portfolio. I want to risk only 2% of my total capital on a trade entering at $45 with a stop-loss at $42. How many shares should I buy?"

**🤖 AI Agent:**
> You should purchase 166 units. This results in a total position cost of $7,470 and a cash at risk of $498.


## ❓ FAQ

**Q: How does the tool calculate tax liabilities?**
The `analyze_stock_trade` tool compares your purchase and sale dates. If the holding period is less than one year, it applies the `shortTermTaxRate`; otherwise, it uses the `longTermTaxRate` you provided.

**Q: Can I calculate complex options spreads?**
Yes, using `evaluate_options_strategy`, you can input a JSON array of multiple legs (calls or puts) to find the break-even price and risk/reward ratio for vertical spreads and other multi-leg strategies.

**Q: How do I manage my portfolio risk?**
You can use `plan_position_size` to determine exactly how many units to buy. By providing your total portfolio value and a stop-loss price, the tool calculates the number of shares that keeps your potential loss within your specified risk percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stock-profitloss-calculator](https://vinkius.com/mcp/stock-profitloss-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stock Profit/Loss Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stock-profitloss-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stock Profit/Loss Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stock-profitloss-calculator": {
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
