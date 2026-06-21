# Close CRM (Inside Sales CRM & Automation API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/close-crm-inside-sales-crm-automation-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage leads, contacts, and sales opportunities in Close CRM — automate your inside sales pipeline and lead tracking directly from any AI agent.

## Description
Connect your **Close CRM** account to any AI agent to streamline your sales workflows. This server provides comprehensive access to manage your leads, contacts, and sales opportunities through natural language.

### What you can do

- **Lead Management** — List, create, update, and delete leads (companies/organizations) to keep your database current and accurate.
- **Contact Organization** — Manage individual contacts within leads, including names and email details for precise communication.
- **Opportunity Tracking** — List and create sales opportunities, track deal values (in cents), confidence levels, and pipeline stages.
- **Sales Automation** — Use AI to quickly update lead statuses or record new potential deals without manual data entry.

### How it works

1. Subscribe to this server
2. Enter your Close API Key
3. Start managing your sales pipeline from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — update lead info and opportunities on the fly during or after calls to maintain momentum.
- **Sales Ops** — automate lead list cleaning, field updates, and organization via AI-driven workflows.
- **Founders & Executives** — get a quick overview of the sales pipeline and key opportunities without digging through CRM menus.


## Available Tools
- **activity_report**: Generate an Activity Report
- **bulk_email**: Initiate a mass email to a filtered list of leads
- **create_contact**: Create a new Contact
- **create_lead**: Create a new Lead
- **create_opportunity**: Create a new Opportunity
- **create_task**: Create a new Task
- **create_webhook**: Create a Webhook subscription
- **delete_lead**: Delete a Lead
- **get_custom_field_schema**: Get Custom Field Schema for an object type
- **list_calls**: List Call activities
- **list_contacts**: List Contacts in Close CRM
- **list_emails**: List Email activities
- **list_events**: List Event Log (last 30 days)
- **list_form_submissions**: List Form Submission activities
- **list_forms**: List web forms and their field definitions
- **list_leads**: Supports pagination and field selection.

List Leads in Close CRM
- **list_meetings**: List Meeting activities
- **list_notes**: List Note activities
- **list_opportunities**: List Opportunities
- **list_sequences**: List Sequences (automated outreach workflows)
- **list_sms**: List SMS activities
- **list_tasks**: List Tasks
- **search_data**: Advanced Filtering for Leads or Contacts
- **update_contact**: Update an existing Contact
- **update_lead**: Behaves as a PATCH request.

Update an existing Lead
- **update_opportunity**: Update an existing Opportunity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Close CRM (Inside Sales CRM & Automation API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 5 leads in my Close CRM and show their names and IDs."

**🤖 AI Agent:**
> I've retrieved your first 5 leads: 1. TechFlow (ID: lead_1), 2. GreenEnergy (ID: lead_2), 3. BlueSky (ID: lead_3), 4. AlphaCorp (ID: lead_4), and 5. Zenith (ID: lead_5).

---

**👤 You:**
> "Create a new lead named 'Vurb Marketplace' with a contact 'Alice Smith' and email 'alice@vurb.com'."

**🤖 AI Agent:**
> The lead 'Vurb Marketplace' has been successfully created with Alice Smith as the primary contact. The Lead ID is lead_vurb_99.

---

**👤 You:**
> "Add a new opportunity for lead lead_123 with a value of $1000 and 80% confidence."

**🤖 AI Agent:**
> I've added the opportunity to lead_123. It is recorded with a value of 100,000 cents ($1,000.00) and an 80% confidence level.


## ❓ FAQ

**Q: Can I permanently remove a lead from my CRM using this server?**
Yes, you can use the `delete_lead` tool by providing the specific Lead ID. Please note that this action is permanent and cannot be undone.

**Q: How do I track the financial value and confidence of a potential deal?**
Use the `create_opportunity` or `update_opportunity` tools. You can specify the `value` (in cents), the `value_period` (monthly, annual, or one_time), and a `confidence` percentage from 0 to 100.

**Q: Can I filter or limit the number of leads returned when listing them?**
Yes! The `list_leads` tool supports `_limit` for result counts, `_skip` for pagination, and `_fields` to specify exactly which data points (like name or status) you want to retrieve.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/close-crm-inside-sales-crm-automation-api](https://vinkius.com/mcp/close-crm-inside-sales-crm-automation-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Close CRM (Inside Sales CRM & Automation API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `close-crm-inside-sales-crm-automation-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Close CRM (Inside Sales CRM & Automation API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "close-crm-inside-sales-crm-automation-api": {
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
