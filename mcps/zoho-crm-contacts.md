# Zoho CRM Contacts MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-crm-contacts)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Search, create, and manage contacts, leads, and accounts — with lead conversion and related records in Zoho CRM.

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


## Available Tools (11)
- **zoho_convert_lead**: This is the standard sales qualification workflow in Zoho CRM. The lead is removed from the Leads module and data transfers to the new records. Use when a lead is qualified and ready to enter the sales pipeline.

Convert a qualified Zoho CRM lead into a Contact + Account + Deal — the key sales qualification step
- **zoho_create_account**: Account_Name is required. Industry should match Zoho industry picklist values. Once created, contacts and deals can be linked to this account.

Create a new account (company/organization) in Zoho CRM with name, industry, phone, and website
- **zoho_create_contact**: Last_Name is required. Account_Name links the contact to a company account. Use for adding qualified individuals — not raw leads (use zoho_create_lead for unqualified prospects).

Create a new contact in Zoho CRM with name, email, phone, and linked account for customer management
- **zoho_create_lead**: Last_Name is required. Use for new, unqualified prospects. Lead_Source: Web Download, Advertisement, Cold Call, Employee Referral, External Referral, Partner, Conference, Trade Show. Once qualified, convert using zoho_convert_lead.

Create a new lead (unqualified prospect) in Zoho CRM with name, email, company, and lead source
- **zoho_get_account**: Returns account name, industry, annual revenue, employees, billing/shipping address, and all custom fields. Use after searching to get full company details.

Get complete details of a specific Zoho CRM account by ID, including industry, revenue, and linked records
- **zoho_get_contact**: Returns full data: name, emails, phones, account, department, title, mailing address, and custom fields. Use after searching to drill into contact details.

Get complete details of a specific Zoho CRM contact by ID, including all custom fields and linked records
- **zoho_related_records**: For example: module="Accounts", recordId="123", relatedModule="Contacts" returns all contacts at that account. Common patterns: Accounts→Contacts, Contacts→Deals, Deals→Notes, Accounts→Deals. Use when the user asks "who are the contacts at this company?" or "what deals does this contact have?"

Get records related to a parent record in Zoho CRM — e.g., contacts of an account, deals of a contact, notes of a lead
- **zoho_search_accounts**: Returns account name, industry, website, phone, annual revenue, and owner. Accounts are the company-level records that contacts and deals are linked to.

Search Zoho CRM accounts (companies) by name to find business entities and their organizational data
- **zoho_search_contacts**: Returns contact name, email, phone, linked account, and owner. Contacts represent qualified individuals — converted leads or manually created customer records. Use when the user asks about a specific person or needs contact details.

Search Zoho CRM contacts by name or email to find qualified prospects and existing customers
- **zoho_search_leads**: Returns lead name, email, company, lead source (Web/Advertisement/Referral), lead status (Not Contacted/Contacted/Junk), and owner. Leads are the top-of-funnel — unqualified prospects. Once qualified, they can be converted to contacts+accounts+deals.

Search Zoho CRM leads by name, email, or company to find unqualified prospects at the top of the funnel
- **zoho_update_contact**: Only specified fields change. Use to correct info, update phone numbers, or reassign accounts.

Update an existing Zoho CRM contact — change name, email, phone, or other properties


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho CRM Contacts** MCP server using an AI Agent (Claude, ChatGPT, etc.).

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

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-crm-contacts](https://vinkius.com/mcp/zoho-crm-contacts)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zoho CRM Contacts** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zoho-crm-contacts` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho CRM Contacts** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-crm-contacts": {
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
