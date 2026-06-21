# Cliengo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cliengo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cliengo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cliengo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage conversational marketing and leads via Cliengo — track chatbot conversations, monitor captured leads, and audit chat history directly from any AI agent.

## Description
Connect your **Cliengo** account to any AI agent and take full control of your conversational marketing and lead management through natural conversation. Streamline how you capture and qualify leads via chatbot and WhatsApp natively.

### What you can do

- **Lead Oversight** — List and retrieve details for all leads and contacts captured via Cliengo natively
- **Conversation Intelligence** — Access all chatbot or WhatsApp conversations and retrieve full message histories flawlessly
- **Website Tracking** — List all websites and projects where your Cliengo chatbot is installed securely
- **Message Auditing** — Retrieve all specific messages exchanged with a contact to understand their needs flawlessly
- **User Management** — List internal users and agents who manage conversations within your account securely
- **Webhook Visibility** — Monitor all configured webhooks for real-time lead data integration directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Cliengo API Key (found in Dashboard > Settings > API)
3. Start managing your conversational leads from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Managers** — monitor lead capture rates and review chatbot interactions using natural language
- **Marketing Teams** — audit lead sources and UTM campaign data without opening the dashboard
- **Customer Support** — quickly look up chat histories and contact profiles straight from their chat interface
- **Ops Teams** — verify chatbot installation status and webhook integration health


## Available Tools
- **get_contact_messages**: Retrieve all messages exchanged with a specific contact
- **get_lead_details**: Get detailed information for a specific contact
- **get_chat_history**: Get the full message history for a specific conversation
- **list_cliengo_users**: List all internal users and agents in the account
- **list_cliengo_leads**: List all leads and contacts captured via Cliengo
- **list_chat_conversations**: List all chatbot or WhatsApp conversations
- **list_cliengo_webhooks**: List all configured webhooks for real-time lead data
- **list_cliengo_websites**: List all websites/projects where Cliengo is installed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cliengo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all new leads from Cliengo today."

**🤖 AI Agent:**
> Retrieving today's leads... I found 5 new contacts: Juan Perez (WhatsApp), Maria Garcia (Chatbot), and 3 others. Would you like to see their details or chat history?

---

**👤 You:**
> "Show me the chat history for Juan Perez."

**🤖 AI Agent:**
> Checking messages for Juan Perez... He asked about 'Pricing Plans' and 'WhatsApp Integration' at 10:15 AM via the website chatbot. He left his phone number for a follow-up.

---

**👤 You:**
> "List all internal users who manage my Cliengo account."

**🤖 AI Agent:**
> Retrieving user list... Your account has 3 active users: Sarah Miller (Admin), Mike Scott (Agent), and Jane Doe (Agent). All are currently available to handle new conversations.


## Installation & Usage

To install and use the **Cliengo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cliengo](https://vinkius.com/mcp/cliengo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
