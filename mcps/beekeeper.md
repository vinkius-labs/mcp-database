# Beekeeper MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/beekeeper)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/beekeeper-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/beekeeper-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Empower your frontline workforce via Beekeeper — manage users, streams, posts, and messages directly from any AI agent.

## Description
Connect your **Beekeeper** account to any AI agent and streamline your internal communications and frontline management through natural conversation.

### What you can do

- **User & Group Management** — List all employees and groups to maintain an organized organizational structure.
- **Stream & Post Control** — Manage communication channels (streams) and publish updates to keep everyone informed.
- **Direct Messaging** — Send messages and retrieve conversation histories to facilitate instant communication.
- **Tenant Insights** — Access tenant information and system metadata for administrative oversight.
- **Advanced Search** — Quickly find specific users by name or email to coordinate efforts effectively.

### How it works

1. Subscribe to this server
2. Enter your Beekeeper Subdomain and API Token
3. Start managing your workforce communication from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Managers** — quickly list and find employee contact details without manual searches.
- **Operations Leads** — publish urgent updates to specific frontline streams instantly.
- **Internal Communicators** — monitor engagement and messages across the organization directly from their workflow.


## Available Tools
- **create_post**: Create a new post in a stream
- **get_tenant_info**: Retrieve Beekeeper tenant information
- **get_user**: Get details of a specific user
- **list_groups**: List Beekeeper groups
- **list_messages**: List messages in a conversation
- **list_posts**: List posts in a specific stream
- **list_streams**: List Beekeeper streams (channels)
- **list_users**: List all Beekeeper users
- **search_users**: Search for users by name or email
- **send_message**: Send a direct message to a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beekeeper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active communication streams on Beekeeper."

**🤖 AI Agent:**
> I've retrieved your streams. You have 4 active channels: 'Company News' (ID: str_1), 'Operations Updates' (ID: str_2), 'HR Announcements' (ID: str_3), and 'Social Feed' (ID: str_4).

---

**👤 You:**
> "Post to stream str_2: 'Reminder: New safety protocols start tomorrow morning.'"

**🤖 AI Agent:**
> Done! I've posted your reminder to the 'Operations Updates' stream. Everyone in that channel will see it in their Beekeeper app.

---

**👤 You:**
> "Find the user ID for 'Sarah Miller'."

**🤖 AI Agent:**
> I found one user matching 'Sarah Miller'. Her User ID is `u_99283`. She is part of the 'Logistics Team' group.


## Installation & Usage

To install and use the **Beekeeper** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/beekeeper](https://vinkius.com/mcp/beekeeper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
