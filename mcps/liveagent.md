# LiveAgent MCP Server

Manage customer support tickets, conversations, and call records directly through LiveAgent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/liveagent)

## Overview
**Category:** customer-support
**Tools Count:** 16

## Description
Connect your **LiveAgent** helpdesk to any AI agent and manage your customer support operations through natural conversation.

### What you can do

- **Ticket Management** — List all tickets, filter by status, and track history using `list_tickets` and `list_ticket_history`.
- **Conversations** — Retrieve full conversation threads with `get_conversation` and respond or add internal notes using `add_conversation_message`.
- **Communication Logs** — Access call records and phone number configurations via `list_calls` and `list_phone_numbers`.
- **Agent & Account Info** — Fetch agent profiles with `get_agent` and account settings with `get_settings`.
- **CRM & Reporting** — Manage companies and customer groups with `list_companies` and `list_customer_groups`, and view performance via `list_time_reports`.

### How it works

1. Subscribe to this server
2. Enter your LiveAgent Domain and API Key
3. Start managing your helpdesk from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Leads** — monitor ticket volumes and agent performance without leaving your workspace
- **Developers** — integrate support data into workflows or debug customer issues directly from the IDE
- **Customer Success Managers** — quickly retrieve conversation history and company details to prepare for meetings


## Available Tools
- **get_settings**: Retrieve account settings (v3)
- **list_ticket_history**: Uses cursor-based pagination.

Retrieve ticket history (v3)
- **list_tickets**: Supports simple or advanced JSON filters (e.g. {"status":"N"} or [["date_created","DP","TW"]]).

Retrieve a list of tickets (v3)
- **list_time_reports**: Uses cursor-based pagination.

Retrieve time reports (v3)
- **update_conversation_status**: Change conversation status (v1)
- **add_customer_fields**: Add custom field values to a customer (v1)
- **add_conversation_message**: Add a new message or note to a conversation (v1)
- **list_calls**: Uses cursor-based pagination.

Retrieve call records (v3)
- **list_companies**: List all companies (v1)
- **list_conversations**: Supports optional filtering parameters.

List all conversations/tickets (v1)
- **list_customer_groups**: List customer groups (v1)
- **delete_conversation**: Delete a conversation (v1)
- **get_agent**: Retrieve agent info and auth token (v1)
- **get_company**: Retrieve company info (v1)
- **get_conversation**: Retrieve conversation details (v1)
- **list_phone_numbers**: Uses cursor-based pagination.

Retrieve phone numbers (v3)


## Installation & Usage

To install and use the **LiveAgent** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/liveagent](https://vinkius.com/mcp/liveagent)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
