# Stock Average Price Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/stock-average-price-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate weighted average cost basis for stock portfolios.

## Description
This MCP server provides tools to manage and calculate the weighted average cost basis of stock holdings. Users can record new transactions using `add_purchase`, retrieve full purchase histories with `get_transaction_history`, and check current holdings via `get_average_price`. It also includes `validate_portfolio_integrity` to ensure transaction records match the calculated averages. It is compatible with Cursor, VS Code, Claude Desktop, Windsurf, and any MCP-compatible client.


## Available Tools (4)
- **add_purchase**: It will update the average price.

Record a new purchase of a stock
- **get_average_price**: Get the current weighted average price of total holdings for a specific stock
- **get_transaction_history**: Get all individual purchase events for a specific stock
- **validate_portfolio_integrity**: Verify if recorded transactions are consistent with calculated averages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stock Average Price Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current average price for AAPL?"

**🤖 AI Agent:**
> The current weighted average price for AAPL is $150.25 with a total of 50 shares held.

---

**👤 You:**
> "I just bought 10 shares of MSFT at $300.00 today."

**🤖 AI Agent:**
> Successfully added the purchase. Your new average price for MSFT is $300.00.

---

**👤 You:**
> "Show me all my transactions for TSLA."

**🤖 AI Agent:**
> You have three transactions for TSLA: 5 shares at $200.00 on 2023-01-10, 10 shares at $210.00 on 2023-02-15, and 2 shares at $220.00 on 2023-03-01.


## ❓ FAQ

**Q: How is the average price calculated?**
The average price is the total cost of all shares divided by the total quantity of shares held.

**Q: Can I add new stock purchases?**
Yes, you can use the `add_purchase` tool to record new transactions and automatically update your average price.

**Q: How do I verify my portfolio data?**
You can use `validate_portfolio_integrity` to perform a checksum and ensure your transaction history matches your calculated averages.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/stock-average-price-tracker](https://vinkius.com/en/ai-agent-connect/stock-average-price-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stock Average Price Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stock-average-price-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stock Average Price Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stock-average-price-tracker": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
