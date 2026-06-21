# Kustomer MCP Server

Manage customer service — list conversations, audit customers, and search timelines.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kustomer)

## Overview
**Category:** customer-support
**Tools Count:** 10

## Description
Connect your AI agent to **Kustomer** to streamline your support operations and customer data auditing.

### Key Features

- **Omnichannel Conversation Access** — List and audit support conversations from email, chat, and social channels
- **Customer 360 View** — Fetch detailed customer profiles including custom attributes and history
- **Message Auditing** — Retrieve the full message history for any support interaction
- **Timeline Search** — Perform deep searches across customer timelines using complex JSON filters
- **Service Context** — List support queues, agents, and custom data classes (Klasses)

### Simple Setup

1. Subscribe to this server
2. Log in to Kustomer and generate a **Bearer API Key** (Settings > Security > API Keys)
3. Enter your key in the configuration panel
4. Start managing your support data via natural language


## Available Tools
- **list_kustomer_customers**: Essential for identifying customer IDs for support auditing.

List all customers in Kustomer
- **get_customer_profile**: Get details for a specific customer
- **list_support_conversations**: List recent support conversations
- **get_conversation_details**: Get details for a specific conversation
- **list_conversation_messages**: List all messages in a conversation
- **list_support_queues**: g., Billing, Technical Support) defined in Kustomer.

List active support queues
- **list_kustomer_agents**: List all support agents (users)
- **search_kustomer_timeline**: Provide filters as a JSON string.

Perform a deep search across the customer timeline
- **list_data_klasses**: List Kustomer custom data classes (Klasses)
- **check_kustomer_api_status**: Check the status of the Kustomer API


## Installation & Usage

To install and use the **Kustomer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kustomer](https://vinkius.com/mcp/kustomer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
