# Discount Stack Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/discount-stack-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate final transaction totals by compounding multiple discount types and applying regional tax logic.

## Description
The Discount Stack Calculator is a specialized pricing engine designed to handle complex retail promotions. It accurately calculates final prices by managing multiple discount layers, including sequential percentage stacking, fixed currency reductions, and threshold-based incentives. The engine also processes BOGO (Buy One Get One) logic and handles regional taxation complexities, such as whether tax should be applied to the pre-discount or post-discount subtotal. Use `percentage_stacking` to compound rates, `fixed_reduction` for coupons, `threshold_incentive` for spend-based rewards, `bogo_logic` for quantity promotions, and `regional_taxation` for final tax calculations.


## Available Tools (5)
- **bogo_logic**: Calculate BOGO promotion impact
- **fixed_reduction**: Apply fixed currency reductions
- **percentage_stacking**: g., [20, 10] for 20% then 10%). Returns the new subtotal and total savings percentage.

Apply multiple percentage discounts sequentially
- **regional_taxation**: Calculate final price with regional taxes
- **threshold_incentive**: Evaluate spend-based discount eligibility


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Discount Stack Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have an item priced at $100. I have a 20% discount and then a 10% coupon. What is the final subtotal?"

**🤖 AI Agent:**
> $72.00

---

**👤 You:**
> "Calculate the total cost for 5 units of a $10 item using 'buy_one_get_one_free' logic."

**🤖 AI Agent:**
> $30.00 (2 items were free, 3 units at full price)

---

**👤 You:**
> "If my subtotal is $50 and the tax rate is 8% using post_discount mode, what is the grand total?"

**🤖 AI Agent:**
> $54.00


## ❓ FAQ

**Q: How does percentage stacking work?**
The engine uses a multiplicative approach. For example, applying a 20% discount followed by a 10% discount results in an effective total reduction of 28%, not 30%. Use the `percentage_stacking` tool to calculate this accurately.

**Q: Can I calculate taxes for different regions?**
Yes. The `regional_taxation` tool allows you to specify whether tax should be applied using 'pre_discount' or 'post_discount' logic, accommodating both US and European VAT standards.

**Q: Does it support BOGO promotions?**
Yes, the `bogo_logic` tool handles patterns like 'buy_one_get_one_free' and 'buy_two_get_one_free', calculating exactly how many units are at full price and the total savings achieved.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/discount-stack-calculator](https://vinkius.com/mcp/discount-stack-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Discount Stack Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `discount-stack-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Discount Stack Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "discount-stack-calculator": {
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
