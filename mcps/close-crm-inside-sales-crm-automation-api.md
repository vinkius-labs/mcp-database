# Close CRM (Inside Sales CRM & Automation API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/close-crm-inside-sales-crm-automation-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/close-crm-inside-sales-crm-automation-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/close-crm-inside-sales-crm-automation-api-mcp)
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


## Installation & Usage

To install and use the **Close CRM (Inside Sales CRM & Automation API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/close-crm-inside-sales-crm-automation-api](https://vinkius.com/mcp/close-crm-inside-sales-crm-automation-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
