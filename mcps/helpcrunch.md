# HelpCrunch MCP Server

Automate customer support via HelpCrunch — manage chats, customers, and team assignments directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/helpcrunch)

## Overview
**Category:** customer-support
**Tools Count:** 11

## Description
Connect your **HelpCrunch** account to any AI agent and take full control of your customer communication and support workflows through natural conversation.

### What you can do

- **Chat Oversight** — List all active and past conversations, retrieve full transcripts, and monitor response times.
- **Customer Management** — Access detailed customer profiles, add descriptive tags, and track user interaction history.
- **Team Coordination** — Reassign chats to specific team members or departments to ensure the right person handles every query.
- **Proactive Support** — Search through chats using complex filters to identify trends or urgent customer issues.
- **Workflow Automation** — Update chat statuses (closed, open, snoozed) directly from the chat interface.
- **Operational Efficiency** — List support departments and monitor the overall health of your customer service operations.

### How it works

1. Subscribe to this server
2. Enter your HelpCrunch API Key (found in Settings > Developers)
3. Start managing your customer support from Claude, Cursor, or any MCP-compatible client

No more jumping between multiple dashboard tabs. Your AI assistant acts as a dedicated Support Lead or Customer Success Manager.

### Who is this for?

- **Support Managers** — instantly retrieve chat summaries and check team workloads without digging through reports.
- **Customer Success Teams** — check client history and add updates or tags during follow-ups.
- **Sales Development Reps** — monitor new inbound chats and qualify leads directly from the communication flow.


## Available Tools
- **add_customer_tag**: Add a label/tag to a customer profile
- **send_message**: Pass the payload as a JSON string in "body_json" (e.g., {"chat": 123, "text": "Hello"}).

Send a message to a chat
- **get_chat_details**: Get detailed information about a specific chat
- **get_customer_details**: Get detailed profile information for a specific customer
- **list_chats**: Each chat includes basic metadata and status.

List all conversations (chats) in HelpCrunch
- **list_customers**: List all customers (contacts) in HelpCrunch
- **list_departments**: List all support departments
- **list_chat_messages**: Useful for understanding context or historical interactions.

List all messages within a specific chat
- **search_chats**: Pass filter criteria as a JSON string in "filter_json" (e.g., {"status": "open"}).

Search for chats using filters
- **update_chat_assignee**: Assign a chat to a specific team member
- **update_chat_status**: Update the status of a chat (e.g., closed, open)


## Installation & Usage

To install and use the **HelpCrunch** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/helpcrunch](https://vinkius.com/mcp/helpcrunch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
