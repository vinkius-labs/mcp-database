# Invoice Ninja (Invoicing & Billing) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/invoice-ninja-invoicing-billing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage invoicing via Invoice Ninja — create clients, track payments, and manage invoices and balances.

## Description
Connect your **Invoice Ninja** account to any AI agent and take full control of your small business billing and client management through natural conversation.

### What you can do

- **Client Management** — List all registered clients and retrieve detailed CRM data including balances, VAT identifiers, and contact histories directly from your agent
- **Invoice Lifecycle** — Create new invoice drafts, update line items, and manage the transition from 'Draft' to 'Sent' and 'Paid' stages securely
- **Balance Audit** — Fetch full tax math and raw total calculations for specific invoices to verify billing accuracy and financial reporting
- **CRM Operations** — Programmatically create and update client profiles with custom JSON payloads to maintain an accurate business registry
- **Document Cleanup** — Irreversibly delete or archive invoices and client records to maintain clean accounting totals and optimized workspace data
- **Billing Workflow** — Browse through your entire billing system to monitor revenue streams and track outstanding payments in real-time

### How it works

1. Subscribe to this server
2. Enter your Invoice Ninja Domain and API Token
3. Start managing your business billing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Small Business Owners** — monitor outstanding invoices and manage client balances through natural conversation during busy workdays
- **Freelancers** — create and update invoice drafts for clients without leaving your development or design environment
- **Accountants & Ops** — audit invoice line items and tax calculations to ensure financial integrity across the entire billing system


## Available Tools (10)
- **create_client**: Create a new client in InvoiceNinja
- **create_invoice**: Create a new invoice for a client
- **delete_client**: Delete a client from InvoiceNinja
- **update_invoice**: g., from draft to sent). Provide modifications as a JSON string.

Update an existing invoice
- **delete_invoice**: Delete an invoice from InvoiceNinja
- **get_client**: Get complete details of a specific InvoiceNinja client
- **get_invoice**: Get details of a specific invoice
- **list_clients**: List all clients registered in InvoiceNinja
- **list_invoices**: List invoices in InvoiceNinja
- **update_client**: You must provide the fields to update encoded as a JSON string.

Update an existing client in InvoiceNinja


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Invoice Ninja (Invoicing & Billing)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 invoices generated this month"

**🤖 AI Agent:**
> I've retrieved the latest 5 invoices. Highlights include INV-001 ($1,200, Paid), INV-002 ($450, Sent), and INV-003 ($2,100, Draft). Would you like to see the detailed line items for any of these?

---

**👤 You:**
> "Show me the details for client 'TechCorp' (ID: client-987)"

**🤖 AI Agent:**
> Client 'TechCorp' (ID: client-987) has a current balance of $3,500. They have 12 total invoices, with 2 currently outstanding. Their primary contact is sarah@techcorp.com. Would you like to create a new invoice for them?

---

**👤 You:**
> "Create a new client: 'Future Labs' with email 'billing@futurelabs.io'"

**🤖 AI Agent:**
> Client 'Future Labs' created successfully. ID: client-012. You can now generate invoices for this client or update their profile with additional VAT and address information. Would you like to add an address now?


## ❓ FAQ

**Q: Can I create a new invoice draft through my agent?**
Yes. Use the `create_invoice` tool by providing an existing Client ID and a JSON array of line items. Your agent will generate the draft in Invoice Ninja, ready for your final review and sending.

**Q: How do I check a client's outstanding balance?**
The `get_client` tool allows your agent to retrieve complete details for a specific client, including their current balance and payment history. This helps you quickly identify which clients need follow-up on outstanding payments.

**Q: Can my agent list all unpaid invoices?**
Absolutely. Use the `list_invoices` tool to browse your billing system. Your agent can filter through the results to show you which invoices are still in 'Sent' or 'Overdue' status directly through natural conversation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/invoice-ninja-invoicing-billing](https://vinkius.com/mcp/invoice-ninja-invoicing-billing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Invoice Ninja (Invoicing & Billing)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `invoice-ninja-invoicing-billing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Invoice Ninja (Invoicing & Billing)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "invoice-ninja-invoicing-billing": {
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
