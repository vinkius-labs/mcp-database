# Product Markup Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/product-markup-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate markup, selling price, and profit margins.

## Description
This MCP server provides essential tools for pricing strategy and profitability analysis. Use `get_markup_percentage` to find the percentage increase over cost, `get_selling_price` to determine final customer pricing, `get_profit_from_markup` to project earnings, and `get_margin_comparison` to understand the relationship between markup and margin.


## Available Tools (4)
- **get_profit_from_markup**: Calculates monetary profit from a cost and markup percentage
- **get_selling_price**: Calculates the final selling price given cost and profit
- **get_margin_comparison**: Compares markup percentage and margin percentage
- **get_markup_percentage**: Calculates markup percentage from cost and profit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Product Markup Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If a product costs $50 and I want a $20 profit, what is the markup percentage?"

**🤖 AI Agent:**
> The markup percentage is 40%.

---

**👤 You:**
> "What should the selling price be for an item that costs $100 with a $25 profit?"

**🤖 AI Agent:**
> The final selling price should be $125.

---

**👤 You:**
> "How much profit will I make if I apply a 30% markup to a $200 item?"

**🤖 AI Agent:**
> The resulting monetary profit will be $60.


## ❓ FAQ

**Q: How do I calculate the selling price?**
You can use the `get_selling_price` tool by providing the original cost and the desired profit amount.

**Q: What is the difference between markup and margin?**
Markup is the profit relative to the cost, while margin is the profit relative to the selling price. Use `get_margin_comparison` to see both values at once.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/product-markup-calculator](https://vinkius.com/en/ai-agent-connect/product-markup-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Product Markup Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `product-markup-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Product Markup Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "product-markup-calculator": {
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
