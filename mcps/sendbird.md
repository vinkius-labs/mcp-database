# Sendbird MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sendbird)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage Sendbird chat infrastructure — orchestrate users, channels, and moderation directly from your AI agent.

## Description
Connect your **Sendbird** application to any AI agent and take full control of your chat ecosystem through natural conversation.

### What you can do

- **User Management** — Create new users, list existing ones, and manage profiles or access tokens for your chat application.
- **Channel Orchestration** — Create and manage Open Channels for massive public scale or Group Channels for private, distinct conversations.
- **Moderation & Safety** — Maintain community standards by blocking, muting, or banning users, and freezing channels during incidents.
- **Automation & Bots** — Create and manage bots to send automated messages and interact with users programmatically.
- **Channel Lifecycle** — Update channel metadata, join or leave group chats, and invite new members seamlessly.

### How it works

1. Subscribe to this server
2. Enter your Sendbird App ID and Master API Token
3. Start managing your messaging infrastructure from Claude, Cursor, or any MCP-compatible client

No more navigating complex dashboards to moderate a user or check channel status. Your AI acts as a real-time chat administrator.

### Who is this for?

- **Support Leads** — quickly moderate users, check channel history, and manage support bots without leaving the console.
- **Developers** — test channel creation, user provisioning, and bot messaging directly from the code editor.
- **Community Managers** — oversee large open channels and enforce safety rules through simple natural language commands.


## Available Tools
- **ban_user**: Ban a user from a channel
- **block_user**: Block a user
- **create_bot**: Create a bot
- **create_group_channel**: Create a group channel
- **create_open_channel**: Create an open channel
- **create_user**: Create a new Sendbird user
- **delete_open_channel**: Delete an open channel
- **freeze_channel**: Freeze a channel
- **get_open_channel**: Get an open channel by URL
- **invite_group_channel**: Invite users to a group channel
- **join_group_channel**: Join a group channel
- **leave_group_channel**: Leave a group channel
- **list_open_channels**: List open channels
- **list_users**: List Sendbird users
- **mute_user**: Mute a user in a channel
- **send_bot_message**: Send a message via bot
- **send_message**: Send a message to a channel
- **update_open_channel**: Update an open channel


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sendbird** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 10 users in our Sendbird application."

**🤖 AI Agent:**
> I've retrieved the user list. Found users: 'admin_01', 'support_agent_a', 'user_992'... Would you like to see the profile details for any of them?

---

**👤 You:**
> "Create a new open channel called 'Global-Lounge' for our community."

**🤖 AI Agent:**
> Channel 'Global-Lounge' has been created successfully. The channel URL is 'sendbird_open_channel_552'. You can now start directing users to this public space.

---

**👤 You:**
> "Freeze the channel at URL 'sendbird_open_channel_123' to stop all messaging."

**🤖 AI Agent:**
> The channel 'sendbird_open_channel_123' is now frozen. Users will be unable to send new messages until it is unfrozen.


## ❓ FAQ

**Q: Can I create a bot to send automated messages in a channel?**
Yes! You can use the `create_bot` tool to register a new bot and then use `send_bot_message` to trigger automated interactions within your chat channels.

**Q: How do I handle disruptive users who violate community rules?**
The server provides several moderation tools: `mute_user` to silence them, `block_user` to prevent interaction, and `ban_user` to remove them from channels entirely.

**Q: Is it possible to manage large-scale public chat rooms?**
Absolutely. Use `create_open_channel` to build public channels that support millions of users, and `list_open_channels` to keep track of your active public environments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sendbird](https://vinkius.com/mcp/sendbird)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sendbird** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sendbird` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sendbird** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sendbird": {
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
