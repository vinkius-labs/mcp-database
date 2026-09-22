# Invoice Total Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/invoice-total-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise invoice line totals, subtotals, and grand totals with tax and discounts.

## Description
This MCP server provides specialized tools for financial invoice calculations. It allows AI agents to compute individual line item totals using `calculate_line_item`, aggregate item sums with `calculate_invoice_subtotal`, apply global fiscal adjustments via `apply_global_adjustments`, or generate a complete financial breakdown using `get_invoice_summary`. It handles complex relationships between quantity, unit price, tax rates, and discounts to ensure accurate grand totals.


## Available Tools (4)
- **apply_global_adjustments**: Applies a single discount or tax rate to an existing subtotal
- **calculate_line_item**: Calculates the total for a single specific item within an invoice
- **calculate_invoice_subtotal**: Calculates the sum of all items before taxes and global discounts
- **get_invoice_summary**: Provides a complete breakdown of an entire invoice including all calculations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Invoice Total Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total for 5 units of a product costing $10.00 each with a 5% tax."

**🤖 AI Agent:**
> The total for 5 units at $10.00 each with a 5% tax is $52.50.

---

**👤 You:**
> "What is the subtotal for an invoice with two items: 2 items at $50.00 and 3 items at $20.00?"

**🤖 AI Agent:**
> The subtotal for the invoice is $160.00.

---

**👤 You:**
> "Apply a 10% discount and a 5% tax to a subtotal of $200.00."

**🤖 AI Agent:**
> After a 10% discount and a 5% tax, the grand total is $189.00.


## ❓ FAQ

**Q: How do I calculate a single item's total?**
You can use the `calculate_line_item` tool by providing the quantity and unit price, along with any specific tax or discount amounts.

**Q: Can I apply a tax to the entire invoice?**
Yes, use `apply_global_adjustments` to add a tax percentage to an existing subtotal.

**Q: What is the best tool for a full invoice breakdown?**
The `get_invoice_summary` tool is designed to provide a complete breakdown, including line items, subtotal, discounts, taxes, and the grand total.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/invoice-total-calculator](https://vinkius.com/en/ai-agent-connect/invoice-total-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Invoice Total Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `invoice-total-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Invoice Total Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "invoice-total-calculator": {
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
