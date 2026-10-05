# Moving Sale Pricer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moving-sale-pricer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimize listing prices for residential liquidation sales.

## Description
Moving Sale Pricer is a dynamic pricing engine designed for residential liquidation. It helps users determine the best listing prices by analyzing purchase cost, current market value, item condition, and the urgency of the sale. Use `get_suggested_listing_price` to find the ideal price for a single item, `compare_item_valuation` to check if your profit goals are realistic, `batch_evaluate_inventory` to summarize total potential revenue for a collection of items, or `validate_market_ceiling` to ensure your prices aren't too high for the local market.


## Available Tools (4)
- **compare_item_valuation**: Compares the user's desired target proceeds against the reality of the item's condition and market value to identify "unrealistic" expectations
- **get_suggested_listing_price**: Calculates the optimal listing price for a single item based on all user-provided variables
- **validate_market_ceiling**: Checks if a specific requested price is prohibited by current market realities to prevent "stale" listings
- **batch_evaluate_inventory**: Processes a list of items to provide a summary of total potential revenue and liquidity needs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moving Sale Pricer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I bought a sofa for $500. It's in great condition (0.9) and I need to sell it quickly (urgency 4). What should I list it for?"

**🤖 AI Agent:**
> You should list the sofa for $320.00.

---

**👤 You:**
> "I want to make $100 on a camera I bought for $200. The market value is $150 and it's in mint condition (1.0). Is this realistic?"

**🤖 AI Agent:**
> No, your target is not realistic. The maximum reasonable price is $150.00, leaving a gap of $50.00.

---

**👤 You:**
> "Is a $250 price for a table with a market value of $200 and condition 0.8 viable?"

**🤖 AI Agent:**
> No, the price is not viable. The ceiling price for this item is $160.00.


## ❓ FAQ

**Q: How does the tool calculate my suggested price?**
The engine calculates a price by applying your item's condition score to the original purchase cost and then adjusting for your specific urgency level, ensuring the price never exceeds the current market value.

**Q: Can I check if my target profit is realistic?**
Yes, you can use `compare_item_valuation` to compare your desired proceeds against the item's condition and market reality to see if your goal is achievable.

**Q: How do I evaluate all my items at once?**
You can use `batch_evaluate_inventory` to process a list of items and receive a summary of total potential revenue and a liquidity score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moving-sale-pricer](https://vinkius.com/en/ai-agent-connect/moving-sale-pricer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moving Sale Pricer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moving-sale-pricer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moving Sale Pricer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moving-sale-pricer": {
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
