# Secondhand Value Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/secondhand-value-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Estimate the current market value and optimal resale strategy for used items.

## Description
The Secondhand Value Calculator helps you determine the worth of your pre-owned goods. Using `estimate_market_valuation`, you can find the depreciation curve and estimated resale range based on age and condition. Use `calculate_net_proceeds` to understand how much cash you'll actually keep after marketplace fees. Finally, use `evaluate_disposal_utility` to decide whether it is better to sell, donate, or repair your item.


## Available Tools (3)
- **evaluate_disposal_utility**: Recommend a disposal strategy
- **calculate_net_proceeds**: Calculate net proceeds after platform fees
- **estimate_market_valuation**: Estimate the current market value of an item


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Secondhand Value Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the estimated value of a 2-year-old iPhone 13 in Excellent condition originally bought for $800?"

**🤖 AI Agent:**
> The estimated resale range is between $450 and $520, with a gradual depreciation curve.

---

**👤 You:**
> "If I sell an item for $100 with a 15% platform fee, how much will I receive?"

**🤖 AI Agent:**
> You will receive $85.00 after the $15.00 fee is deducted.

---

**👤 You:**
> "I have a laptop worth $200 but repairs cost $250. Should I repair it?"

**🤖 AI Agent:**
> The recommended strategy is to Sell or Donate, as the repair cost exceeds the current market value.


## ❓ FAQ

**Q: How can I find out how much my old phone is worth?**
You can use the `estimate_market_valuation` tool by providing its age, brand, and condition.

**Q: Will it tell me if I should sell or donate?**
Yes, the `evaluate_disposal_utility` tool provides a recommendation based on market value and repair costs.

**Q: Does it account for marketplace fees?**
Yes, you can use `calculate_net_proceeds` to see your final profit after all platform fees are deducted.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/secondhand-value-calculator](https://vinkius.com/mcp/secondhand-value-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Secondhand Value Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `secondhand-value-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Secondhand Value Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "secondhand-value-calculator": {
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
