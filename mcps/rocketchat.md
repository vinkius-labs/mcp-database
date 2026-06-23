# Rocket.Chat MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rocketchat)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Connect your AI assistant to Rocket.Chat to seamlessly send messages, explore channels, manage directories, and orchestrate chat operations directly.

## Description
Connect your conversational assistant directly to **Rocket.Chat**, the open-source team communication platform. This integration transforms your AI into an active participant capable of chatting, sending notifications to channels, identifying active users, and auditing chat room data organically within your workspace.

### What you can do

- **Communicate Actively** — Instruct your assistant to post messages into public channels or private direct messages (`chat_post_message`, `chat_send_message`). Need to fix a typo? The AI can seamlessly edit (`chat_update_message`) or delete previous messages (`chat_delete_message`).
- **Explore Channels & Groups** — Give your assistant vision over public discussions (`list_public_channels`) or private channels you belong to (`list_private_groups`). You can then extract deep information about specific rooms using `get_channel_info`.
- **Audit Users in the Network** — Scan the entire user directory (`list_users`) to locate team members and review their roles and connection status directly (`get_user_info`).

### How it works

1. Install this module in your MCP connectivity environment.
2. Visit your Rocket.Chat profile's 'Personal Access Tokens' panel online to configure and generate an Auth Token.
3. Securely enter your `Rocket.Chat URL`, your associated `Rocket.Chat User ID`, and the `Auth Token` in the form below.
4. Interact naturally with your AI: "Send a welcome message to #general thanking the new members, and then list all of my active direct messages."

### Who is this for?

- **Team Leaders** — Orchestrate team-wide announcements asynchronously or ask the AI to summarize active channels without navigating through clunky chat apps.
- **Support Staff** — Instantly ping specific users or lookup a colleague's profile and roles using natural language.
- **Operations & IT** — Empower your conversational agent to act as a responsive chatbot directly inside Rocket.Chat, running commands and pushing logs directly to specific channels.


## Available Tools (10)
- **chat_delete_message**: You must provide both room ID and message ID.

Deletes a message from a room
- **chat_post_message**: Sends a message to a channel or user by name
- **chat_send_message**: Sends a message to a specific room by ID
- **chat_update_message**: Updates the text of an existing message
- **get_channel_info**: Retrieves details for a specific channel
- **get_user_info**: Retrieves detailed information for a specific user
- **list_direct_messages**: Lists all active direct message rooms
- **list_private_groups**: Lists all private groups (channels) the user is a member of
- **list_public_channels**: Lists all public channels in the workspace
- **list_users**: Lists all users in the workspace directory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rocket.Chat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all of my active direct messages."

**🤖 AI Agent:**
> I checked your direct communications using `list_direct_messages` and retrieved 4 active room IDs. These IDs represent ongoing 1-on-1 private channels. Let me know if you would like me to list public channels or drop a message into one of these direct rooms.

---

**👤 You:**
> "Send a welcome message to #general thanking the new members."

**🤖 AI Agent:**
> Done. I invoked the `chat_post_message` tool assigning `#general` as the destination. The room successfully received the message: 'Welcome to all the new members! Glad to have you here.' Let me know if you would like me to modify or erase it.

---

**👤 You:**
> "Find and get the user info for the ID abCD123."

**🤖 AI Agent:**
> I utilized the `get_user_info` tool passing the specific ID. The resulting payload revealed this belongs to user 'Richard', logged as active, carrying an 'Admin' organizational role within your servers. I can list their joined groups next if you want.


## ❓ FAQ

**Q: Can the assistant create new channels or invite new users to the Rocket.Chat workspace?**
No. This tool package is primarily focused on organic text-based communication, message manipulation (sending, modifying, deleting), and environment querying (listing what already exists). The generative capability to create workspace structural entities like 'new channels' or provisioning administrative user accounts is deactivated for baseline security in this module.

**Q: How does `chat_post_message` differ from `chat_send_message`?**
`chat_send_message` uses a unique alphanumeric `Room ID` (e.g. 'cxyz123') to target an exact space unambiguously. Meanwhile, `chat_post_message` is designed to be human-readable, allowing your assistant to route messages to named destinations like '#general', '#dev-team', or directly to a user like '@johndoe'.

**Q: Can the AI edit or delete messages sent by other users?**
Only if the authenticated account has the required admin or moderator permissions in the target channel. The AI inherits the same role-based restrictions as the user whose token is configured.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rocketchat](https://vinkius.com/mcp/rocketchat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rocket.Chat** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rocketchat` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rocket.Chat** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rocketchat": {
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
