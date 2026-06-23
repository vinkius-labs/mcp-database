# Coupa MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coupa)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage purchase orders, invoices, suppliers, and procurement workflows on Coupa — the enterprise procurement platform.

## Description
Connect your **Coupa** instance to any AI agent and manage procurement operations through natural conversation.

### What you can do

- **Purchase Orders** — Create, approve, and query POs with line-item detail, status tracking, and budget validation
- **Supplier Management** — Search and manage supplier records, compliance status, and performance scorecards
- **Invoices** — Process, query, and match invoices against POs with tolerance checks
- **Requisitions** — Submit and track purchase requisitions through approval chains
- **Contracts** — Query contract terms, expiration dates, and spend against contract limits
- **Expense Reports** — View and approve employee expense submissions
- **Budgets** — Check budget availability and spend analytics by cost center or department

### How it works

1. Subscribe to this server
2. Enter your Coupa instance URL and OAuth 2.0 credentials
3. Start managing procurement through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Procurement Officers** — create POs and manage supplier relationships through chat
- **AP Teams** — process and match invoices without navigating the Coupa UI
- **Finance Controllers** — monitor budget utilization and spend analytics by conversation
- **Category Managers** — query contracts and supplier performance scorecards rapidly


## Available Tools (10)
- **approve_purchase_order**: Touches workflow and authorization boundary states.

Approve a pending purchase order
- **create_purchase_order**: Resolves supplier links, line items, and accounting allocations from the provided JSON payload.

Create a new purchase order
- **get_purchase_order**: Touches financial, supplier, and shipping boundary data.

Get details for a specific purchase order
- **get_supplier_details**: Get full profile for a specific supplier
- **list_contracts**: Resolves contract terms, validity periods, and associated suppliers.

List active procurement contracts
- **list_invoices**: Resolves invoice numbers, vendor names, payment statuses, and due dates.

List invoices and their payment status
- **list_purchase_orders**: Resolves PO numbers, supplier names, total amounts, and statuses (e.g., draft, ordered).

List purchase orders
- **list_requisitions**: Resolves requestor names, requested items, and current approval step in the workflow.

List purchase requisitions and their approval state
- **list_suppliers**: Resolves supplier legal names, tax IDs, contact information, and payment terms.

List or search for suppliers
- **query_coupa_resource**: Resolves raw JSON data from the specified API boundary.

Access any Coupa REST API resource directly


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coupa** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all pending POs above $25K for the IT department."

**🤖 AI Agent:**
> Found 6 pending POs for IT > $25K. Top items: 1. PO-2026-4501 — 'Annual Cloud Licensing' ($180,000), 2. PO-2026-4512 — 'Network Equipment Refresh' ($67,500). Total pending: $412,000. Want me to approve any?

---

**👤 You:**
> "Check the compliance status of supplier Acme Corp."

**🤖 AI Agent:**
> Acme Corp (ID: SUP-1045): Compliance Status: Approved ✅. Tax forms: W-9 on file (exp: Dec 2026). Insurance: Current. Diversity cert: Minority-owned (NMSDC). Performance score: 4.2/5 (last 12 months). All documents are up to date.

---

**👤 You:**
> "What's the remaining budget for Marketing Q2 2026?"

**🤖 AI Agent:**
> Marketing Q2 2026 Budget: Total allocated: $450,000. Committed (POs): $285,000. Spent (invoiced): $210,000. Remaining: $165,000 (36.7%). You have 3 pending requisitions totaling $42,000 awaiting approval.


## ❓ FAQ

**Q: What authentication does Coupa use?**
Coupa supports OAuth 2.0 Client Credentials. You create an OAuth client in Setup > Integrations > OAuth2/OpenID Connect Clients, which generates a Client ID and Client Secret.

**Q: Can I create purchase orders through the agent?**
Yes. The create_purchase_order tool posts to the /api/purchase_orders endpoint. Provide supplier, ship-to, currency, and line items with quantities and prices.

**Q: Does it support invoice matching?**
Yes. The query_invoices tool retrieves invoices with their PO match status, tolerance flags, and approval state.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coupa](https://vinkius.com/mcp/coupa)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coupa** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coupa` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coupa** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coupa": {
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
