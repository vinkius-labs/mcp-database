# Mailsac MCP Server

Manage disposable and private email addresses via the Mailsac REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mailsac)

## Overview
**Category:** developer-tools
**Tools Count:** 9

## Description
Connect your **Mailsac** account to any AI agent to automate your email testing and inbox management. This MCP server enables your agent to reserve private email addresses, retrieve and search for messages, and inspect HTML or plain text bodies directly from natural language interfaces.

### What you can do

- **Inbox Oversight** — List and manage your reserved (enhanced) addresses and custom domains
- **Instant Retrieval** — Fetch a list of messages received by any address in your account instantly
- **Content Extraction** — Retrieve sanitized HTML or raw plain text bodies to extract verification codes or links
- **Inbox Maintenance** — Permanently delete individual messages or clear entire inboxes via simple commands
- **Infrastructure Management** — Reserve new private addresses programmatically for isolated testing flows
- **Global Search** — Query messages across all your addresses using advanced search parameters (requires paid tier)

### How it works

1. Subscribe to this server
2. Enter your Mailsac API Key
3. Start managing your disposable inboxes from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Engineers** — Automate the extraction of email-based verification codes for testing suites
- **Developers** — Quickly inspect incoming test emails and manage temporary addresses directly from your IDE
- **Privacy-Conscious Users** — Manage temporary communication channels via simple natural language commands


## Available Tools
- **list_reserved_addresses**: List all reserved (enhanced) email addresses
- **delete_inbox_message**: Permanently remove a message from an inbox
- **list_custom_domains**: List custom domains linked to the account
- **get_html_message_body**: Get the sanitized HTML body of a specific message
- **get_plain_text_body**: Get the plain text body of a specific message
- **list_inbox_messages**: List messages in a specific inbox
- **release_reserved_address**: Delete/Release a reserved email address
- **reserve_new_address**: Reserve a specific email address
- **search_account_messages**: Requires a paid Mailsac tier. Use query params like to, from, subject.

Search for messages across all addresses


## Installation & Usage

To install and use the **Mailsac** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailsac](https://vinkius.com/mcp/mailsac)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
