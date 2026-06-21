# Liveblocks MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/liveblocks)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage real-time collaboration infrastructure—create rooms, authorize users, and inspect collaborative storage or threads directly from your AI agent.

## Description
Connect your **Liveblocks** account to any AI agent to orchestrate multiplayer experiences and real-time collaboration features through natural language.

### What you can do

- **Room Management** — List, create, update, and delete rooms to manage your application's collaborative spaces.
- **User Authentication** — Generate access tokens and identify users with specific permissions using `authorize_user` and `identify_user`.
- **Collaborative Storage** — Inspect and patch room storage state or manage Yjs documents for shared editing.
- **Comments & Threads** — Query, create, and resolve comment threads to keep track of team discussions within rooms.
- **Real-time Presence** — List active users in a room or broadcast custom events to connected clients.

### How it works

1. Subscribe to this server
2. Enter your Liveblocks Secret Key
3. Start managing your real-time infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Full-stack Developers** — quickly debug room storage, manage user permissions, or clear stale rooms without leaving the terminal or IDE.
- **Product Managers** — monitor active collaboration sessions and review comment threads across different project rooms.
- **DevOps Engineers** — automate the provisioning of collaborative environments and manage access rules programmatically.


## Available Tools
- **authorize_user**: Obtain an access token for a client to enter a room
- **broadcast_event**: Broadcast a JSON event to a room
- **create_room**: Create a new room
- **create_thread**: Create a thread and the first comment
- **delete_room**: Delete a room
- **get_room**: Retrieve room details
- **get_storage**: Get the room's Storage tree
- **get_thread**: Get a specific thread
- **get_ydoc**: Get a JSON representation of the Yjs document
- **identify_user**: Permissions are managed on the backend.

Obtain an ID token for a client
- **initialize_storage**: Initialize or reinitialize Storage
- **list_active_users**: List users currently in the room
- **list_rooms**: Can be filtered by metadata or access.

List rooms with filtering and pagination
- **list_threads**: List threads in a room
- **patch_storage**: Apply JSON Patch operations to Storage
- **resolve_thread**: Resolve a thread
- **update_room**: Update room properties
- **update_ydoc**: Send a binary Yjs update


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Liveblocks** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 10 rooms in my Liveblocks project."

**🤖 AI Agent:**
> I've retrieved your rooms. You have active rooms like 'main-editor', 'collaboration-hub', and 'test-room-1'. Would you like to see the metadata for any of these?

---

**👤 You:**
> "Create a new room with ID 'sprint-planning' and set default access to room:write."

**🤖 AI Agent:**
> Room 'sprint-planning' has been successfully created with 'room:write' as the default access level. You can now start authorizing users for this space.

---

**👤 You:**
> "Who is currently active in the room 'main-editor'?"

**🤖 AI Agent:**
> Checking active users... I found 3 users currently connected to 'main-editor': 'alice_dev', 'bob_designer', and 'charlie_pm'.


## ❓ FAQ

**Q: How can I filter rooms by specific metadata using the AI?**
You can ask the agent to use the `list_rooms` tool and provide a JSON string in the metadata parameter. For example, ask to 'List rooms where the project metadata is alpha'.

**Q: Can I generate a temporary access token for a user to join a room?**
Yes. Use the `authorize_user` tool. Provide the Room ID and User ID, and the agent will return a token that grants access to that specific room.

**Q: Is it possible to permanently delete a room and its data?**
Yes, the `delete_room` tool allows you to permanently remove a room and all associated storage, comments, and metadata. Use this with caution as it is irreversible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/liveblocks](https://vinkius.com/mcp/liveblocks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Liveblocks** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `liveblocks` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Liveblocks** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "liveblocks": {
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
