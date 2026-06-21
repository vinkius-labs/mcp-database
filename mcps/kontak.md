# Kontak MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kontak)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kontak-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kontak-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage communications — list messages, send SMS, and audit contacts.

## Description
Connect your AI agent to **Kontak** to automate your customer communications and message auditing.

### Key Features

- **Unified Messaging history** — List and audit all sent and received SMS and call logs
- **Contact Management** — Access and manage your Kontak address book via natural language
- **Outbound SMS** — Send text messages to customers directly from your chat client
- **Template Access** — Browse available message templates for consistent communication
- **Audit & Analytics** — Retrieve system logs and account metadata to monitor performance

### Quick Setup

1. Subscribe to this server
2. Log in to your Kontak account, go to **API Settings** and generate a Bearer Token
3. Enter your token in the configuration panel
4. Start managing your communications via chat


## Available Tools
- **list_kontak_messages**: List all sent and received messages
- **get_message_details**: Get details for a specific message
- **list_kontak_contacts**: List all contacts
- **get_contact_details**: Get details for a specific contact
- **send_outbound_sms**: Send a new SMS message
- **list_kontak_templates**: List available message templates
- **list_kontak_tags**: List all contact tags
- **get_kontak_account_info**: Get account settings and info
- **list_kontak_webhooks**: List configured webhooks
- **get_kontak_audit_logs**: Retrieve system audit logs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kontak** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 messages from my Kontak account"

**🤖 AI Agent:**
> Retrieving your message history… I've found 5 recent SMS messages. The last one was sent to +1234567890 with the body 'Your appointment is confirmed'.

---

**👤 You:**
> "Send an SMS to +1987654321 saying 'Hello from AI'"

**🤖 AI Agent:**
> Message sent successfully to +1987654321. Status: Delivered. ID: msg_abc123.

---

**👤 You:**
> "Find contact named 'Robert'"

**🤖 AI Agent:**
> Found one match: Robert Smith (Phone: +1122334455). He is tagged as 'VIP Customer'. Would you like to see his full profile?


## Installation & Usage

To install and use the **Kontak** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kontak](https://vinkius.com/mcp/kontak)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
