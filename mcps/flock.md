# Flock MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flock)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/flock-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/flock-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage team collaboration via Flock — send rich messages with FlockML, handle public channels and private groups, and search rosters directly from any AI agent.

## Description
Connect your **Flock** bot to any AI agent and take full control of your team communication, private groups, and organizational roster through natural conversation.

### What you can do

- **Rich Messaging Orchestration** — Provision massively fast payloads strictly into Flock chats, utilizing `<flockml>` to render rich enterprise attachments and formatted layouts natively
- **Public Channel Discovery** — Enumerate explicitly attached public channels and execute bulk iterations to capture global namespaces and routing configurations synchronously
- **Private Group Management** — Identify bounded private groups and retrieve precise physical definitions detailing exactly how hidden groups operate within your enterprise
- **Organizational Roster Auditing** — Discovers global identity blocks mapping direct `@` aliases to absolute string UUIDs to solve accurate routing for the entire company
- **Identity Metadata Retrieval** — Perform structural extraction of profile metadata linked to Flock users, resolving time zones and LDAP/SSO properties securely
- **Chat Log Ingestion** — Pull chronological asynchronous logs from any room, extracting raw JSON objects mapping historical strings natively from chat fetchers
- **Membership Oversight** — Audit IAM boundaries and identify explicit active UUIDs directly attached to channels or groups to verify intended audiences flawlessly

### How it works

1. Subscribe to this server
2. Enter your Flock Bot Token (found in the Flock Developer Dashboard > My Apps > Bot Token)
3. Start managing your team communication from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Team Leads & Managers** — send announcements and coordinate private groups without leaving the chat interface
- **Developers** — test bot messaging logic and verify FlockML rendering directly from the IDE or chat
- **IT Admins** — audit channel memberships and verify organizational roster mappings using natural language
- **Ops Teams** — monitor public channels and manage private team communication in real-time


## Available Tools
- **channels_get_info**: Retrieve explicit Channel descriptions and banner logic mappings
- **channels_list_public**: Enumerate explicitly attached `public` channels active within Flock
- **channels_list_members**: Identify explicit Active UUIDs directly attached evaluating Channel ingress
- **chat_fetch_messages**: Extracts raw JSON objects mapping historical strings natively returned by `chat.fetchMessages`.

Read recent structural Chat payloads targeting a Flock Room
- **users_get_metadata**: Perform structural extraction of metadata linked to a Flock Identity
- **groups_get_info**: Inspect deep internal credentials identifying a precise Private Group
- **groups_list_private**: Returns arrays necessary to retrieve correct routing UUIDs.

Identify bounded Private Groups tracking strict IAM boundaries
- **groups_list_members**: Crucial for verifying sensitive message targets.

Audit IAM boundaries explicitly granting read permissions to a Group
- **roster_list_directory**: Returns explicit array definitions mapping direct `@` aliases to absolute string UUIDs solving accurate routing natively.

Identify precise active Human constraints navigating the entire Flock company
- **chat_send_message**: Detects if formatted `<flockml>` definitions are passed and converts the payload dynamically bypassing standard Markdown limits rendering rich enterprise attachments.

Provision a massively fast payload strictly into an established Flock Chat


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flock** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a message to group 'g:123': 'Project update is live!'"

**🤖 AI Agent:**
> Message dispatched! 'Project update is live!' has been sent to group g:123. I've used your bot token to route the payload through the Flock API synchronously.

---

**👤 You:**
> "List all public channels in my Flock workspace"

**🤖 AI Agent:**
> Retrieving channels... I found 5 public environments: '#general', '#product-news', '#marketing', '#announcements', and '#engineering'. Which one would you like to see the members for?

---

**👤 You:**
> "Get the metadata for user '@john_doe'"

**🤖 AI Agent:**
> Retrieving identity... For alias '@john_doe' (UUID: u:456), I found: Name: John Doe, Email: john@example.com, Time Zone: America/New_York. He is currently an active member of 3 private groups.


## Installation & Usage

To install and use the **Flock** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flock](https://vinkius.com/mcp/flock)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
