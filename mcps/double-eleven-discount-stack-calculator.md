# Double-Eleven Discount Stack Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/double-eleven-discount-stack-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate exact final prices and optimal spending for 11.11 shopping festivals.

## Description
This MCP server provides precise tools to navigate the complex discount hierarchies of Chinese e-commerce festivals like 11.11. It calculates the final cost by sequentially applying store coupons, platform-wide cross-store thresholds, VIP discounts, and red packets. Use `get_final_price` to find your exact total, `get_threshold_analysis` to determine the optimal add-on amount needed to reach the next discount tier, and `get_savings_comparison` to visualize your total savings.


## Available Tools (3)
- **get_final_price**: 
- **get_savings_comparison**: 
- **get_threshold_analysis**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Double-Eleven Discount Stack Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my final price for a 400 RMB item with a 20 RMB store coupon, a 50 RMB discount for every 300 RMB spent, and a 10% VIP discount?"

**🤖 AI Agent:**
> Your final price is 315.0 RMB.

---

**👤 You:**
> "I have 250 RMB in my cart. How much more do I need to spend to reach the 300 RMB threshold for a 50 RMB discount?"

**🤖 AI Agent:**
> You need to add 50.0 RMB to your cart to reach the next threshold.

---

**👤 You:**
> "Compare the savings for a 500 RMB item with a 50 RMB platform discount (300 threshold) versus no discounts."

**🤖 AI Agent:**
> The original price was 500.0 RMB and your final price is 450.0 RMB, resulting in total savings of 50.0 RMB.


## ❓ FAQ

**Q: How does the discount calculation order work?**
Discounts are applied in a strict sequence: first the store coupon, then the platform cross-store threshold, followed by the VIP discount, and finally the red packet deduction.

**Q: Can I use this to plan my 11.11 shopping cart?**
Yes, you can use `get_threshold_analysis` to see exactly how much more you need to add to your cart to trigger the next platform-wide discount tier.

**Q: What is the difference between a store coupon and a platform threshold?**
A store coupon is specific to a single merchant, while the platform threshold is a cross-store discount applied by the platform for every fixed increment spent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/double-eleven-discount-stack-calculator](https://vinkius.com/ai-agent-connect/double-eleven-discount-stack-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Double-Eleven Discount Stack Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `double-eleven-discount-stack-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Double-Eleven Discount Stack Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "double-eleven-discount-stack-calculator": {
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
