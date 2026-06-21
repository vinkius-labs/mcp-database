# Placetel MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/placetel)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/placetel-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/placetel-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage Placetel users, devices, numbers, and calls.

## Description
# Placetel

The Placetel MCP Server allows AI agents to interact with your Placetel PBX data seamlessly.

### What you can do
- Retrieve users, SIP users, and groups.
- Access phone numbers and routing plans.
- Manage devices and call detail records (CDRs).

### How it works
Connect your Placetel account via your API Token to manage your VoIP configurations dynamically.


## Available Tools
- **get_group**: Get details for a specific group
- **get_sip_user**: Get details for a specific SIP user
- **get_user**: Get details for a specific user
- **list_call_detail_records**: List Call Detail Records (CDRs)
- **list_calls**: List active or recent calls
- **list_devices**: List all devices
- **list_groups**: List all Placetel groups
- **list_numbers**: List all Placetel numbers
- **list_sip_users**: List all Placetel SIP users
- **list_users**: List all Placetel users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Placetel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all devices in Placetel."

**🤖 AI Agent:**
> I retrieved your devices. Here are the active ones: 'Desk Phone 1', 'Softphone - John'.

---

**👤 You:**
> "Get call details from today."

**🤖 AI Agent:**
> Here are your Call Detail Records for today, including 5 inbound calls and 3 outbound calls.

---

**👤 You:**
> "List all users in my account."

**🤖 AI Agent:**
> You have 2 users in your account: 'Admin' and 'Sales'.


## Installation & Usage

To install and use the **Placetel** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/placetel](https://vinkius.com/mcp/placetel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
