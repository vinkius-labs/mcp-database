# SimpleFatoora MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/simplefatoora)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Connect your AI agents to SimpleFatoora for ZATCA-compliant e-invoicing with full product, customer, and tax document management.

## Description
Empower your AI agents to completely automate your billing and tax operations using the SimpleFatoora platform. With 20 dedicated tools, your AI can now programmatically generate all six ZATCA-compliant invoice types, validate tax compliance, manage customer and product catalogs, and issue credit notes directly from your natural language interface.

### What you can do
- Create ZATCA Phase 2 compliant invoices (B2C, B2B, Purchase)
- Issue compliant credit and debit notes automatically
- Manage product catalogs and VAT rates with full CRUD
- Maintain customer profiles and tax registration numbers
- Verify API keys and cryptographic stamps
- Perform compliance verification checks

### How it works
1. Subscribe to this server
2. Enter your SimpleFatoora API Key (found in your developer dashboard)
3. Start managing your Saudi e-invoicing operations directly via Vinkius

### Who is it for?
Perfect for financial controllers, accountants, and businesses operating in Saudi Arabia that require strict ZATCA e-invoicing compliance combined with AI automation.


## Available Tools (20)
- **check_simplefatoora_status**: Verify connectivity
- **create_credit_note**: Create credit note
- **create_customer**: Create a customer
- **create_debit_note**: Create debit note
- **create_product**: Create a product
- **create_simplified_purchase**: Create simplified purchase invoice
- **create_simplified_invoice**: Create B2C invoice
- **create_standard_purchase**: Create standard purchase invoice
- **create_vat_invoice**: Create B2B VAT invoice
- **delete_customer**: Delete a customer
- **delete_product**: Delete a product
- **get_customer**: Get customer details
- **get_invoice**: Get invoice details
- **get_product**: Get product details
- **list_customers**: List customers
- **list_invoices**: List all invoices
- **list_products**: List products
- **update_customer**: Update a customer
- **update_product**: Update a product
- **validate_api_key**: Validate API key


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SimpleFatoora** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a simplified B2C invoice for 3 items totaling 450 SAR in SimpleFatoora."

**🤖 AI Agent:**
> I've successfully created the simplified B2C invoice. The total is 450 SAR, including VAT. The ZATCA-compliant invoice with its cryptographic QR code has been generated. Would you like me to send it to the customer?

---

**👤 You:**
> "List all customers in SimpleFatoora with their VAT registration numbers."

**🤖 AI Agent:**
> Retrieving your customer list... You currently have 42 registered customers. I have compiled their names and VAT registration numbers. Would you like to export this list as a CSV file?

---

**👤 You:**
> "Create a credit note for invoice #1234 in SimpleFatoora due to a partial return."

**🤖 AI Agent:**
> Credit note successfully created and linked to invoice #1234. The adjustment for the partial return has been recorded and stamped for ZATCA Phase 2 compliance. Do you need to apply this credit to the customer's balance?


## ❓ FAQ

**Q: How can my AI generate ZATCA-compliant invoices?**
Simply use the `create_invoice` tool. Your agent can instantly generate six types of invoices (including B2C and B2B), all fully compliant with ZATCA Phase 2, complete with QR codes, UUIDs, and cryptographic stamps.

**Q: Is it possible to programmatically access my client list and VAT numbers?**
Yes. By executing the `list_customers` action, your AI agent can retrieve your entire client registry, including tax identification numbers, addresses, and contact details for seamless CRM integration.

**Q: Can I automatically issue credit notes for partial returns?**
Absolutely. Ask the agent to use the `create_credit_note` tool. It will safely generate a ZATCA-compliant credit note linked to the original invoice, adjusting the accounting records automatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simplefatoora](https://vinkius.com/mcp/simplefatoora)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SimpleFatoora** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `simplefatoora` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SimpleFatoora** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "simplefatoora": {
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
