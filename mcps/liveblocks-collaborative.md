# Liveblocks (Collaborative) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/liveblocks-collaborative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage real-time collaborative rooms, user presence, and shared storage via Liveblocks — list rooms, track active users, and handle threads directly from your AI agent.

## Description
Connect your **Liveblocks** account to any AI agent to orchestrate real-time collaborative experiences and manage infrastructure through natural conversation.

### What you can do

- **Room Lifecycle** — Create, list, update, and delete collaborative rooms with custom metadata and access controls.
- **Presence & Interaction** — Monitor active users in any room, set ephemeral presence, and broadcast custom events to connected clients.
- **Data Synchronization** — Retrieve and patch room storage or Yjs documents to manage shared state across collaborative sessions.
- **Comments & Feedback** — Manage collaborative threads, create new discussions, and resolve existing ones to streamline team feedback.
- **User Identity** — Authorize and identify users with specific permissions and group assignments via secure token generation.

### How it works

1. Subscribe to this server
2. Enter your Liveblocks Secret Key from the dashboard
3. Start managing your real-time infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — Monitor active collaboration sessions and review user feedback threads without leaving the chat interface.
- **Full-stack Developers** — Debug room storage, inspect Yjs document states, and manage room permissions directly from the IDE.
- **Support Teams** — Quickly identify active users in a room and verify room configurations to assist customers in real-time.


## Available Tools (19)
- **list_active_users**: List users currently in the room
- **authorize_user**: Obtain an access token with specific permissions
- **broadcast_event**: Broadcast a JSON event to a room
- **create_room**: Create a new room
- **create_thread**: Create a thread and the first comment
- **delete_room**: Delete a room
- **get_room**: Retrieve room details
- **get_storage**: Get the room's Storage tree (LSON or JSON format)
- **get_ydoc**: Get a JSON representation of the Yjs document
- **identify_user**: Obtain an ID token for a user
- **initialize_storage**: Initialize or reinitialize Storage
- **list_rooms**: List rooms with filtering and pagination
- **list_threads**: List threads in a room
- **list_versions**: List Yjs version history snapshots
- **patch_storage**: Apply JSON Patch operations to Storage
- **resolve_thread**: Resolve a thread
- **set_presence**: Set ephemeral presence for a user/agent
- **update_room**: Update room properties (metadata, permissions)
- **update_ydoc**: Send a binary Yjs update


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Liveblocks (Collaborative)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Liveblocks rooms created after January 1st with the metadata 'status:active'."

**🤖 AI Agent:**
> I've found 3 rooms matching your criteria: 'Project-Alpha' (ID: room_01), 'Design-Sprint' (ID: room_05), and 'Team-Sync' (ID: room_09). Would you like to see the active users for any of these?

---

**👤 You:**
> "Check who is currently collaborating in room 'editor-prod-42'."

**🤖 AI Agent:**
> There are currently 2 active users in 'editor-prod-42': 'Alice (ID: user_A)' and 'Bob (ID: user_B)'. Alice has been connected for 15 minutes.

---

**👤 You:**
> "Create a new collaborative room for 'Sprint 24 Planning' with default access set to 'room:write'."

**🤖 AI Agent:**
> Room 'Sprint 24 Planning' has been successfully created with ID 'sprint-24-plan'. Default access is set to write. You can now start adding threads or initializing storage.


## ❓ FAQ

**Q: How can I see which users are currently active in a specific collaboration room?**
You can use the `list_active_users` tool by providing the Room ID. The agent will return a list of all users currently connected to that room, including their connection IDs and associated info.

**Q: Is it possible to inspect or modify the shared state of a room from the AI?**
Yes! Use `get_storage` to retrieve the current LSON/JSON storage tree or `patch_storage` to update specific keys in the room's shared state. For Yjs-based rooms, you can use `get_ydoc` and `update_ydoc`.

**Q: Can I manage user comments and discussion threads through this integration?**
Absolutely. You can use `list_threads` to see all discussions in a room, `create_thread` to start a new one, and `resolve_thread` to mark a discussion as completed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/liveblocks-collaborative](https://vinkius.com/mcp/liveblocks-collaborative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Liveblocks (Collaborative)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `liveblocks-collaborative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Liveblocks (Collaborative)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "liveblocks-collaborative": {
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
