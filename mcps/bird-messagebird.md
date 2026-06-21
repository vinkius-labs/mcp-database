# Bird (MessageBird) MCP Server

Unified communications platform for SMS, WhatsApp, Email, and Voice — manage conversations and contacts at scale.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/bird-messagebird)

## Overview
**Category:** talk-to-me
**Tools Count:** 10

## Description
Connect **Bird** (formerly MessageBird) to your AI agents to orchestrate omnichannel communication through simple natural language. 

### What you can do

- **Unified Conversations** — List, read, and manage conversation threads across multiple channels (SMS, WhatsApp, Email) in a single view.
- **Direct Messaging** — Send messages instantly to any customer identifier using your registered Bird channels.
- **CRM & Contacts** — Create and update customer profiles, managing identifiers and metadata to maintain a clean communication record.
- **Voice Audit** — List and inspect voice call history and statuses directly from the AI.

### How it works

1. Subscribe to this server
2. Enter your Bird Access Key and Workspace ID
3. Start communicating via Claude, Cursor, or any MCP client

### Who is this for?

- **Support Teams** — Audit conversation history and respond to customers across any channel without switching tabs.
- **Sales & Marketing** — Register new leads as contacts and trigger personalized messages via WhatsApp or SMS.
- **Operations** — Automate communication workflows and audit voice call logs for quality assurance.


## Available Tools
- **create_contact**: Identifiers should be a JSON string, e.g., '[{"key":"phone","value":"+123"}]'.

Create a new contact profile in the Bird workspace
- **get_call**: Fetch the details of a single voice call
- **get_contact**: Retrieve detailed information about a specific contact profile
- **get_conversation**: Fetch the detailed metadata and status of a single conversation by its unique ID
- **list_calls**: List all voice calls made or received in the workspace
- **list_contacts**: List all customer contact profiles stored in the workspace
- **list_conversations**: Retrieve a list of all ongoing or archived conversations in the Bird workspace
- **list_messages**: List all individual messages within a specific conversation thread
- **send_message**: You must provide a valid channelId (e.g., for SMS or WhatsApp).

Send a new message to a recipient through a specific communication channel (SMS, WhatsApp, etc.)
- **update_contact**: Data should be a JSON string, e.g., '{"displayName":"New Name"}'.

Update the metadata or identifiers of an existing contact


## Installation & Usage

To install and use the **Bird (MessageBird)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bird-messagebird](https://vinkius.com/mcp/bird-messagebird)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
