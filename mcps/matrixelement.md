# Matrix/Element MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/matrixelement)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Automate your Matrix communications — manage rooms, send secure messages, and sync account state directly from your AI agent.

## Description
Connect your **Matrix** account to any AI agent and take full control of your decentralized communications through natural conversation.

### What you can do

- **Room Management** — Create, join, knock, or leave rooms using simple commands like `create_room` and `join_room`.
- **Messaging & Events** — Send messages or custom events to any room with transaction tracking via `send_message`.
- **State Synchronization** — Use `sync_client` to fetch the latest state from the homeserver and stay updated on all conversations.
- **User Discovery** — Search the global user directory using `search_user_directory` to find and connect with others.
- **Account Control** — Manage your profile, change passwords, or handle account registration and deactivation.
- **Encryption & Keys** — Handle cryptographic keys (`upload_keys`, `query_keys`) for secure, end-to-end encrypted communication.

### How it works

1. Subscribe to this server
2. Provide your Matrix Homeserver URL and Access Token
3. Start orchestrating your chats from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — automate alert rooms and incident response directly from the terminal.
- **Privacy Advocates** — maintain secure, decentralized communication without leaving your AI workflow.
- **Community Managers** — manage room states and user interactions across large Matrix networks.


## Available Tools
- **change_password**: Change the account password
- **claim_keys**: Claim E2EE keys from the homeserver
- **create_room**: Create a new Matrix room
- **deactivate_account**: Deactivate the current Matrix account
- **download_media**: Download media from the homeserver
- **get_room_state**: Get state events for a room
- **join_room**: Join a Matrix room by ID or alias
- **knock_room**: Knock on a Matrix room to request access
- **leave_room**: Leave a Matrix room
- **login_account**: Log in to a Matrix account
- **logout_account**: Log out of the current Matrix account
- **query_keys**: Query E2EE keys from the homeserver
- **register_account**: Register a new Matrix account
- **search_user_directory**: Search the user directory
- **send_message**: Send a message or event to a Matrix room
- **set_room_state**: Set state events for a room
- **sync_client**: Synchronize client state with the homeserver
- **upload_keys**: Upload E2EE keys to the homeserver
- **upload_media**: Upload media to the homeserver


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Matrix/Element** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Sync my Matrix client to see if I have any new notifications."

**🤖 AI Agent:**
> I've triggered a sync. You have 3 new messages in '!engineering:matrix.org' and a new invitation to join the 'Project X' room.

---

**👤 You:**
> "Send a message to room !abc:matrix.org saying 'The deployment is complete'."

**🤖 AI Agent:**
> Message sent successfully to room !abc:matrix.org with transaction ID 'txn_12345'.

---

**👤 You:**
> "Search the user directory for 'bob'."

**🤖 AI Agent:**
> I found 2 users matching 'bob': Bob Smith (@bob_s:matrix.org) and Bob Builder (@builder:matrix.org).


## ❓ FAQ

**Q: How do I see the latest messages in my rooms?**
Use the `sync_client` tool. It synchronizes your local state with the homeserver, retrieving all new events, messages, and room state changes since your last sync.

**Q: Can I search for people on other Matrix servers?**
Yes, the `search_user_directory` tool allows you to search the directory available to your homeserver, helping you find users by their display name or Matrix ID.

**Q: Is it possible to manage room settings like the topic or name?**
Absolutely. Use `set_room_state` to update room metadata. You can change the room name, topic, or other state events by providing the correct `event_type` and `body`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/matrixelement](https://vinkius.com/mcp/matrixelement)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Matrix/Element** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `matrixelement` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Matrix/Element** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "matrixelement": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
