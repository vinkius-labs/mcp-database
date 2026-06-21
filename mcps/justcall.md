# JustCall MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/justcall)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/justcall-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/justcall-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage phone calls, SMS, and recordings via JustCall API.

## Description
Empower your AI agents with JustCall's cloud phone system. This MCP server allows you to list and retrieve phone calls, track SMS/MMS messages, manage contacts, and access call recordings directly through the JustCall API. Ideal for automating communication workflows and sales engagement.


## Available Tools
- **get_call**: Includes timestamps, participants, and associated notes. Use this for deep investigation of a specific communication event.

Retrieves details for a specific call
- **get_contact**: Returns associated phone numbers, email addresses, and metadata. Use this for detailed customer vetting before or after a call.

Retrieves details for a specific contact
- **list_calls**: Returns call direction (inbound/outbound), duration, status, and IDs. Use this to audit communication activity or track call volumes.

Lists all phone calls
- **list_campaigns**: g., dialer campaigns). Useful for monitoring sales outreach and telemarketing efforts.

Lists all calling campaigns
- **list_contacts**: Returns names, phone numbers, and IDs. Use this to search for customers or provide contact information to the user.

Lists all contacts in JustCall
- **list_messages**: Includes message content, sender/receiver, and delivery status. Essential for monitoring text-based customer interactions.

Lists all SMS/MMS messages
- **list_numbers**: Useful for identifying which numbers are available for specific campaigns or teams.

Lists all phone numbers in your JustCall account
- **list_recordings**: Use this when the user wants to audit call quality or retrieve a specific conversation record.

Lists all call recordings
- **list_users**: Useful for identifying which agent handled a specific call or message.

Lists all users in your organization
- **list_webhooks**: Useful for auditing system integrations.

Lists all configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JustCall** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all recent phone calls in JustCall."

**🤖 AI Agent:**
> I'll fetch the history of your recent phone calls from JustCall.

---

**👤 You:**
> "Show me the latest SMS messages."

**🤖 AI Agent:**
> I'll retrieve the list of recent text messages from your JustCall account.

---

**👤 You:**
> "Check the details for contact ID '123'."

**🤖 AI Agent:**
> I'll look up the full profile and history for that specific contact in JustCall.


## Installation & Usage

To install and use the **JustCall** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/justcall](https://vinkius.com/mcp/justcall)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
