# Jellyfin (Plex Alternative) MCP Server

Manage your media library via Jellyfin — list movies, shows, and music, track playback progress, and inspect server status directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/jellyfin-plex-alternative)

## Overview
**Category:** loved-by-devs
**Tools Count:** 12

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


## Installation & Usage

To install and use the **Jellyfin (Plex Alternative)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jellyfin-plex-alternative](https://vinkius.com/mcp/jellyfin-plex-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
