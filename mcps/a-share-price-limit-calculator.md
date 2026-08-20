# A-share Price Limit Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/a-share-price-limit-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates daily upper and lower price limits for Chinese A-share stocks.

## Description
This MCP server provides deterministic tools for calculating the daily price boundaries for stocks in the Chinese A-share market. It accounts for specific regulatory rules across different boards including the Main Board, ChiNext, STAR Market, and BSE. Using `calculate_price_limits`, users can find the exact upper and lower bounds based on the previous close, the specific board, and whether the stock has ST (Special Treatment) status. It also includes `get_board_configuration` to check standard volatility limits and `validate_price_tick` to ensure prices adhere to the required 0.01 precision.


## Available Tools (3)
- **calculate_price_limits**: Calculates the specific upper and lower price boundaries for a single stock
- **validate_price_tick**: 01 precision level.

Verifies if a calculated price adheres to standard Chinese market decimal precision
- **get_board_configuration**: Retrieves the standard fluctuation percentages assigned to each stock board


## 💬 Prompt Examples

Here are some examples of how you can interact with the **A-share Price Limit Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the price limits for a Main Board stock with a previous close of 10.00 that is not an ST stock?"

**🤖 AI Agent:**
> The limit up price is 11.00 and the limit down price is 9.00.

---

**👤 You:**
> "Calculate the limits for a ChiNext stock with a previous close of 50.00."

**🤖 AI Agent:**
> The limit up price is 60.00 and the limit down price is 40.00.

---

**👤 You:**
> "What are the limits for an ST stock on the Main Board with a previous close of 5.00?"

**🤖 AI Agent:**
> The limit up price is 5.25 and the limit down price is 4.75.


## ❓ FAQ

**Q: How are the price limits determined?**
Limits are determined by the stock board and ST status. For example, the Main Board has a 10% limit, which reduces to 5% for ST stocks. ChiNext and STAR Market use 20%, while BSE uses 30%.

**Q: Can I check the standard limits for a specific board?**
Yes, you can use the `get_board_configuration` tool to retrieve the standard fluctuation percentages for any recognized market board.

**Q: Does this tool handle Chinese rounding rules?**
Yes, the `calculate_price_limits` tool implements the specific discretization and rounding logic required for the Chinese market to ensure valid price ticks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/a-share-price-limit-calculator](https://vinkius.com/ai-agent-connect/a-share-price-limit-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **A-share Price Limit Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `a-share-price-limit-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **A-share Price Limit Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "a-share-price-limit-calculator": {
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
