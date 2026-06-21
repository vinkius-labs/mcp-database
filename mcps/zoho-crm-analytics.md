# Zoho CRM Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-crm-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access custom views, organization info, module metadata, fields, and pipeline analysis in Zoho CRM.

## Description
Connect **Zoho CRM** to any AI agent — manage your entire CRM without switching tabs.

### What you can do
- **Leads** — Search and create leads with source and status tracking
- **Contacts** — Find and create contacts linked to accounts
- **Accounts** — Search companies and organizations
- **Deals** — Search, create, and track deals through pipeline stages
- **Notes** — Create notes attached to any CRM record
- **Generic List** — Query any Zoho CRM module directly

### Who is this for?
- **Sales Reps** — CRM at your fingertips through AI
- **BDRs** — Quickly qualify and create leads
- **Sales Managers** — Pipeline visibility and deal insights
- **Support Teams** — Access contact and account data seamlessly


## Available Tools
- **zoho_module_fields**: Returns field name, display label, data type (text/number/date/picklist/lookup), whether it is required, read-only, and formula-based. Essential for understanding the data model before creating or updating records. Use when the user asks "what fields are on Contacts?" or needs to know valid field names for API operations.

Get all fields (properties) configured on a Zoho CRM module with data types, validation rules, and edit permissions
- **zoho_org_info**: Returns company name, Zoho CRM edition (Free/Standard/Professional/Enterprise/Ultimate), default timezone, currency, and admin contact. Use when the user needs account-level information, subscription details, or org configuration.

Get Zoho CRM organization details — company name, subscription edition, timezone, currency, and license information
- **zoho_custom_views**: Returns view name, system name, category (shared/personal), and whether it is the default. Custom views are saved filters that define how records appear in the module list view (e.g., "All Open Deals", "My Contacts", "Unread Leads"). Use when the user asks about available filters, saved views, or list configurations.

List saved custom views/filters for a Zoho CRM module — predefined list views like "My Open Deals" or "All Leads"
- **zoho_list_modules**: Returns module name, plural label, API name, whether the module supports API access, and visibility status. Modules include: Leads, Contacts, Accounts, Deals, Tasks, Events, Calls, Notes, Products, Quotes, Sales_Orders, Invoices, Purchase_Orders, and custom modules. Use to discover the data model or verify which modules are available.

List all available CRM modules in Zoho with their names, API support status, and whether they are visible
- **zoho_list_pipelines**: For deals: shows sales pipeline stages with associated win probability percentages (e.g., Qualification=10%, Proposal=75%, Closed Won=100%). Returns pipeline name, stage names, stage IDs, and probabilities. Use to understand the sales process, find stage names for deal operations, or check pipeline configuration.

List deal (or custom module) pipelines in Zoho CRM with their stages, win probabilities, and display order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho CRM Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for leads from web form"

**🤖 AI Agent:**
> 👥 **Leads from Web Form**
| Name | Email | Company | Status |
|---|---|---|---|
| John Smith | john@acme.com | Acme Corp | New |
| Maria Garcia | maria@beta.io | Beta Inc | Contacted |

---

**👤 You:**
> "Create a deal: Enterprise Plan $25,000"

**🤖 AI Agent:**
> ✅ **Deal Created!**
- Name: Enterprise Plan
- Amount: $25,000
- Stage: Qualification
- Closing: 2024-03-30


## ❓ FAQ

**Q: What Zoho CRM data can I access?**
Leads, Contacts, Accounts, Deals, Notes, and any custom module. All data respects your Zoho CRM permissions.

**Q: How does authentication work?**
Uses Zoho OAuth 2.0 with a refresh token. Create a Self Client in the Zoho API Console, generate a refresh token, and provide Client ID, Client Secret, and Refresh Token.

**Q: Does it support multi-region Zoho?**
Yes! Set your API domain: zohoapis.com (US), zohoapis.eu (EU), zohoapis.in (India), zohoapis.com.au (Australia), zohoapis.jp (Japan).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-crm-analytics](https://vinkius.com/mcp/zoho-crm-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zoho CRM Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zoho-crm-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho CRM Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-crm-analytics": {
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
