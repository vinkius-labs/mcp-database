# Online Cart Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/online-cart-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A strategic decision engine for finding the most cost-effective product combinations.

## Description
This MCP server acts as a decision engine to help users maximize their shopping value. It evaluates product combinations against complex constraints including discount coupons, shipping thresholds, and store inventory limits. By using tools like `get_best_cart_combination`, users can identify the optimal set of items that fit within their budget while minimizing shipping costs and maximizing savings. It also provides utility for checking `validate_coupon_eligibility`, `calculate_shipping_cost`, and `check_inventory_compliance` to ensure every cart is both affordable and valid.


## Available Tools (4)
- **check_inventory_compliance**: Ensures a proposed cart does not exceed the allowed quantity for any single product
- **calculate_shipping_cost**: Determines the shipping fee based on the current cart value
- **get_best_cart_combination**: Finds the optimal set of products to maximize user value within all constraints
- **validate_coupon_eligibility**: Checks if a specific coupon can be applied to a specific set of products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Online Cart Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the best combination of products from this list: [{id: 'p1', price: 10, stockLimit: 5}, {id: 'p2', price: 20, stockLimit: 2}] with a budget of 25 and a 5 dollar coupon."

**🤖 AI Agent:**
> The optimal selection is product p2 for a total of 15 dollars after the coupon is applied.

---

**👤 You:**
> "Is the coupon 'SAVE10' valid for a cart containing product p1 (price 15) if the minimum spend is 20?"

**🤖 AI Agent:**
> No, the coupon is not valid because the current cart total is 15, which is below the required 20 minimum spend.

---

**👤 You:**
> "What is the shipping cost for a 40 dollar cart if the free shipping threshold is 50 and the standard fee is 5?"

**🤖 AI Agent:**
> The shipping cost is 5 dollars.


## ❓ FAQ

**Q: How does the optimizer handle coupons?**
The engine evaluates available coupons to find the best combination. You can use `validate_coupon_eligibility` to check if a specific discount applies to your current selection.

**Q: Can I set a maximum budget?**
Yes, the `get_best_cart_combination` tool allows you to specify a `maxBudget` to ensure the final total, including shipping, stays within your limit.

**Q: How is shipping cost calculated?**
Shipping is calculated based on your cart value relative to a threshold. You can use `calculate_shipping_cost` to determine if you have reached the free shipping limit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/online-cart-optimizer](https://vinkius.com/en/ai-agent-connect/online-cart-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Online Cart Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `online-cart-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Online Cart Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "online-cart-optimizer": {
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
