# Liveblocks MCP Server

Manage real-time collaboration infrastructure—create rooms, authorize users, and inspect collaborative storage or threads directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/liveblocks)

## Overview
**Category:** productivity
**Tools Count:** 18

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


## Installation & Usage

To install and use the **Liveblocks** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/liveblocks](https://vinkius.com/mcp/liveblocks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
