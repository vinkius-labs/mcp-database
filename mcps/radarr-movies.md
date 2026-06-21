# Radarr (Movies) MCP Server

Manage your movie library, search for new titles, and monitor download queues via Radarr.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/radarr-movies)

## Overview
**Category:** content-management
**Tools Count:** 15

## Description
Connect your **Radarr** instance to any AI agent to take full control of your movie collection and PVR workflows through natural conversation.

### What you can do

- **Library Management** — List all movies in your collection, fetch detailed metadata, and update movie configurations.
- **Discovery & Search** — Search for new movies using TMDB integration and add them to your library with specific quality profiles.
- **Download Monitoring** — Track your active download queue, view history of grabs/imports, and manage queue items.
- **System Operations** — Check disk space, system status, and execute internal commands like library refreshes.
- **Infrastructure Mapping** — Retrieve root folders and quality profiles to ensure correct organization of your media files.

### How it works

1. Subscribe to this server
2. Enter your Radarr URL and API Key
3. Start managing your media library from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Home Lab Enthusiasts** — manage your media server without opening the web UI
- **Content Collectors** — quickly search and add movies to your watchlist via chat
- **System Administrators** — monitor disk space and download health across your media stack


## Available Tools
- **add_movie**: Requires TMDB ID, quality profile, and root folder path.

Add a new movie to Radarr
- **delete_movie**: Remove a movie from Radarr
- **delete_queue_item**: Remove an item from the download queue
- **execute_command**: g., RescanMovie, MovieSearch, RefreshMovie, RenameMovie).

Execute a specific system command
- **get_commands**: List active or recently completed commands
- **get_disk_space**: Get disk space information
- **get_history**: View the history of grabs and imports
- **get_movie**: Get details for a specific movie
- **get_quality_profiles**: g., HD-1080p, Ultra-HD) configured in Radarr.

Get available quality profiles
- **get_queue**: Get the current download queue
- **get_root_folders**: Get configured root folders
- **get_system_status**: Get Radarr system status
- **list_movies**: List all movies in the Radarr library
- **lookup_movie**: g., "term=Inception" or "term=tmdb:27205").

Search for movies to add to Radarr
- **update_movie**: Provide the full movie object payload.

Update an existing movie in Radarr


## Installation & Usage

To install and use the **Radarr (Movies)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/radarr-movies](https://vinkius.com/mcp/radarr-movies)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
