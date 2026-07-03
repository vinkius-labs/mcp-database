# PubNub (Real-time Messaging) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pubnub-real-time-messaging)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Enable real-time messaging, presence tracking, and message history for your AI agent using PubNub's global data stream network.

## Description
Connect your **PubNub** account to any AI agent to orchestrate real-time communication, monitor user presence, and manage data streams through natural language.

### What you can do

- **Real-time Messaging** — Publish JSON payloads to any channel and retrieve historical message logs with precise timetokens.
- **Presence Monitoring** — Track who is online (`here_now`), see which channels a user is in (`where_now`), and manage custom presence states.
- **User & Channel Metadata** — Manage App Context by creating and retrieving user profiles, channel metadata, and memberships.
- **Message Management** — Count messages sent after specific timestamps or purge history for compliance and storage management.
- **File Sharing** — Generate upload URLs and manage files stored within the PubNub network.
- **Admin & Push** — Monitor keyset metrics, manage applications, and configure mobile push notifications (APNS/FCM).

### How it works

1. Subscribe to this server
2. Enter your PubNub Subscribe Key, Publish Key, and UUID
3. Start streaming data and managing real-time interactions from your MCP-compatible client

### Who is this for?

- **IoT Developers** — Monitor device heartbeats and send control commands via real-time channels.
- **Support Teams** — Inspect chat history and user presence to provide better live assistance.
- **System Architects** — Audit channel metadata and monitor keyset metrics directly from the AI interface.


## Available Tools (31)
- **delete_message_history**: Delete message history for channels
- **generate_file_upload_url**: Generate a file upload URL
- **get_all_users**: Get all users (App Context)
- **get_channel**: Get a specific channel (App Context)
- **get_file_url**: Get a file URL
- **get_memberships**: Get memberships for a user (App Context)
- **get_user**: Get a specific user (App Context)
- **get_message_history**: Get message history for channels
- **list_files**: List files in a channel
- **get_message_count**: Get message count for channels
- **pam_grant_token**: Grant a PAM v3 token
- **pam_revoke_token**: Revoke a PAM v3 token
- **presence_get_state**: Get presence state for a user in a channel
- **presence_heartbeat**: Send presence heartbeat
- **presence_here_now**: Get current channel occupancy (Here Now)
- **presence_leave**: Leave a channel (Presence)
- **presence_set_state**: Set presence state for a user in a channel
- **presence_where_now**: Get channels a user is in (Where Now)
- **publish_message**: Publish a message to a channel
- **push_manage**: Manage or list push notification channels for a device (APNS v2)
- **push_remove_all**: Remove all push notification channels for a device (APNS v2)
- **remove_user**: Remove a user (App Context)
- **set_channel**: Set or update a channel (App Context)
- **set_memberships**: Set or update memberships for a user (App Context)
- **set_user**: Set or update a user (App Context)
- **admin_create_app**: Create a new PubNub app (Admin API)
- **admin_get_metrics**: Get usage metrics (Admin API)
- **admin_list_apps**: List all PubNub apps (Admin API)
- **admin_list_keysets**: List all keysets (Admin API)
- **delete_file**: Delete a file from a channel
- **get_all_channels**: Get all channels (App Context)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PubNub (Real-time Messaging)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Publish a message to the 'alerts' channel saying 'System update scheduled for midnight'."

**🤖 AI Agent:**
> I've published the message to the 'alerts' channel. The timetoken for this message is 17156348210000000.

---

**👤 You:**
> "Get the last 5 messages from the 'support-chat' channel."

**🤖 AI Agent:**
> I retrieved the last 5 messages from 'support-chat'. They include inquiries about billing and a technical setup question from user UUID-987.

---

**👤 You:**
> "Who is currently active in the 'lobby' channel?"

**🤖 AI Agent:**
> There are currently 3 users in the 'lobby' channel: 'admin-01', 'user-55', and 'guest-12'.


## ❓ FAQ

**Q: How can I check if a specific user is currently online in a channel?**
You can use the `presence_here_now` tool to see a list of all active UUIDs in a specific channel, or `presence_where_now` to find all channels a specific UUID is currently subscribed to.

**Q: Can the AI retrieve past messages from a channel?**
Yes, the `get_message_history` tool allows the agent to fetch historical messages from one or more channels, including metadata and specific time ranges.

**Q: Is it possible to manage user profiles and metadata through this server?**
Absolutely. You can use `set_user` to create or update profiles and `get_user` to retrieve them. You can also manage channel metadata using `set_channel` and `get_channel`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pubnub-real-time-messaging](https://vinkius.com/mcp/pubnub-real-time-messaging)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PubNub (Real-time Messaging)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pubnub-real-time-messaging` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PubNub (Real-time Messaging)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pubnub-real-time-messaging": {
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
