# Freshdesk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freshdesk)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/freshdesk-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/freshdesk-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage customer support via Freshdesk — track tickets, handle contacts, and oversee agent groups via AI agents.

## Description
Connect your **Freshdesk** instance to any AI agent to automate your customer service operations and helpdesk workflows through the Model Context Protocol (MCP). Freshdesk is an award-winning customer support software that enables businesses of all sizes to deliver exceptional service. This MCP server enables you to manage your support tickets, track agent performance, and retrieve detailed contact metadata directly through natural conversation.

### Key Features

- **Ticket Orchestration** — List all support tickets, fetch detailed metadata including priority and status, and open new tickets instantly.
- **Contact & Company Oversight** — Access your database of end-users and company organizations to maintain full context of customer relationships.
- **Collaborative Threads** — Retrieve full conversation histories and internal notes associated with any specific support ticket.
- **Workforce Insights** — List all support agents and team members to verify who is online and handling the helpdesk volume.
- **Group & Queue Monitoring** — Access configured agent groups and routing queues to understand your support structure.
- **Product Discovery** — List all products mapped in your helpdesk instance for multi-product support environments.
- **Real-time Performance** — Fetch high-level helpdesk metadata to verify connectivity and account health.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Freshdesk Domain prefix and API Key (found in Profile Settings > Your API Key)
3. Start managing your helpdesk from Claude, Cursor, or any MCP client

### Who is this for?

- **Support Managers** — quickly monitor ticket volumes or list agent workloads without manual dashboard navigation.
- **Customer Success Teams** — get a real-time overview of customer support history and organization metadata via simple AI commands.
- **Agents & Technicians** — automate the retrieval of ticket threads and requester profiles while focused on resolution.


## Available Tools
- **list_helpdesk_agents**: List support agents
- **create_ticket**: Open a new ticket
- **check_freshdesk_status**: Verify helpdesk status
- **get_agent_details**: Get agent metadata
- **get_company_details**: Get company metadata
- **get_contact_details**: Get customer metadata
- **get_ticket_details**: Get ticket metadata
- **list_helpdesk_companies**: List client companies
- **list_helpdesk_contacts**: List customers
- **list_ticket_thread**: List ticket interactions
- **list_tickets**: List support tickets
- **update_ticket**: Modify ticket properties


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freshdesk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open support tickets in my Freshdesk."

**🤖 AI Agent:**
> Retrieving tickets... I found 5 open requests, including 'Broken Login' (Priority: Urgent) and 'Billing Inquiry'. Would you like the full details for the urgent one?

---

**👤 You:**
> "Show me the conversation thread for ticket '12345'."

**🤖 AI Agent:**
> Fetching thread... For ticket 12345, I found 3 replies and 1 private note. The last update was from Agent Mike stating 'investigating the server logs'.

---

**👤 You:**
> "Create a new ticket: 'API Access Problem' from 'user@example.com'."

**🤖 AI Agent:**
> Ticket created! I've successfully opened ticket ID 67890 regarding 'API Access Problem' for user@example.com. It has been assigned to the general support queue.


## Installation & Usage

To install and use the **Freshdesk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freshdesk](https://vinkius.com/mcp/freshdesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
