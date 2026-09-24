# Supplier Order Total Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/supplier-order-total-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate order subtotals, taxes, and discounts for supplier orders.

## Description
This MCP server provides a specialized calculation engine for managing supplier order finances. It allows AI agents to accurately compute order subtotals using `calculate_order_subtotal`, apply various discount types with `apply_order_discounts`, and determine tax obligations via `calculate_tax_liability`. For a complete financial overview, use `generate_order_summary` to get a full breakdown of subtotals, taxes, and discounts in one call. It is designed to ensure mathematical integrity for purchase orders and tax compliance.


## Available Tools (4)
- **apply_order_discounts**: Calculate the new total after applying specific discount rules
- **calculate_order_subtotal**: Calculate the total cost of all items before taxes and discounts
- **calculate_tax_liability**: You may also provide an optional global tax rate.

Calculate the total tax owed based on provided tax rates
- **generate_order_summary**: Generate a complete financial breakdown of the order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Supplier Order Total Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the subtotal for 2 items at $15.00 each and 3 items at $10.00 each?"

**🤖 AI Agent:**
> The subtotal is $60.00.

---

**👤 You:**
> "Apply a 10% discount to a subtotal of $100.00."

**🤖 AI Agent:**
> The discounted total is $90.00.

---

**👤 You:**
> "Give me a full summary for 1 item costing $50.00 with a 5% tax rate."

**🤖 AI Agent:**
> The order summary is: Subtotal: $50.00, Total Tax: $2.50, Final Total: $52.50.


## ❓ FAQ

**Q: How do I calculate the subtotal of an order?**
You can use the `calculate_order_subtotal` tool by providing a list of order lines containing quantities and unit prices.

**Q: Can I apply both flat and percentage discounts?**
The `apply_order_discounts` tool supports both 'flat' and 'percentage' discount types to adjust your totals.

**Q: How are taxes handled for different items?**
The `calculate_tax_liability` tool allows you to specify individual tax rates per item or provide a global tax rate to apply to all items.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/supplier-order-total-calculator](https://vinkius.com/en/ai-agent-connect/supplier-order-total-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Supplier Order Total Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `supplier-order-total-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Supplier Order Total Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "supplier-order-total-calculator": {
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
