# AgentMail MCP Server

Give your AI agents their own email inbox to read, send, and reply to messages natively.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/agentmail)

## Overview
**Category:** productivity
**Tools Count:** 11

## Description
Connect **AgentMail** to your AI agent and unlock a programmable email client. Stop relying on complex integrations and grant your agent its own functional inbox to communicate with the world.

### What you can do

- **Inboxes** — Create, list, and delete custom email addresses on the fly for your agent
- **Threads** — Scan active conversations and read full historical threads natively
- **Messages** — Send new emails, reply contextually to specific threads, and forward messages
- **Attachments** — Extract and process files attached to incoming emails automatically

### How it works

1. Subscribe to this server
2. Enter your AgentMail API Key
3. Start managing emails from Claude, Cursor, or any MCP-compatible client

Give your AI the ability to reach out, follow up, and monitor replies autonomously.

### Who is this for?

- **AI Developers** — build autonomous agents that communicate with users via email
- **Customer Support** — deploy agents that read incoming tickets and draft thoughtful replies
- **Sales Automation** — let your agent handle outreach and monitor responses automatically


## Available Tools
- **list_inboxes**: An inbox is required to send or receive emails. Returns an array of inboxes with their IDs, email addresses, and names.

List all inboxes assigned to the AgentMail API Key
- **get_inbox**: Get details of a specific inbox by ID
- **create_inbox**: You can optionally link it to a custom domain.

Create a new email inbox for an agent
- **delete_inbox**: Warning: this deletes all emails in it.

Delete a specific inbox by ID
- **list_threads**: Returns a list of thread objects including subject lines and recent message previews. The agent needs an inbox_id first.

List conversation threads inside an inbox
- **get_thread**: Requires a thread_id.

Read all messages inside a specific conversation thread
- **get_attachment**: Attachments might be encoded in base64. Ensure you parse or read it correctly.

Download or read a specific attachment from a message
- **send_message**: Requires the sender inbox_id, which you can get from list_inboxes.

Send a brand new email message
- **reply_to_message**: The thread will be preserved.

Reply to an existing email message/thread
- **forward_message**: You can optionally add text to the forwarded message.

Forward an existing email message
- **update_message**: Update an existing message metadata (like marking it as read)


## Installation & Usage

To install and use the **AgentMail** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agentmail](https://vinkius.com/mcp/agentmail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
