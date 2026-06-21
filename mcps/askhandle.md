# AskHandle MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/askhandle)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/askhandle-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/askhandle-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Integrate custom AI agents with AskHandle.

## Description
The AskHandle MCP server enables your AI agent to manage chat rooms, messages, leads, and webhooks. Interact with your AskHandle AI agents and capture visitor information directly from your conversation.


## Available Tools
- **create_lead**: Create a new lead
- **create_room**: Create a new chat room
- **create_webhook**: Create a new webhook subscription
- **delete_webhook**: Delete a webhook subscription
- **get_me**: Check API connectivity and get account context
- **list_leads**: List all leads captured
- **list_messages**: List messages, optionally filtered by room
- **list_rooms**: List all chat rooms
- **list_webhooks**: List all configured webhooks
- **retrieve_lead**: Get details of a specific lead
- **retrieve_room**: Get details of a specific chat room
- **send_message**: Send a message to a chat room


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AskHandle** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active chat rooms in AskHandle."

**🤖 AI Agent:**
> Fetching active rooms... You currently have 5 active sessions. The latest is 'Support Query - Ticket #402'.

---

**👤 You:**
> "Send a message 'Hello' to room 'ROOM_ID'."

**🤖 AI Agent:**
> Message 'Hello' successfully sent to room 'ROOM_ID'.

---

**👤 You:**
> "List all captured leads."

**🤖 AI Agent:**
> I've retrieved your leads. You have 24 new leads from this week, including 'Acme Corp' and 'TechLogix'.


## Installation & Usage

To install and use the **AskHandle** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/askhandle](https://vinkius.com/mcp/askhandle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
