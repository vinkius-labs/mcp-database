# Beauty Basket Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/beauty-basket-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate beauty product prices, subtotals, and regional taxes.

## Description
This MCP server provides tools to manage beauty product pricing and basket calculations. Use `get_product_price` to find individual item costs, `calculate_basket_subtotal` for pre-tax sums, `calculate_regional_tax` for location-based taxes, or `get_basket_summary` for a complete financial breakdown including subtotal, tax, and grand total.


## Available Tools (4)
- **calculate_basket_subtotal**: Calculates the sum of all product prices in a basket before tax
- **calculate_regional_tax**: Determines the tax amount applicable to a subtotal based on the user's location
- **get_basket_summary**: Provides a complete breakdown of a shopping basket, including subtotal, tax, and the final grand total
- **get_product_price**: Retrieves the unit price for a specific product based on its tier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beauty Basket Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much does product B001 cost in the Premium tier?"

**🤖 AI Agent:**
> The unit price for product B001 in the Premium tier is $45.00.

---

**👤 You:**
> "Calculate the subtotal for 2 units of B001 and 1 unit of B002."

**🤖 AI Agent:**
> The subtotal for your items is $110.00.

---

**👤 You:**
> "Give me a summary for 3 units of B001 in the USA."

**🤖 AI Agent:**
> Subtotal: $135.00, Tax: $11.48, Grand Total: $146.48.


## ❓ FAQ

**Q: How do I check the price of a specific item?**
You can use the `get_product_price` tool by providing the product code and the desired tier (Standard, Premium, or Luxury).

**Q: Can I calculate the total cost including tax?**
Yes, the `get_basket_summary` tool provides a full breakdown including the subtotal, the applied tax, and the final grand total for your region.

**Q: Which regions are supported for tax calculation?**
Currently, the system supports tax calculations for the USA and Europe.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/beauty-basket-total](https://vinkius.com/en/ai-agent-connect/beauty-basket-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Beauty Basket Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `beauty-basket-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Beauty Basket Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "beauty-basket-total": {
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
