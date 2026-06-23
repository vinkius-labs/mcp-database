# Odoo ERP (Full) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/odoo-erp-full)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage CRM leads, contacts, companies, sales orders, and notes — complete Odoo ERP access through natural conversation.

## Description
Connect **Odoo ERP** to any AI agent — manage your entire business without switching tabs.

### What you can do
- **CRM** — Search and create leads, track opportunities through your pipeline
- **Contacts** — Find individual contacts and companies, create new partners
- **Sales** — List and manage sales orders with full order details
- **Notes** — Add comments and notes to any record in your Odoo instance

### Who is this for?
- **Sales Teams** — CRM pipeline at your fingertips through AI
- **Account Managers** — Quick access to contact and company information
- **Operations** — Monitor sales orders without switching screens
- **Odoo Administrators** — Query any module through natural conversation


## Available Tools (7)
- **odoo_create_contact**: partner record. Set is_company=true to create a company/organization, or false (default) for an individual person. For individuals, you can optionally set parent_id to link them to an existing company. Returns the created partner with its new ID.

Create a new contact (person) or company in Odoo with name, email, phone, and optional parent company
- **odoo_create_lead**: lead. Set type to "lead" for unqualified leads or "opportunity" for qualified prospects already in the pipeline. The name field is the lead title (e.g., "Website Redesign - Acme Corp"). partner_name is the company/organization name. Returns the created record with its new ID.

Create a new CRM lead or opportunity in Odoo with contact details and expected revenue
- **odoo_create_note**: message of type "comment" with subtype "note", which appears in the chatter/history of the specified record. Provide resModel (e.g., "crm.lead", "sale.order", "res.partner") and resId to attach the note to a specific record. If no resModel/resId is given, creates a standalone note. Use when the user wants to log information, add a comment, or leave a note on any Odoo record.

Add a note or internal comment to any Odoo record — leads, contacts, orders, tasks, etc
- **odoo_list_sales_orders**: order records ordered by creation date descending. Returns order number (e.g., S00042), customer name, order state (draft/sent/sale/done/cancel), total amount, assigned salesperson, and order date. Use when the user asks about recent orders, sales activity, or wants a summary of current sales.

List the most recent sales orders in Odoo with customer, amount, and status
- **odoo_search_companies**: partner with is_company=true to find company/organization records. Returns company name, email, phone, website, city, and country. Use when the user asks about a company, organization, or account — distinct from individual contacts.

Search companies and organizations in Odoo by name
- **odoo_search_contacts**: partner with is_company=false to find individual contacts. Returns name, email, phone, city, country, and parent company. Use when the user asks about a person, wants to find contact info, or needs to look up a customer or partner by name.

Search individual contacts (people) in Odoo by name, email, or phone
- **odoo_search_leads**: lead model for leads and opportunities matching the query. Returns id, name, email, phone, pipeline stage, expected revenue, type (lead vs opportunity), and assigned salesperson. Use this when the user wants to find prospects, check pipeline status, or look up a specific lead by name or company.

Search CRM leads and opportunities in Odoo by name, company, or keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Odoo ERP (Full)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for leads from the website"

**🤖 AI Agent:**
> 👥 **CRM Leads — Website**
| Name | Email | Stage | Revenue |
|---|---|---|---|
| Acme Corp | info@acme.com | Qualification | $15,000 |
| Beta Inc | hello@beta.io | Proposition | $8,500 |

---

**👤 You:**
> "Show recent sales orders"

**🤖 AI Agent:**
> 📋 **Sales Orders**
| SO# | Customer | Amount | Status |
|---|---|---|---|
| S00042 | Acme Corp | $12,500 | Confirmed |
| S00041 | Beta Inc | $3,200 | Draft |


## ❓ FAQ

**Q: Which Odoo versions are supported?**
This server uses the JSON-RPC protocol, which is compatible with Odoo 14, 15, 16, 17, and 18. Both Odoo Community and Enterprise editions are supported.

**Q: Does it work with Odoo.com (SaaS)?**
Yes! Works with both Odoo.com hosted instances and self-hosted Odoo servers. Just provide your instance URL and API key.

**Q: How do I generate an API Key?**
Go to Settings → Users → select your user → API Keys tab → New API Key. Give it a descriptive name and copy the generated key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/odoo-erp-full](https://vinkius.com/mcp/odoo-erp-full)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Odoo ERP (Full)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `odoo-erp-full` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Odoo ERP (Full)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "odoo-erp-full": {
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
