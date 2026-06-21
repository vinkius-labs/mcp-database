# Nutshell CRM MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nutshell-crm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nutshell-crm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nutshell-crm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage sales and relationships via Nutshell CRM — track leads, contacts, and accounts directly from your AI agent.

## Description
Connect your **Nutshell CRM** account to your AI agent and take control of your sales pipeline and customer relationships through natural conversation using their JSON-RPC API.

### What you can do

- **Lead Management** — List and search for sales leads, and retrieve complete metadata, values, and pipeline stages.
- **Relationship Tracking** — Access your entire database of individual contacts and business accounts with deep profile inspection.
- **Activity Monitoring** — View a list of all tasks, calls, and meetings, and browse through available activity types.
- **Universal Search** — Perform a global keyword search across leads, contacts, and accounts simultaneously.
- **Custom Data Access** — Retrieve definitions for all custom fields configured in your Nutshell instance.
- **Deep Inspection** — Fetch complete metadata for specific records using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Nutshell login Email (or Domain) and API Key
3. Start managing your sales from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales Teams** — quickly look up a lead's status or contact details without navigating the CRM interface.
- **Account Managers** — monitor customer interactions and account health directly from your workspace.
- **Business Owners** — automate the retrieval of pipeline reports and activity logs for daily standups.


## Available Tools
- **list_accounts**: Find and list business accounts
- **list_activities**: List CRM activities
- **list_activity_types**: g. Phone Call, Email) available for logging.

List available activity types
- **list_contacts**: Find and list people/contacts
- **list_leads**: Find and list CRM leads
- **get_account_details**: Get specific account info
- **get_contact_details**: Get specific contact details
- **list_custom_fields**: List CRM custom fields
- **get_lead_details**: Get specific lead info
- **universal_search**: Search across all entities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nutshell CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my most recent sales leads."

**🤖 AI Agent:**
> Retrieving leads... I found 5 recent leads including 'Enterprise Upgrade - Acme' ($12,000), 'New Office Solution', and 'Q4 Growth'. Would you like the full details for the Acme upgrade?

---

**👤 You:**
> "Search for any contact or lead related to 'Dunder Mifflin'."

**🤖 AI Agent:**
> Executing universal search... I've found 1 Account ('Dunder Mifflin Paper Co.'), 2 Contacts ('Michael Scott', 'Dwight Schrute'), and 1 active Lead. Which record would you like to inspect?

---

**👤 You:**
> "What are my upcoming activities and meetings?"

**🤖 AI Agent:**
> Retrieving activities... You have 3 scheduled items: 'Follow-up Call' with John Smith at 2:00 PM, 'Project Kickoff' tomorrow at 10:00 AM, and a 'Dinner Meeting'. Shall I retrieve the contact info for John Smith?


## Installation & Usage

To install and use the **Nutshell CRM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nutshell-crm](https://vinkius.com/mcp/nutshell-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
