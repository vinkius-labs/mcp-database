# Missive MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/missive)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/missive-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/missive-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Collaborative email and shared inbox for teams.

## Description
Connect **Missive** to your AI agent and manage your team's communication efficiently. Access conversations, messages, and contacts through natural conversation to stay organized and responsive.

### What you can do

- **Conversation Management** — List and view conversations from any mailbox (inbox, assigned, closed).
- **Collaboration** — Post internal comments or trigger actions like closing and assigning conversations.
- **Message Access** — Read all messages and comments within a specific conversation thread.
- **Contact Organization** — Search for and create contacts in your shared or private contact books.
- **Draft & Send** — Create email drafts and deliver them directly from your AI agent.

### How it works

1. Subscribe to this server
2. Enter your Missive Access Token
3. Start collaborating with Claude, Cursor, or any MCP client


## Available Tools
- **create_contact**: Create a new contact
- **create_draft**: Create an email draft
- **create_post**: Can also trigger actions like closing, assigning, or labeling.

Create a post (comment or action) in a conversation
- **get_conversation**: Get details for a specific conversation
- **get_me**: Get current Missive user details
- **list_contacts**: List Missive contacts
- **list_conversations**: A mailbox filter is required (e.g., "inbox", "all", "assigned", "closed").

List conversations from a specific mailbox
- **list_labels**: List Missive labels
- **list_messages**: List messages in a conversation
- **send_draft**: Send a prepared draft


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Missive** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my recent conversations in the inbox."

**🤖 AI Agent:**
> Fetching conversations... I found 8 recent threads including 'Project Update' and 'Client Feedback'.

---

**👤 You:**
> "Add a comment 'Working on this now' to conversation id 123."

**🤖 AI Agent:**
> Posting comment... Your note has been added to the conversation history.

---

**👤 You:**
> "Find contact info for 'Jane Smith'."

**🤖 AI Agent:**
> Searching contacts... Found Jane Smith (jane@example.com) in the shared contact book.


## Installation & Usage

To install and use the **Missive** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/missive](https://vinkius.com/mcp/missive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
