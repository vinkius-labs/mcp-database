# LiveAgent MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/liveagent)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/liveagent-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/liveagent-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage customer support tickets, conversations, and call records directly through LiveAgent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LiveAgent** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all currently open tickets in LiveAgent."

**🤖 AI Agent:**
> I've retrieved the open tickets. You have 3 pending: 'Login Issue' (ID: 452), 'Billing Inquiry' (ID: 453), and 'Feature Request' (ID: 454). Would you like to see the details for any of these?

---

**👤 You:**
> "Add a note to conversation 452: 'Investigating server logs now'."

**🤖 AI Agent:**
> Internal note successfully added to conversation 452. The team will be able to see your update.

---

**👤 You:**
> "Get the profile information for agent support@company.com."

**🤖 AI Agent:**
> I've found the agent profile. Name: Sarah Connor, Role: Senior Support, Status: Active. Would you like to see her recent time reports?


## Installation & Usage

To install and use the **LiveAgent** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/liveagent](https://vinkius.com/mcp/liveagent)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
