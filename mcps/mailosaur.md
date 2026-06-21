# Mailosaur MCP Server

Automate email and SMS testing and management via the Mailosaur REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mailosaur)

## Overview
**Category:** productivity
**Tools Count:** 8

## Description
Connect your **Mailosaur** account to any AI agent to automate your email and SMS testing workflows. This MCP server enables your agent to manage virtual servers (inboxes), retrieve and search for messages, and extract content for validation directly from natural language interfaces.

### What you can do

- **Virtual Inbox Oversight** — List and manage all virtual servers and retrieve their unique routing domains
- **Message Retrieval** — List all email and SMS messages received by a specific server instantly
- **Advanced Search** — Find specific messages by sender, recipient, subject, or body content using detailed criteria
- **Content Inspection** — Retrieve the full HTML and text content of any message for automated validation
- **Inbox Maintenance** — Clear entire server inboxes or delete specific messages via simple commands
- **Dynamic Infrastructure** — Create and configure new virtual servers programmatically for testing isolation

### How it works

1. Subscribe to this server
2. Enter your Mailosaur API Key
3. Start managing your test communications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Engineers** — Automate the verification of transactional emails and SMS codes via natural language commands
- **Developers** — Quickly inspect incoming test emails and clear virtual inboxes directly from your IDE
- **Operations Teams** — Monitor automated communication flows and audit incoming messages effortlessly


## Available Tools
- **create_virtual_server**: Create a new virtual server/inbox
- **clear_server_inbox**: Delete all messages in a server
- **delete_specific_message**: Permanently remove a message
- **get_message_content**: Get the full content of a specific message
- **get_server_details**: Get details for a specific virtual server
- **list_server_messages**: List all messages in a virtual server
- **search_server_messages**: Requires a server ID and criteria like sentTo, sentFrom, or subject.

Search for specific messages using criteria
- **list_virtual_servers**: Use this to identify server IDs.

List all Mailosaur virtual servers


## Installation & Usage

To install and use the **Mailosaur** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailosaur](https://vinkius.com/mcp/mailosaur)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
