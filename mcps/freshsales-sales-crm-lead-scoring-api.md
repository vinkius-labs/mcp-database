# Freshsales (Sales CRM & Lead Scoring API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freshsales-sales-crm-lead-scoring-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/freshsales-sales-crm-lead-scoring-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/freshsales-sales-crm-lead-scoring-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage your sales pipeline via Freshsales — create leads, track contacts, manage deals, and automate CRM workflows directly from any AI agent.

## Description
Connect your **Freshsales** CRM to any AI agent to streamline your sales operations through natural conversation.

### What you can do

- **Lead Management** — Create, update, and list leads, or convert them into contacts once qualified using the `convert_lead` tool.
- **Contact & Account Tracking** — Maintain detailed profiles for individuals and organizations within your sales ecosystem with `create_contact` and `create_account`.
- **Deal Pipeline** — Monitor and create sales deals to keep your revenue targets on track using `create_deal` and `list_deal_stages`.
- **Sales Activities** — Log notes, tasks, and appointments to ensure no follow-up is missed via `create_note`, `create_task`, and `create_appointment`.
- **Global Search** — Instantly find any record across your CRM using powerful `search_global` and `search_lookup` tools.

### How it works

1. Subscribe to this server
2. Enter your Freshsales Domain and API Key
3. Start managing your sales funnel from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Representatives** — quickly update lead status and log notes without leaving your workflow.
- **Sales Managers** — get instant reports on deal stages and lead sources via chat.
- **Account Executives** — manage contacts and accounts seamlessly while preparing for meetings.


## Available Tools
- **convert_lead**: last_name and company_name are mandatory.

Convert a lead to a contact
- **create_account**: Create a new sales account
- **create_appointment**: Create an appointment
- **create_contact**: Create a new contact
- **create_deal**: Create a new deal
- **create_lead**: Provide at least a first name or email.

Create a new lead in Freshsales
- **create_note**: Create a note for a record
- **create_task**: Create a task
- **get_account**: View a specific sales account
- **get_contact**: View a specific contact
- **get_deal**: View a specific deal
- **get_lead**: View a specific lead
- **list_deal_stages**: Fetch deal stages
- **list_industry_types**: Fetch industry types
- **list_lead_sources**: Fetch lead sources
- **list_leads**: Use filters API to get view_id if unknown.

List all leads in a specific view
- **list_owners**: Fetch all users/owners
- **search_global**: Global search across entities
- **search_lookup**: Lookup search for specific fields
- **update_contact**: Update an existing contact
- **update_lead**: Update an existing lead


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freshsales (Sales CRM & Lead Scoring API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new lead for Sarah Jenkins (sarah.j@example.com) from 'Global Tech'."

**🤖 AI Agent:**
> I've created the lead for Sarah Jenkins at Global Tech. The record has been successfully added to your Freshsales CRM.

---

**👤 You:**
> "Search for any contact or lead associated with the email 'mike@startup.io'."

**🤖 AI Agent:**
> I found one lead matching that email: Mike Ross (ID: 88293). Would you like to see his full details or log a new task for him?

---

**👤 You:**
> "List all the leads in my 'New Leads' view (ID: 400123)."

**🤖 AI Agent:**
> Fetching leads from view 400123... I've found 12 leads. The most recent ones are 'Alice Cooper' and 'Bob Smith'.


## Installation & Usage

To install and use the **Freshsales (Sales CRM & Lead Scoring API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freshsales-sales-crm-lead-scoring-api](https://vinkius.com/mcp/freshsales-sales-crm-lead-scoring-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
