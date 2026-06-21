# Kintone MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kintone-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kintone-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kintone-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Build custom business apps without code using drag-and-drop forms, workflow automation, and team collaboration spaces.

## Description
Connect your **Kintone** instance to any AI agent and manage business applications through natural conversation.

### What you can do

- **App Management** — List all apps and inspect their field configurations
- **Record Operations** — Create, read, update, and query records in any app
- **Data Queries** — Search records using Kintone query syntax with field filters
- **Field Access** — Browse app fields and their types for data modeling

### How it works

1. Subscribe to this server
2. Enter your Kintone domain and API Token
3. Start managing apps from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Teams** — manage business data without opening each app
- **Developers** — integrate Kintone data into AI workflows
- **Managers** — query records and track metrics across apps


## Available Tools
- **add_records**: Input should be a JSON array of record objects.

Add one or more records to an app
- **delete_records**: Delete records from an app
- **get_app_fields**: Get app field settings
- **get_record**: Get details for a specific record
- **get_space_details**: Get details for a space
- **list_apps**: List all accessible Kintone apps
- **list_records**: You can provide an optional query string.

List records from a Kintone app
- **update_records**: Update one or more records


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kintone** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all apps and show the latest 5 records from the 'Sales Pipeline' app."

**🤖 AI Agent:**
> Apps: 6. Sales Pipeline (234 records), Customer DB (456), Inventory (89), HR Requests (34), Bug Tracker (123), Expenses (67). Latest Sales Pipeline: 1) Acme Corp — $45K, Stage: Proposal. 2) TechCo — $28K, Negotiation. 3) StartupXYZ — $12K, Demo. 4) GlobalInc — $67K, Closing. 5) MediCorp — $33K, Qualification.

---

**👤 You:**
> "Create a new deal in Sales Pipeline and query all deals over $50K."

**🤖 AI Agent:**
> Record created! 'NovaTech Partnership' — $85K, Stage: Proposal, Owner: Sarah. Pipeline: 235 records. Deals over $50K: 4 records. 1) NovaTech — $85K (Proposal). 2) GlobalInc — $67K (Closing). 3) EntCorp — $120K (Negotiation). 4) MegaGroup — $55K (Demo). Total pipeline value >$50K: $327K.

---

**👤 You:**
> "Show the field configuration for the Customer DB app."

**🤖 AI Agent:**
> Customer DB fields: 10. Company Name (text, required), Contact Email (email), Phone (phone), Industry (dropdown: SaaS, Healthcare, Finance, Retail), Size (number), Annual Revenue (currency), Status (dropdown: Active, Prospect, Churned), Last Contact (date), Notes (textarea), Attachments (file). 456 records total.


## Installation & Usage

To install and use the **Kintone** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kintone-alternative](https://vinkius.com/mcp/kintone-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
