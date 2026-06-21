# Zoho Books MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-books)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage invoices, estimates, and contacts via the Zoho Books API.

## Description
Connect your **Zoho Books** account to any AI agent to streamline your cloud accounting and billing operations. This MCP server enables your agent to interact with invoices, estimates, and customer contacts directly from natural language interfaces.

### What you can do

- **Invoicing Management** — List, retrieve, and create professional billing invoices for your clients
- **Estimate Tracking** — Access all quotes and proposals generated for your businesses to stay on top of sales
- **Inventory Visibility** — List the catalog of products and services sold across your organizations
- **Contact Oversight** — Manage customer and vendor profiles and retrieve their details instantly
- **Multi-Org Support** — List all businesses associated with your account and manage data by organization ID

### How it works

1. Subscribe to this server
2. Enter your Zoho Client ID, Client Secret, and Data Center Domain
3. Start managing your accounting from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Small Business Owners** — Quickly check invoice statuses and client balances via natural language commands
- **Accountants & Bookkeepers** — Automate the retrieval of financial records and maintain contact hygiene
- **Developers** — Integrate accounting data and billing automation into your daily development workflow


## Available Tools (7)
- **list_books_contacts**: List all contacts (customers/vendors)
- **create_new_invoice**: Requires a JSON body with invoice details.

Create a new invoice
- **list_estimates**: List all estimates (quotes) for an organization
- **get_invoice_details**: Get details for a specific invoice
- **list_invoices**: List all invoices for an organization
- **list_inventory_items**: List all items (products/services)
- **list_organizations**: Use this to identify the organization ID for other calls.

List all Zoho Books organizations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho Books** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all organizations in my Zoho Books account."

**🤖 AI Agent:**
> I've retrieved your organizations. You have 2 entities: 'Acme Corp (ID: 123456)' and 'Global Services (ID: 789012)'. Which one would you like to manage?

---

**👤 You:**
> "Show the latest invoices for organization ID '123456'."

**🤖 AI Agent:**
> For organization 123456, I found 5 recent invoices. The latest is INV-001 for $1,200.00, currently marked as 'Sent'. Would you like to see the line items?

---

**👤 You:**
> "List my items in organization '123456'."

**🤖 AI Agent:**
> I've retrieved 10 items for your organization, including 'Web Design Service' ($150/hr), 'Cloud Hosting' ($25/mo), and 'Consulting Package' ($500).


## ❓ FAQ

**Q: How do I find my Organization ID?**
Use the `list_organizations` tool to retrieve all businesses registered in your account along with their unique IDs.

**Q: Which Data Center domains are supported?**
You can use Zoho domains such as `com` (US), `eu` (Europe), `in` (India), `com.au` (Australia), or `jp` (Japan).

**Q: Is it possible to create an invoice directly via the agent?**
Yes, use the `create_new_invoice` tool by providing the Organization ID and a JSON object containing the invoice details and line items.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-books](https://vinkius.com/mcp/zoho-books)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zoho Books** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zoho-books` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho Books** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-books": {
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
