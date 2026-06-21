# HubSpot MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hubspot)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Grow better with an integrated CRM that unifies marketing, sales, service, and operations in one powerful platform.

## Description
Connect your **HubSpot** account to any AI agent and manage your entire CRM through natural conversation.

### What you can do

- **Contact Management** — List, create, search, and delete contacts with full property access
- **Company Records** — Browse and inspect companies with metadata and associations
- **Deal Pipeline** — List all deals with amounts, stages, and pipeline assignments, and inspect individual deal details
- **Smart Search** — Search contacts using HubSpot filter syntax for targeted queries
- **Association Management** — Link CRM objects together (Contact ↔ Company, Contact ↔ Deal, etc.)
- **Schema Discovery** — List all available properties for any object type (contacts, companies, deals, tickets)
- **Pipeline Configuration** — View all sales pipelines with stages and probabilities
- **Team Management** — List all HubSpot users and record owners

### How it works

1. Subscribe to this server
2. Enter your HubSpot Private App Access Token
3. Start managing your CRM from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — search contacts, update deal stages, and link records without switching to the CRM dashboard
- **Marketing Teams** — manage contact databases, segment audiences, and audit property schemas
- **RevOps** — inspect pipelines, audit data quality, and manage associations through AI


## Available Tools (12)
- **link_crm_objects**: g. Contact to Company).

Create association
- **create_contact**: Add new contact
- **remove_contact**: Delete contact
- **get_company_info**: Get company details
- **get_contact_details**: Get contact info
- **get_deal_details**: Get deal info
- **list_companies**: List CRM companies
- **list_contacts**: List CRM contacts
- **list_deals**: List sales deals
- **list_hubspot_users**: List record owners
- **get_object_schema**: List fields
- **search_contacts**: Find contacts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HubSpot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all deals in the pipeline and the contacts associated with the highest-value one."

**🤖 AI Agent:**
> 12 active deals. Pipeline: 'Sales Pipeline'. Stages: Prospect (3), Qualified (4), Proposal (3), Negotiation (2). Top deal by value: 'Enterprise SaaS Migration' — $285,000, Stage: Negotiation, Close date: May 15, 2025, Owner: Sarah Chen. Associated contacts: 1) John Smith (CTO, john@acmecorp.com). 2) Lisa Park (VP Engineering, lisa@acmecorp.com). 3) Mike Torres (Procurement, mike@acmecorp.com). Associated company: Acme Corp (company_456, 500 employees, Enterprise segment). Total pipeline value: $892,000. Would you like to search for contacts or view the pipeline configuration?

---

**👤 You:**
> "Search for all contacts with @enterprise.com emails and create a new contact for the CEO."

**🤖 AI Agent:**
> Search results for '@enterprise.com': 4 contacts found. 1) James Rodriguez (VP Sales, james@enterprise.com). 2) Ana Müller (Director Marketing, ana@enterprise.com). 3) Chen Wei (Head of Engineering, wei@enterprise.com). 4) Sarah Johnson (HR Manager, sarah.j@enterprise.com). New contact created! Email: ceo@enterprise.com, First name: David, Last name: Williams, ID: contact_8921. Now linking to company... ✅ Associated to 'Enterprise Corp' (company_789). You now have 5 contacts for Enterprise Corp. Would you like to list companies or view deal details?

---

**👤 You:**
> "Show the sales pipelines, all HubSpot users, and the property schema for deals."

**🤖 AI Agent:**
> Sales pipelines: 2 configured. 1) 'Sales Pipeline' — 5 stages: Prospect (10%), Qualified (25%), Proposal (50%), Negotiation (75%), Closed Won (100%). 12 active deals, $892K value. 2) 'Partnership Pipeline' — 4 stages: Introduction, Evaluation, Agreement, Active Partner. 3 active deals, $150K value. HubSpot users: 8 owners. Sarah Chen (Sales), Mike Torres (Sales), Lisa Park (Marketing), James Rodriguez (CS), Ana Müller (RevOps), 3 others. Deal properties (42 total): Key fields: dealname, amount, dealstage, pipeline, closedate, hubspot_owner_id, description, deal_currency_code. Custom: contract_length, implementation_fee, annual_recurring_revenue. Would you like to create a deal or search contacts?


## ❓ FAQ

**Q: Can I search for contacts using specific filters?**
Yes. The `search_contacts` tool accepts a JSON array of HubSpot filters. Example: `[{"propertyName":"email","operator":"CONTAINS_TOKEN","value":"@company.com"}]`. This uses HubSpot's native search API to find contacts matching property values, date ranges, or engagement criteria. Use `get_object_schema` with 'contacts' to discover all searchable properties.

**Q: Can I link contacts to companies and deals?**
Yes. Use `link_crm_objects` with the source object type and ID, target object type and ID, and the association type name. Example: link a contact to a company with `fromType='contacts', fromId='123', toType='companies', toId='456', associationType='contact_to_company'`. This creates bidirectional CRM relationships.

**Q: What type of HubSpot credential do I need?**
You need a **Private App Access Token** from your HubSpot account. This is different from OAuth tokens — it provides direct API access scoped to the permissions you select when creating the Private App. The token is sent as a Bearer token in the Authorization header against `api.hubapi.com`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hubspot](https://vinkius.com/mcp/hubspot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HubSpot** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hubspot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HubSpot** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hubspot": {
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
