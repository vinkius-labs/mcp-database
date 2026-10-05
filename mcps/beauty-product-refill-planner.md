# Beauty Product Refill Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/beauty-product-refill-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Schedules beauty product repurchases based on consumption and stock.

## Description
This MCP server provides a precision scheduling engine for beauty product replenishment. It connects your AI assistant to your inventory data to calculate optimal repurchase dates, predict how changes in usage frequency affect your supply, and optimize bulk orders. Use `get_stock_status` to monitor current inventory, `calculate_refill_schedule` to find the perfect order date, `predict_usage_trends` to model usage changes, and `optimize_bulk_order` to determine the best package size for your needs.


## Available Tools (4)
- **get_stock_status**: Answers how much product is left and when it will run out
- **optimize_bulk_order**: Recommends package size for a target supply duration
- **predict_usage_trends**: Predicts how usage changes with frequency adjustments
- **calculate_refill_schedule**: Calculates the optimal date to place a new order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beauty Product Refill Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much of my moisturizer is left and when will I run out?"

**🤖 AI Agent:**
> You have 15ml of moisturizer remaining, which provides approximately 10 days of supply. Your stock is currently low.

---

**👤 You:**
> "When should I order my next bottle of cleanser to avoid running out?"

**🤖 AI Agent:**
> You should place your order by October 12th, 2024, to ensure your new bottle arrives before you run out of your current supply.

---

**👤 You:**
> "What happens to my supply if I start using my serum twice a day instead of once?"

**🤖 AI Agent:**
> Increasing your usage frequency by 2x will reduce your estimated days of supply from 30 days down to 15 days.


## ❓ FAQ

**Q: How does the refill schedule work?**
The `calculate_refill_schedule` tool calculates a target order date by accounting for your current stock, the product's consumption rate, and the delivery lead time, ensuring you order just before you run out.

**Q: Can I predict how much more product I will need if I use it more often?**
Yes, you can use `predict_usage_trends` to see how increasing or decreasing your usage frequency will impact your remaining days of supply.

**Q: How do I know if I am running low on a product?**
You can use `get_stock_status` to check your current remaining amount and see if your stock has fallen below the safe threshold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/beauty-product-refill-planner](https://vinkius.com/en/ai-agent-connect/beauty-product-refill-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Beauty Product Refill Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `beauty-product-refill-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Beauty Product Refill Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "beauty-product-refill-planner": {
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
