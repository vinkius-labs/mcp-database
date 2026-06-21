# MessageBird MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/messagebird)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/messagebird-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/messagebird-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage your global communications — send SMS and audit contacts via AI.

## Description
Empower your AI agent to orchestrate your entire global communication strategy with **MessageBird**, the leading omnichannel platform. By connecting MessageBird to your agent, you transform complex messaging workflows into a natural conversation. Your agent can instantly send SMS to multiple recipients, audit your contact database, and check your real-time account balance without you ever touching a dashboard. Whether you are providing verification codes or managing marketing broadcasts, your agent acts as a real-time communication coordinator, ensuring your messages are delivered and your audience data is organized.

### What you can do

- **Messaging Intelligence** — Send SMS messages to global recipients and retrieve detailed delivery status and history.
- **Contact Auditing** — List and retrieve detailed metadata for your global contact database and groups.
- **Financial Oversight** — Check your real-time account balance to maintain strict organizational control over your costs.
- **Channel Management** — List configured communication channels to ensure your omnichannel strategy is active.
- **Network Intelligence** — List HLR (Home Location Register) requests to verify number validity and network status.

### How it works

1. Subscribe to this server
2. Enter your MessageBird API Key
3. Start managing your global communications through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — monitor communication spend and send quick global alerts straight from your workflow.
- **Marketing Leads** — verify if new contact groups have been correctly created and are ready for broadcasts.
- **Customer Support** — perform rapid audits of message history and verify recipient connectivity without manual logins.
- **Business Owners** — automate omnichannel querying to orchestrate your data-driven communication strategy smoothly.


## Available Tools
- **get_balance**: Get current MessageBird account balance
- **get_contact**: Get details for a specific contact
- **get_group**: Get details for a specific group
- **get_message**: Get details for a specific message
- **list_channels**: List configured channels
- **list_contacts**: List MessageBird contacts
- **list_groups**: List contact groups
- **list_hlr**: List HLR (Network Lookup) requests
- **list_messages**: List recent SMS messages
- **send_sms**: Send an SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MessageBird** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my MessageBird account balance."

**🤖 AI Agent:**
> I've retrieved your balance. You currently have $50.00 available in your account. The payment type is set to PREPAID.

---

**👤 You:**
> "List the last 5 SMS messages sent from my account."

**🤖 AI Agent:**
> I've found your recent messages. You have 5 sent SMS, including one to +123456789 with status 'delivered'. Would you like the full text for any of them?

---

**👤 You:**
> "Send SMS 'Your discount code is VINKIUS20' to +15550123."

**🤖 AI Agent:**
> Message delivered! I've successfully sent the discount code to +15550123. The originator was set to 'Vinkius'. The message ID is xxxxxxxx.


## Installation & Usage

To install and use the **MessageBird** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/messagebird](https://vinkius.com/mcp/messagebird)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
