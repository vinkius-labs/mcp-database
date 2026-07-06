# Evoliz Invoicing & Management MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/evoliz-invoicing-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Equip your AI agent to manage sales invoices, track CRM clients, and monitor quotes via the Evoliz API.

## Description
Integrate **Evoliz**, the powerful cloud-based invoicing and business management platform, directly into your AI workflow. Manage your sales invoices and quotes, track client profiles and financial summaries, monitor product catalogs and supplier records, and oversee your entire business operation using natural language.

### What you can do

- **Invoicing Oversight** — List and retrieve detailed information, line items, and payment status for all your sales invoices.
- **Client Intelligence** — Monitor CRM client profiles and financial summaries, resolving billing details and document history.
- **Quote Management** — Access and monitor sales quotes and estimates, tracking validation statuses and total amounts.
- **Financial Auditing** — Retrieve high-level summaries of document volume, overdue invoices, and organizational business health instantly.

### How it works

1. Connect the Evoliz integration to your AI assistant.
2. Authorize using your Evoliz API Public Key and Secret Key (found in your account settings).
3. Orchestrate your business management and invoicing strategy through intuitive conversation.

### Who is this for?

- **Business Owners & CFOs** — Quickly check revenue totals and overdue invoices on the go.
- **Sales Teams** — Research client history and quote statuses via chat during negotiations.
- **Operations Teams** — Monitor product availability and organizational financial metadata instantly.


## Available Tools (10)
- **list_crm_clients**: List all clients registered in your organization
- **list_sales_invoices**: List all sales invoices in your Evoliz account
- **list_unpaid_overdue_invoices**: Identify invoices that are currently past their due date
- **list_product_catalog**: List all products and services available in your catalog
- **list_sales_quotes**: List all sales quotes and estimates
- **list_authorized_suppliers**: List all authorized suppliers and vendors
- **get_evoliz_account_metadata**: Retrieve metadata and limits for your Evoliz account
- **get_client_detailed_profile**: Get detailed profile and financial summary for a specific client
- **get_invoice_detailed_data**: Get detailed settings and line items for a specific invoice
- **quick_financial_volume_audit**: Retrieve a high-level summary of invoices and quotes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Evoliz Invoicing & Management** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all overdue invoices."

**🤖 AI Agent:**
> I've found 5 overdue invoices totaling 12,500 €. The largest is from 'Global Tech' (4,500 €, 15 days late). Would you like the contact details for Global Tech to send a reminder?

---

**👤 You:**
> "Show me the details for invoice ID 12345."

**🤖 AI Agent:**
> Invoice #12345 (Client: John Doe) is for 1,250 € and is currently 'Paid'. It includes 3 line items: 'Consulting Services', 'Software License', and 'Implementation'. Should I pull the payment timestamp?

---

**👤 You:**
> "Search for client 'Sarah Connor'."

**🤖 AI Agent:**
> Sarah Connor (Client ID: 998877) has 3 active quotes and 2 paid invoices. Their total lifetime value is 8,500 €. Current status is 'Active'. Would you like to see the details for their most recent quote?


## ❓ FAQ

**Q: How do I get Evoliz API credentials?**
Log in to your Evoliz account, navigate to **Apps > API**, and you can generate your unique **Public Key** and **Secret Key** there. Ensure your user has the necessary permissions for API usage.

**Q: Does the integration support overdue tracking?**
Yes, you can use the list_unpaid_overdue_invoices tool to instantly identify all sales invoices that are past their due date.

**Q: Can the agent create new invoices?**
This integration currently focuses on listing and auditing invoices, quotes, and clients. Creating or converting quotes to invoices should be managed via the Evoliz web interface or mobile app to ensure proper accounting compliance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/evoliz-invoicing-management](https://vinkius.com/mcp/evoliz-invoicing-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Evoliz Invoicing & Management** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `evoliz-invoicing-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Evoliz Invoicing & Management** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "evoliz-invoicing-management": {
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
