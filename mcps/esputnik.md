# eSputnik MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/esputnik)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/esputnik-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/esputnik-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Omnichannel marketing automation with eSputnik.

## Description
The eSputnik MCP server allows your AI agent to orchestrate marketing campaigns across Email, SMS, Web Push, and Mobile Push. Send messages, retrieve contact lists, and manage omnichannel workflows seamlessly.


## Available Tools
- **attach_to_group**: Add contacts to a specific group
- **create_contact**: Create a new contact in eSputnik
- **detach_from_group**: Remove contacts from a group
- **get_account_info**: Retrieve account and organization metadata
- **get_contact**: Retrieve details for a specific contact
- **get_message_status**: Check the delivery status of a sent message
- **list_contacts**: List all contacts in eSputnik
- **list_groups**: List all contact groups/segments
- **list_unsubscribed**: List unsubscribed email addresses
- **search_contacts**: Search for contacts by email or phone
- **send_smart_send**: Trigger an omnichannel message send
- **trigger_event**: Generate a system event to trigger workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **eSputnik** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my contact groups in eSputnik."

**🤖 AI Agent:**
> I've retrieved your segments. You have 3 groups: 'VIP Customers', 'Newsletter Subs', and 'Inactive Users'.

---

**👤 You:**
> "Send an SMS saying 'Your order has shipped!' to +123456789."

**🤖 AI Agent:**
> The SMS has been successfully dispatched to +123456789 via eSputnik.

---

**👤 You:**
> "Add 'john@example.com' to the 'VIP Customers' list."

**🤖 AI Agent:**
> Contact 'john@example.com' was successfully added to the 'VIP Customers' group.


## Installation & Usage

To install and use the **eSputnik** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/esputnik](https://vinkius.com/mcp/esputnik)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
