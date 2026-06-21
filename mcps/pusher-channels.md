# Pusher Channels MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pusher-channels)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage real-time communication via Pusher — trigger events, monitor active channels, and manage presence users directly from your AI agent.

## Description
Connect your **Pusher Channels** infrastructure to any AI agent to orchestrate real-time messaging and monitor your application's pub/sub health through natural language.

### What you can do

- **Event Broadcasting** — Trigger single or batch events across multiple channels with custom JSON payloads to update your frontend instantly.
- **Channel Monitoring** — List all active channels, filter by prefix, and fetch specific metadata like subscription counts or user counts.
- **Presence Management** — Retrieve lists of user IDs currently subscribed to presence channels to understand real-time engagement.
- **Session Control** — Terminate all active WebSocket connections for a specific user ID to handle security incidents or forced logouts.
- **State Inspection** — Query the detailed state of any specific channel to debug message flow or connection metrics.

### How it works

1. Subscribe to this server
2. Provide your Pusher App ID, Key, Secret, and Cluster
3. Start broadcasting events and managing connections from Claude, Cursor, or any MCP client

No more jumping into the Pusher Debug Console to manually trigger test events or check if a channel is active. Your AI acts as a real-time infrastructure operator.

### Who is this for?

- **Full-stack Developers** — trigger test events and verify webhook payloads directly from the code editor.
- **DevOps Engineers** — monitor channel activity and user counts without opening the Pusher dashboard.
- **Support Teams** — quickly identify if a user is connected to a presence channel or terminate problematic sessions.


## Available Tools
- **get_channel**: Fetch information for a specific channel
- **list_channel_users**: Fetch users in a presence channel
- **list_channels**: Fetch multiple channels
- **terminate_user_connections**: Terminate all connections for a user
- **trigger_batch_events**: Trigger multiple events in a single batch
- **trigger_event**: Max 10KB data payload.

Trigger an event on one or more channels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pusher Channels** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Trigger a 'new-order' event on the 'orders' channel with data '{"id": 123, "total": 50.00}'."

**🤖 AI Agent:**
> Event 'new-order' successfully triggered on channel 'orders'. The payload has been broadcasted to all active subscribers.

---

**👤 You:**
> "List all active channels that start with 'presence-'."

**🤖 AI Agent:**
> I found 3 active presence channels: 'presence-chat-room-1', 'presence-lobby', and 'presence-editor-v2'. Would you like to see the users in any of these?

---

**👤 You:**
> "Terminate all connections for user ID 'user_999'."

**🤖 AI Agent:**
> All active WebSocket connections for 'user_999' have been terminated. The user will need to re-authenticate to reconnect.


## ❓ FAQ

**Q: Can I send the same event to multiple channels at once?**
Yes. The `trigger_event` tool accepts an array of channel names (up to 100) to broadcast your message simultaneously across your infrastructure.

**Q: How do I check which users are currently online in a presence channel?**
Use the `list_channel_users` tool with the specific channel name (must start with `presence-`). It will return a list of all active user IDs.

**Q: Is it possible to force a user to disconnect?**
Yes. The `terminate_user_connections` tool allows you to close all active WebSocket connections for a specific user ID immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pusher-channels](https://vinkius.com/mcp/pusher-channels)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pusher Channels** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pusher-channels` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pusher Channels** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pusher-channels": {
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
