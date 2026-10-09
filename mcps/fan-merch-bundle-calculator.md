# Fan Merch Bundle Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fan-merch-bundle-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate merchandise bundle totals, savings, and final prices.

## Description
This MCP server provides tools to manage fan merchandise bundle pricing. It allows for calculating the subtotal of multiple items using `get_subtotal`, determining savings with `calculate_bundle_savings`, and computing the final cost with `calculate_final_bundle_price`. For a complete breakdown of costs and discounts, use `get_bundle_summary`.


## Available Tools (4)
- **calculate_bundle_savings**: Determines the specific dollar amount that will be deducted from a subtotal based on a discount rule
- **calculate_final_bundle_price**: Computes the final amount a customer owes after applying a bundle discount to a subtotal
- **get_bundle_summary**: Provides a complete breakdown of the bundle cost, including the original cost, the savings, and the total due
- **get_subtotal**: Calculates the combined cost of all items in a merchandise selection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fan Merch Bundle Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total for items priced at 10.00, 15.50, and 5.00 with a 10% discount?"

**🤖 AI Agent:**
> The subtotal is 30.50, the discount is 3.05, and the final price is 27.45.

---

**👤 You:**
> "Calculate a bundle with items costing 20.00 and 30.00 using a flat 5.00 discount."

**🤖 AI Agent:**
> The subtotal is 50.00, the discount is 5.00, and the final price is 45.00.

---

**👤 You:**
> "I have items for 12.00 and 8.00. What is the final price with a 20% discount?"

**🤖 AI Agent:**
> The subtotal is 20.00, the discount is 4.00, and the final price is 16.00.


## ❓ FAQ

**Q: How do I calculate the total cost of my items?**
You can use the `get_subtotal` tool to sum up the individual prices of all items in your selection.

**Q: Can I apply both percentage and flat discounts?**
The tools allow you to choose between a 'percentage' or 'flat' discount type when using `calculate_bundle_savings` or `get_bundle_summary`.

**Q: How can I see the full breakdown of my bundle?**
Use the `get_bundle_summary` tool to receive the subtotal, the discount amount, and the final price in a single response.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fan-merch-bundle-calculator](https://vinkius.com/en/ai-agent-connect/fan-merch-bundle-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fan Merch Bundle Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fan-merch-bundle-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fan Merch Bundle Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fan-merch-bundle-calculator": {
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
