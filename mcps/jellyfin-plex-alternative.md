# Jellyfin (Plex Alternative) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jellyfin-plex-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage your media library via Jellyfin — list movies, shows, and music, track playback progress, and inspect server status directly from any AI agent.

## Description
Connect your **Jellyfin** media server to any AI agent and take full control of your media library through natural conversation.

### What you can do

- **Library Navigation** — Use `list_virtual_folders` to see your root libraries and `list_items` to browse movies, shows, and music.
- **Detailed Metadata** — Retrieve specific item details, including descriptions and IDs, using `get_item`.
- **Playback Tracking** — Monitor and update media playback status with `session_playing` and `session_playing_progress`.
- **Server Monitoring** — Check server version, OS, and configuration using `get_system_info`.
- **User Management** — List and authenticate users via `list_users` and `authenticate_by_name`.

### How it works

1. Subscribe to this server
2. Enter your Jellyfin Server URL and API Key
3. Start managing your media from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Media Enthusiasts** — browse and manage your self-hosted collection without leaving your AI chat
- **Home Lab Users** — monitor server health and system info directly from the terminal or AI agent
- **Developers** — test Jellyfin API interactions and metadata retrieval through natural language


## Available Tools
- **authenticate_by_name**: Authenticate a user by name and password
- **get_current_user**: Get information about the currently logged-in user
- **get_item**: Get detailed information about a specific item
- **get_playback_info**: Retrieve information required to start playback
- **list_items**: Query for items in the library
- **list_users**: List all users (Admin only)
- **list_virtual_folders**: List the root libraries (Movies, TV Shows, etc.)
- **session_playing_progress**: Update the server on current playback position
- **session_playing_stopped**: Notify the server that playback has ended
- **session_playing**: Notify the server that playback has started
- **get_system_configuration**: Get the server global configuration
- **get_system_info**: Get basic server information (version, operating system, etc.)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jellyfin (Plex Alternative)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the root libraries on my Jellyfin server."

**🤖 AI Agent:**
> I've retrieved your root libraries. You have 'Movies' (ID: 1a2b), 'TV Shows' (ID: 3c4d), and 'Music' (ID: 5e6f) configured.

---

**👤 You:**
> "Show me the movies available in my library."

**🤖 AI Agent:**
> Fetching movies... I found titles including 'Big Buck Bunny' and 'Elephants Dream'. Would you like details for any of these?

---

**👤 You:**
> "What is the current status and version of my Jellyfin server?"

**🤖 AI Agent:**
> Your Jellyfin server is running version 10.9.11 on Linux. The system is healthy and all services are operational.


## ❓ FAQ

**Q: Can I filter my library to only show Movies or Series?**
Yes! Use the `list_items` tool and provide 'Movie' or 'Series' in the `include_item_types` parameter to filter your results accordingly.

**Q: How do I check if my Jellyfin server is running the latest version?**
You can use the `get_system_info` tool. It returns the server version, operating system, and other vital system metrics.

**Q: Can I see all the root libraries configured on my server?**
Absolutely. Run the `list_virtual_folders` tool to retrieve a list of all top-level libraries like Movies, TV Shows, and Music.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jellyfin-plex-alternative](https://vinkius.com/mcp/jellyfin-plex-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jellyfin (Plex Alternative)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `jellyfin-plex-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jellyfin (Plex Alternative)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jellyfin-plex-alternative": {
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
