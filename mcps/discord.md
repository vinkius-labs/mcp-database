# Discord MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/discord)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Manage communities via Discord — list server channels and members, send and edit messages, and handle channel moderation directly from any AI agent.

## Description
Connect your **Discord** bot to any AI agent and take full control of your community management and real-time messaging through natural conversation.

### What you can do

- **Server & Guild Auditing** — Perform structural extraction of metadata linked to a Discord Server, fetching member approximations and Snowflake IDs
- **Channel Orchestration** — Identify explicitly assigned routing text/voice channels and manage parent-category mappings to organize your server logically
- **Messaging & Chat** — Dispatch automated text payloads with Markdown support and edit pre-existing textual strings to update dynamic information in real-time
- **Member Oversight** — Enumerate explicitly attached user accounts and iterate through authorized members matching your server namespace
- **Content Moderation** — Forcibly purge chat payloads out of visible memory and irreversibly delete active channel mappings to manage server security
- **Real-time Logs** — Pull chronological asynchronous logs from any channel, extracting string contents and nested attachment metadata
- **Slowmode Control** — Inspect deep properties identifying precise rate-limit configurations and evaluate assigned delays natively

### How it works

1. Subscribe to this server
2. Enter your Discord Bot Token (found in the Discord Developer Portal > Application > Bot)
3. Start managing your Discord communities from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Community Managers** — moderate channels and update server information without switching to the Discord client
- **Developers** — test bot messaging logic and verify channel configurations directly from the IDE or chat
- **Customer Support** — monitor channel messages and respond to inquiries using natural language
- **Ops Teams** — audit server member lists and manage channel hierarchies in real-time


## Available Tools (15)
- **add_reaction**: Use URL-encoded custom emojis (name:id) or standard Unicode emojis (e.g., 👍).

Add an emoji reaction to a Discord message
- **create_guild_channel**: Default `type=0` maps to standard Text Channels.

Provision a radically fast new structural Channel sandbox
- **create_message**: Capable of mapping Markdown `<@user_id>` tags natively forcing push notifications instantly.

Dispatch an automated text Payload resolving towards a Channel
- **create_thread**: If message_id is provided, creates a thread from that message.

Create a new thread in a Discord channel
- **delete_channel**: Vaporizes all nested historical chat payloads, pinned messages, and file attachments natively dropping active connections entirely returning 404s.

Irreversibly delete an entirely active Discord Channel mapping
- **delete_message**: Drops the raw chat out of the Channel history permanently replacing it with visual space on all clients natively.

Purge an existing Chat Payload out of the visible memory
- **edit_message**: Ideal for updating dynamic progress bars inside a live Chat context.

Mutate pre-existing textual strings tied to a Bot Message
- **get_channel**: Inspect deep properties identifying a precise Discord Channel
- **get_guild_member**: Get details for a specific server member
- **get_guild**: Fetches explicit Snowflake IDs configuring precisely the total member approximations natively bypassing localized channel scopes.

Perform structural extraction of metadata linked to a Discord Server
- **list_channel_messages**: Extracts string contents, nested attachments mapping binary sizes, and embed payloads.

Read recent structural Chat payloads targeting a Channel
- **list_guild_channels**: Returns crucial Snowflake Channel IDs prerequisite to performing all downstream messaging actions.

Identify explicitly assigned routing text/voice Channels within a Server
- **list_guild_members**: Restricted heavily by `GUILD_MEMBERS` Privileged Intent inside the developer portal securely.

Enumerate explicitly attached user accounts active within the Server
- **list_guild_roles**: Use role IDs with member management.

List all roles configured in a Discord server
- **pin_message**: Channels have a maximum of 50 pins.

Pin a message in a Discord channel


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Discord** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all channels in guild '123456789'"

**🤖 AI Agent:**
> I found 5 channels in your server. Text channels include '#general' (ID: 101) and '#announcements' (ID: 102). Voice channels include 'General VC' (ID: 201). Which one would you like to interact with?

---

**👤 You:**
> "Send a message to channel '101': 'Hello community! The bot is live.'"

**🤖 AI Agent:**
> Message dispatched! 'Hello community! The bot is live.' has been sent to channel 101. The message ID is 'msg_999'.

---

**👤 You:**
> "Get the last 5 messages from channel '101'"

**🤖 AI Agent:**
> Retrieving messages from channel 101... I found 5 recent posts. Highlights include a welcome message from 'System' and a question about API keys from 'User_A'. Would you like the full text of these messages?


## ❓ FAQ

**Q: Can my agent list all members of a Discord server?**
Yes. Use the 'list_guild_members' tool. Note that this action is heavily restricted by the 'GUILD_MEMBERS' Privileged Intent, which must be enabled for your bot in the Discord Developer Portal.

**Q: How do I edit a message previously sent by the bot via chat?**
Provide the 'channel_id', 'message_id', and the new 'content' to the 'edit_message' tool. Your agent will update the core content directly, substituting the payload rendered globally without deleting and reposting.

**Q: Can I delete an entire channel through natural conversation?**
Yes. The 'delete_channel' mutation allows you to irreversibly delete an active Discord channel. The agent will destroy the routing bucket and vaporize all nested chat payloads and attachments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/discord](https://vinkius.com/mcp/discord)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Discord** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `discord` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Discord** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "discord": {
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
