# BulkSMS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bulksms)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bulksms-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bulksms-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication](../categories/communication.md)

Send and manage SMS messages via BulkSMS.com — track delivery, manage groups, and monitor credits directly from any AI agent.

## Description
Connect your **BulkSMS.com** account to any AI agent and orchestrate your global SMS communications, contact management, and credit oversight through natural conversation.

### What you can do

- **SMS Dispatch** — Send single or bulk SMS messages to any international destination using the REST API.
- **Delivery Tracking** — List and retrieve detailed metadata for sent messages and monitor their delivery status.
- **Contact Organization** — Access and list your contact groups and their members directly from your workspace.
- **Account Oversight** — Retrieve your account profile and real-time credit balance to ensure uninterrupted service.
- **Message Deep Dives** — Get detailed data for specific message IDs straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your BulkSMS.com Username and Password
3. Start managing your SMS campaigns from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Teams** — quickly send notifications or promotional alerts without manual portal work.
- **Support Desks** — send one-off updates or verification codes straight from their workflow tools.
- **Operations Managers** — monitor message delivery and account balance using natural language.


## Available Tools
- **get_message**: Get details of a specific message
- **get_profile**: Retrieve account profile and credit balance
- **get_account_info**: Retrieve core account information
- **list_group_members**: List members of a specific contact group
- **list_groups**: List contact groups
- **list_messages**: List sent messages
- **send_bulk_sms**: Send multiple SMS messages
- **send_sms**: Send a single SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BulkSMS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to +1234567890 saying 'Your appointment is confirmed'."

**🤖 AI Agent:**
> I've sent the SMS to +1234567890. The message ID is msg_123 and it's currently being processed for delivery.

---

**👤 You:**
> "How many credits do I have left in my BulkSMS account?"

**🤖 AI Agent:**
> Retrieving your profile... You currently have 450.25 credits remaining in your BulkSMS account.

---

**👤 You:**
> "List the members of my 'VIP Customers' group."

**🤖 AI Agent:**
> Retrieving group members... I found 15 contacts in the 'VIP Customers' group, including John Doe (+1234567890) and Sarah Smith (+0987654321).


## Installation & Usage

To install and use the **BulkSMS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bulksms](https://vinkius.com/mcp/bulksms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
