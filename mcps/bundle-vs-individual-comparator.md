# Bundle vs Individual Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bundle-vs-individual-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare bundle discounts against individual coupon stacking to find the best savings.

## Description
This MCP server provides an analytical engine to determine if a multi-item bundle purchase offers better value than buying items separately using their respective stackable coupons. Use `calculate_bundle_cost` to find the total price after a unified discount, `calculate_individual_total` to compute costs with individual coupon arrays (supporting both 'percentage' and 'fixed' modes), and `compare_pricing_strategies` to identify the exact savings difference in cents.


## Available Tools (3)
- **calculate_individual_total**: Determines the total cost of items using individual coupons
- **compare_pricing_strategies**: Compares bundle cost vs individual coupon cost
- **calculate_bundle_cost**: Determines the total cost of items as a bundle


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bundle vs Individual Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the bundle cost for Item A at 1000 cents and Item B at 2000 cents with a 15% discount."

**🤖 AI Agent:**
> The total bundle cost is 2550 cents.

---

**👤 You:**
> "Is it better to buy items separately? Item A: 1000c, Item B: 2000c. Coupons for A: [{'value': 10, 'mode': 'percentage'}]. Coupons for B: [{'value': 100, 'mode': 'fixed'}]."

**🤖 AI Agent:**
> The individual total cost is 2800 cents.

---

**👤 You:**
> "Compare a bundle costing 2550 cents vs an individual total of 2800 cents."

**🤖 AI Agent:**
> Choosing the bundle saves you 250 cents.


## ❓ FAQ

**Q: How does the coupon stacking work?**
The `calculate_individual_total` tool iterates through all provided coupons for each item. It supports both 'percentage' and 'fixed' modes, applying them to the base price while ensuring the final price per item never drops below zero cents.

**Q: Can I compare different discount strategies?**
Yes. You can use `compare_pricing_strategies` by providing the results from `calculate_bundle_cost` and `calculate_individual_total` to see the exact savings difference.

**Q: What precision is used for calculations?**
All financial calculations are processed in cents (integers) to ensure absolute precision and avoid floating-point errors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bundle-vs-individual-comparator](https://vinkius.com/mcp/bundle-vs-individual-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bundle vs Individual Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bundle-vs-individual-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bundle vs Individual Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bundle-vs-individual-comparator": {
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
