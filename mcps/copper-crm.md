# Copper CRM MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/copper-crm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/copper-crm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/copper-crm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage leads, people, and sales opportunities directly within Copper CRM.

## Description
Integrate **Copper**, the CRM designed for Google Workspace, directly into your AI workflow. Manage your entire sales pipeline and contact list using natural language.

### What you can do

- **Lead Management** — List, retrieve, and create leads to keep your pipeline moving.
- **Contact Tracking** — Quickly find people and companies, and view their full profiles.
- **Sales Opportunities** — Monitor deals and opportunities to stay on top of your revenue goals.
- **Activity Logging** — Log calls, emails, and meetings directly to any record via chat.

### How it works

1. Connect the Copper integration to your AI assistant.
2. Authorize using your Copper User Email and API Key (found in Settings > API Keys).
3. Manage your CRM data through intuitive conversation.

### Who is this for?

- **Sales Teams** — Update lead statuses and log activities instantly after calls.
- **Account Managers** — Retrieve company and contact details during client meetings.
- **Business Owners** — Get a quick overview of the sales pipeline and project progress.


## Available Tools
- **create_lead**: Creates a new lead record with identity properties and prepares it for pipeline entry.

Create a new lead in the CRM
- **get_lead_details**: Resolves granular profile data including contact history, custom field values, and system-level metadata.

Get detailed information for a specific lead
- **get_person_details**: Resolves individual profile data including email addresses, phone numbers, and associated entity linkages.

Get detailed profile for a specific person
- **list_companies**: Resolves company identity properties such as company IDs, legal names, and primary contact links.

List all companies in the CRM
- **list_leads**: Resolves lead identity properties including names, email addresses, and pipeline status across the CRM system boundary.

List all leads in Copper CRM
- **list_opportunities**: Resolves opportunity data including deal names, monetary values, closing dates, and current stage identifiers.

List sales opportunities and deals
- **list_people**: Resolves individual identity properties including unique identifiers, contact names, and associated organizations.

List contacts (people) in Copper
- **list_projects**: Resolves project identity properties and metadata for collaborative tracking.

List all projects in Copper
- **list_tasks**: Resolves actionable item properties including task descriptions, due dates, and associated CRM records.

List tasks and follow-ups
- **log_activity**: Resolves and links activity details, types, and parent entity identifiers across the CRM interaction boundary.

Log a new activity (call, email, meeting) for a record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Copper CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all leads that are currently in the 'New' status."

**🤖 AI Agent:**
> I found 8 leads with the status 'New', including 'TechCorp Solutions' and 'Bright Future Agency'. Would you like to see the details for any of them?

---

**👤 You:**
> "Log a call activity for the lead 'TechCorp Solutions' regarding the pricing proposal."

**🤖 AI Agent:**
> Call activity logged successfully for 'TechCorp Solutions'. I've noted that you discussed the pricing proposal. Should I set a follow-up task for next Tuesday?

---

**👤 You:**
> "Show me my top 5 sales opportunities sorted by monetary value."

**🤖 AI Agent:**
> Here are your top 5 opportunities: 1. 'Global Expansion' ($50,000), 2. 'Q4 Software License' ($25,000), 3. 'Infrastructure Upgrade' ($15,000)... Would you like to update the close date for any of these?


## Installation & Usage

To install and use the **Copper CRM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/copper-crm](https://vinkius.com/mcp/copper-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
