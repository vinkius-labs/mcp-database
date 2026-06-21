# Freshdesk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freshdesk-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/freshdesk-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/freshdesk-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Resolve customer tickets faster with omnichannel helpdesk tools, smart automation, and self-service portals your users will love.

## Description
Connect your **Freshdesk** account to any AI agent and take full control of your customer support ecosystem and helpdesk workflows through natural conversation.

### What you can do

- **Ticket Orchestration** — List and manage support tickets programmatically, including updating statuses (Open, Pending, Resolved, Closed) and priorities
- **Relationship Management** — Access your complete directory of contacts and companies to retrieve detailed profiles and interaction histories
- **Support Intelligence** — Monitor agent groups and individual staff status to coordinate internal routing and manage team workload
- **Knowledge Navigation** — Explore knowledge base folders and organizational structures to assist with customer self-service and internal research
- **Real-time Monitoring** — Retrieve granular metadata for specific tickets, including complete conversation threads and audit logs

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from Freshdesk (Profile Settings)
3. Identify your **Account Subdomain** (e.g., 'vinkius' from vinkius.freshdesk.com)
4. Start managing your helpdesk from Claude, Cursor, or any MCP client

No more manual status checking or complex navigation through support queues. Your AI acts as your dedicated support operations and helpdesk coordinator.

### Who is this for?

- **Support Teams** — instantly triage ticket queues and update statuses using natural language commands
- **Customer Success Managers** — retrieve full interaction histories and verify contact details without leaving your workspace
- **Ops Leads** — monitor agent availability and manage organizational records across the helpdesk


## Available Tools
- **list_support_agents**: List support staff
- **list_support_companies**: List organization records
- **list_contacts**: List helpdesk contacts
- **list_help_folders**: List knowledge base folders
- **list_support_groups**: g. Support, Billing).

List support agent groups
- **list_tickets**: Supports filtering by status or priority.

List helpdesk tickets
- **create_ticket**: Create a new ticket
- **get_contact_details**: Get details for a contact
- **get_ticket_details**: Get details for a ticket
- **update_ticket_details**: Modify an existing ticket


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freshdesk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my open tickets in Freshdesk."

**🤖 AI Agent:**
> I've retrieved 5 open tickets. Notable requests include 'Login issues' (ID: 101) and 'Billing question' (ID: 102). Would you like the full details for any specific ticket?

---

**👤 You:**
> "Show me the details for ticket ID '101'."

**🤖 AI Agent:**
> Fetching metadata for ticket 101... The issue is reported by 'john@example.com'. It's currently 'Open' with 'High' priority. The latest message says the user can't access the dashboard. Shall I list the full conversation?

---

**👤 You:**
> "Create a new ticket 'Feature suggestion' for 'sarah@example.com'."

**🤖 AI Agent:**
> Done! I've created the new ticket for Sarah. The ID is 103 and I've set the priority to 'Low'. Your team will see this in the Freshdesk queue immediately.


## Installation & Usage

To install and use the **Freshdesk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freshdesk-alternative](https://vinkius.com/mcp/freshdesk-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
