# Menu Margin Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/menu-margin-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate food margins, simulate pricing, and analyze menu profitability.

## Description
A specialized financial tool for restaurateurs to manage profitability. Use `calculate_item_margin` to find the profit and cost percentage of a single dish, `simulate_pricing_adjustment` to determine the ideal price for a target cost, `analyze_menu_composition` to view aggregate menu performance, and `evaluate_profitability_threshold` to verify if items meet specific profit requirements.


## Available Tools (4)
- **analyze_menu_composition**: Calculate weighted average cost and margin for a group of items
- **calculate_item_margin**: Calculate the dollar profit and percentage margin for a specific dish
- **evaluate_profitability_threshold**: Check if an item meets minimum profit requirements
- **simulate_pricing_adjustment**: Determine the required menu price to hit a target cost percentage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Menu Margin Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the margin for a burger that costs $5 to make and sells for $15?"

**🤖 AI Agent:**
> The burger has a food margin of $10.00 and a food cost percentage of 33.33%.

---

**👤 You:**
> "I want a 25% food cost for a steak that costs $12.00. What should I charge?"

**🤖 AI Agent:**
> To achieve a 25% food cost, you should charge $48.00, resulting in a $36.00 profit.

---

**👤 You:**
> "Does a dish with a $12 price and $6 cost meet a minimum $7 profit requirement?"

**🤖 AI Agent:**
> No, the item is not profitable because the current margin of $6.00 is below the required $7.00.


## ❓ FAQ

**Q: How do I calculate the margin for a single dish?**
You can use the `calculate_item_margin` tool by providing the menu price and the total ingredient cost.

**Q: Can I simulate how a price change affects my profit?**
Yes, the `simulate_pricing_adjustment` tool allows you to input your ingredient cost and a target cost percentage to find the suggested menu price.

**Q: How can I check if my entire menu is profitable?**
Use the `analyze_menu_composition` tool with a list of your items to see the total revenue, total cost, and weighted average cost percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/menu-margin-calculator](https://vinkius.com/en/ai-agent-connect/menu-margin-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Menu Margin Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `menu-margin-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Menu Margin Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "menu-margin-calculator": {
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
