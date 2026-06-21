# Zendesk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zendesk)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zendesk-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zendesk-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage support tickets, users, and organizations on Zendesk — the complete customer service platform for high-scale teams.

## Description
Connect your **Zendesk** account to any AI agent and manage your customer service infrastructure through natural conversation.

### What you can do

- **Ticket Monitoring** — List all active support tickets and retrieve comprehensive details including subject, description, priority, and internal comments
- **Advanced Filtering** — Search for tickets using the full Zendesk search syntax (e.g., 'type:ticket status:open tags:escalation') for complex audits
- **User Discovery** — List and browse all users (customers and agents), and retrieve deep profile details including contact info and organization membership
- **Team Organization** — List support groups and organizations to understand team structures and retrieve IDs for ticket assignment
- **Workflow Governance** — Browse available support macros (templates) and system views to verify your support team's operational processes
- **Customer Insights** — Retrieve full metadata for organization records to see linked users and high-level account properties
- **Deep Discovery** — Quickly find unique ticket, user, group, and macro IDs required for automated support workflows

### How it works

1. Subscribe to this server
2. Enter your Zendesk Subdomain, Email, and API Token
3. Start managing your support operations through Claude, Cursor, or any MCP-compatible client

No more manual logging into the Zendesk dashboard to check a ticket's status. Your AI agent becomes your support operations coordinator.

### Who is this for?

- **Support Leads & Managers** — monitor ticket queues and audit agent performance through simple chat commands
- **Customer Success Managers** — quickly lookup customer profiles and organization details without manual navigation
- **Operations Teams** — verify ticket tags and macro configurations through conversation
- **Developers** — test API responses and verify ticket metadata for custom support integrations


## Available Tools
- **list_macros**: Lists all available support macros (canned responses)
- **list_tickets**: Lists all support tickets in the Zendesk account
- **get_ticket**: Retrieves comprehensive details for a specific support ticket
- **search_tickets**: Syntax: "type:ticket status:open tags:escalation".

Searches for tickets using the Zendesk search syntax
- **list_users**: Lists all users (customers and agents) in the Zendesk account
- **get_user**: Retrieves details for a specific Zendesk user
- **list_organizations**: Lists all organizations defined in Zendesk
- **list_groups**: Lists all support agent groups
- **list_views**: g. "Unassigned tickets") and their IDs.

Lists shared and personal ticket views


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zendesk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open tickets in Zendesk."

**🤖 AI Agent:**
> I found 8 open tickets. The most recent are: 1. 'Login issue' (ID: 501, Priority: High), 2. 'Billing question' (ID: 502, Priority: Normal), and 3. 'Feature request' (ID: 503, Priority: Low). Which one would you like to inspect?

---

**👤 You:**
> "Search for tickets with the tag 'escalation' that are still pending."

**🤖 AI Agent:**
> Searching Zendesk... I found 3 pending tickets with the 'escalation' tag: 1. #550 (Escalated to Engineering), 2. #555 (Critical bug report), and 3. #560 (Data recovery request). Would you like the full details for any of these?

---

**👤 You:**
> "Show me the contact info for user ID '123456789'."

**🤖 AI Agent:**
> User ID 123456789 found: Name: John Doe, Email: john@example.com, Role: End-user, Organization: Acme Corp. He has 3 active tickets. Would you like me to list them for you?


## Installation & Usage

To install and use the **Zendesk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zendesk](https://vinkius.com/mcp/zendesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
