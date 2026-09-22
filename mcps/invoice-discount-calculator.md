# Invoice Discount Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/invoice-discount-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise invoice totals, discount breakdowns, and bulk invoice processing.

## Description
This MCP server provides precise financial tools for managing invoice discounts. Use `calculate_discount_details` to get a full breakdown of savings and final totals, or `validate_discount_eligibility` to check if a discount meets business limits. For high-volume tasks, `get_bulk_invoice_totals` processes multiple invoices at once, while `apply_flat_fee_after_discount` handles final totals that include post-discount service fees.


## Available Tools (4)
- **apply_flat_fee_after_discount**: Calculates a final total when a fixed service fee must be added to the discounted amount
- **calculate_discount_details**: Provides a full breakdown of the discount application, including the amount saved and the final total
- **get_bulk_invoice_totals**: Pass a JSON string of invoice objects.

Processes multiple subtotal and discount pairs to return a list of calculated totals
- **validate_discount_eligibility**: Checks if a specific discount percentage is within allowed business limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Invoice Discount Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the discount details for a subtotal of 100 with a 15% discount."

**🤖 AI Agent:**
> The subtotal is 100, the discount amount is 15, and the final total is 85.

---

**👤 You:**
> "Is a 25% discount eligible?"

**🤖 AI Agent:**
> The discount is eligible if it does not exceed the maximum allowed limit.

---

**👤 You:**
> "What is the total for a 200 subtotal with a 10% discount and a 5 service fee?"

**🤖 AI Agent:**
> The final total including the service fee is 185.


## ❓ FAQ

**Q: How do I calculate a single invoice discount?**
You can use the `calculate_discount_details` tool by providing the subtotal and the discount percentage.

**Q: Can I process multiple invoices at once?**
Yes, use the `get_bulk_invoice_totals` tool to process a list of invoice objects.

**Q: How are service fees handled?**
Use `apply_flat_fee_after_discount` to apply a discount first and then add a fixed service fee to the result.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/invoice-discount-calculator](https://vinkius.com/en/ai-agent-connect/invoice-discount-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Invoice Discount Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `invoice-discount-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Invoice Discount Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "invoice-discount-calculator": {
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
