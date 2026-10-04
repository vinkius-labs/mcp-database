# Coupon Bundle Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/coupon-bundle-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Finds the cheapest way to buy items using unit prices, bundles, and coupons.

## Description
This MCP server provides an optimization engine to determine the most cost-effective way to fulfill a required quantity of items. It evaluates unit prices, package sizes, coupons, percentage discounts, and bundle constraints to minimize total spend. Use `get_best_purchase_plan` to find the optimal combination of products and packages, or `validate_coupon_eligibility` to check if a specific discount applies to your selection.


## Available Tools (4)
- **calculate_item_surplus**: Determines how many extra units were acquired beyond the target requirement
- **get_best_purchase_plan**: Finds the single cheapest combination of purchases to satisfy the target quantities
- **simulate_single_option_cost**: Calculates the cost of a specific single purchase before global optimization
- **validate_coupon_eligibility**: Checks if a specific coupon can be applied to a proposed selection of items or packages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coupon Bundle Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the cheapest way to get 10 units of Item A if they are $2 each, or available in a pack of 6 for $10, with a $2 coupon for any pack?"

**🤖 AI Agent:**
> The cheapest way is to buy one pack of 6 for $8 (after the $2 coupon) and 4 individual units at $2 each, for a total of $16.

---

**👤 You:**
> "I need 5 units of Item B. Item B costs $5 individually. There is a bundle of 3 for $12. What is my best plan?"

**🤖 AI Agent:**
> The best plan is to buy one bundle of 3 for $12 and 2 individual units for $10, totaling $22.

---

**👤 You:**
> "Check if a $5 off coupon is valid for a $20 purchase of Item C."

**🤖 AI Agent:**
> The coupon is valid for this purchase.


## ❓ FAQ

**Q: How does the optimization work?**
The engine calculates every valid combination of individual units and packages, applying all applicable coupons and bundle rules to find the lowest total price.

**Q: What happens if I buy more items than needed?**
If a package contains more units than your target quantity, the extra units are tracked as surplus using the `calculate_item_surplus` tool.

**Q: Can I check if a specific coupon is valid for my items?**
Yes, you can use the `validate_coupon_eligibility` tool to verify if a proposed selection of items meets the requirements of a specific coupon.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/coupon-bundle-comparator](https://vinkius.com/en/ai-agent-connect/coupon-bundle-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coupon Bundle Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coupon-bundle-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coupon Bundle Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coupon-bundle-comparator": {
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
