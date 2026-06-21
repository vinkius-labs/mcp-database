# Invoicing Plus MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/invoicing-plus)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Create professional invoices and estimates in minutes with a clean interface designed for small businesses and freelancers.

## Description
Connect your **Invoicing Plus** account to any AI agent and manage billing through natural conversation.

### What you can do

- **Invoice Management** — List, create, inspect, and send invoices with line items and tax calculations
- **Client Database** — Browse clients, create new client records, and inspect profiles
- **Payment Tracking** — Monitor payment statuses and track overdue invoices
- **Product Catalog** — Browse products and services with pricing for quick invoice creation
- **Revenue Monitoring** — Track total revenue, outstanding amounts, and payment trends

### How it works

1. Subscribe to this server
2. Enter your Invoicing Plus API Key
3. Start managing invoices from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Freelancers** — create and send invoices without opening the billing app
- **Small Businesses** — manage clients, track payments, and monitor cash flow
- **Accountants** — review invoices and payment statuses through AI


## Available Tools
- **create_customer**: plus with the provided name and email.

Create a new customer in Invoicing.plus
- **get_company**: plus.

Get a specific company from Invoicing.plus
- **get_customer**: plus API.

Get a specific customer from Invoicing.plus
- **get_estimate**: plus API.

Get a specific estimate from Invoicing.plus
- **get_invoice**: plus API.

Get a specific invoice from Invoicing.plus
- **get_item**: plus API.

Get a specific item from Invoicing.plus
- **list_companies**: plus.

List companies from Invoicing.plus
- **list_customers**: plus API.

List customers from Invoicing.plus
- **list_estimates**: plus API.

List estimates from Invoicing.plus
- **list_invoices**: plus API.

List invoices from Invoicing.plus
- **list_items**: plus API.

List items/products from Invoicing.plus
- **list_payments**: plus API.

List payments from Invoicing.plus


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Invoicing Plus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create an invoice for Acme Corp with 3 line items and show all overdue invoices."

**🤖 AI Agent:**
> Invoice created! #INV-2089, Client: Acme Corp. Items: 1) Web Development ($5,000). 2) UI Design ($2,500). 3) QA Testing ($1,200). Subtotal: $8,700. Tax (10%): $870. Total: $9,570. Status: Draft. Overdue invoices: 3 total ($4,250). #INV-2075 — TechCo ($1,800, 15 days overdue). #INV-2080 — StartupXYZ ($1,200, 8 days). #INV-2083 — DesignCo ($1,250, 3 days).

---

**👤 You:**
> "Show all clients and the revenue summary for this month."

**🤖 AI Agent:**
> Clients: 24 total. Top by revenue: Acme Corp ($28K lifetime), TechCo ($15K), StartupXYZ ($8K). This month: Revenue: $18,450 (12 invoices). Paid: $14,200 (77%). Outstanding: $4,250 (3 overdue). Average invoice: $1,537. Compared to last month: +12%.

---

**👤 You:**
> "Browse the product catalog and send the draft invoice to Acme Corp."

**🤖 AI Agent:**
> Product catalog: 12 items. Services: Web Development ($150/hr), UI Design ($120/hr), QA Testing ($80/hr), Consulting ($200/hr). Products: Hosting ($49/mo), SSL ($19/yr), Domain ($12/yr). Invoice #INV-2089 sent! ✅ Delivered to billing@acmecorp.com. Status: Sent. Payment due: May 10, 2025.


## ❓ FAQ

**Q: Can I create and send invoices through the AI agent?**
Yes. Use the invoice creation tools with client ID, line items, and tax settings. Browse products for quick item selection and send invoices directly to clients.

**Q: Can I track overdue invoices and payment status?**
Yes. List invoices with status filters to identify overdue, paid, and pending invoices. Track payment amounts and dates for cash flow monitoring.

**Q: Can I manage my product catalog?**
Yes. Browse all products and services with pricing. Use products directly when creating invoices for quick line item selection.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/invoicing-plus](https://vinkius.com/mcp/invoicing-plus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Invoicing Plus** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `invoicing-plus` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Invoicing Plus** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "invoicing-plus": {
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
