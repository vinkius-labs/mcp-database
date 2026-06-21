# Sonarr (TV) MCP Server

Automate TV library management via Sonarr — list series, track episodes, and monitor download queues directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sonarr-tv)

## Overview
**Category:** productivity
**Tools Count:** 18

## Description
Connect your **Sonarr** instance to any AI agent to take full control of your TV media library through natural conversation.

### What you can do

- **Library Management** — List all series, add new shows via TVDB ID, and update monitoring status or quality profiles.
- **Episode Tracking** — Fetch details for specific episodes, list all episodes in a series, and manage their monitored state.
- **File Control** — List and delete physical episode files directly from your storage to manage disk space.
- **Activity Monitoring** — Access download history and current queue status to see what's downloading or stalled.
- **System Health** — Check Sonarr's connectivity, system status, and internal health metrics to ensure smooth operation.

### How it works

1. Subscribe to this server
2. Enter your Sonarr URL and API Key
3. Start managing your media library from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Media Enthusiasts** — manage your library, check episode statuses, and clean up files without opening the web interface
- **Home Lab Users** — automate show tracking and monitor download health via simple chat commands
- **Automation Fans** — integrate your media server workflows into your daily AI assistant routines


## Available Tools
- **add_series**: Adds a new series to the library
- **delete_episode_file**: Deletes an episode file from disk
- **delete_queue_item**: Removes an item from the queue
- **delete_series**: Removes a series from the library
- **get_episode_file**: Returns a specific episode file
- **get_episode**: Returns a specific episode by its ID
- **get_health**: Returns any health check warnings or errors
- **get_history**: Access the history of grabbed and imported episodes
- **get_queue**: Returns all items in the download queue
- **get_series**: Returns a specific series by its ID
- **get_system_status**: Returns system information (version, OS, paths)
- **list_commands**: Returns all currently running commands
- **list_episode_files**: Returns all episode files for a series
- **list_episodes**: Returns all episodes for a specific series
- **list_series**: Returns all series in the library
- **start_command**: g., SeriesSearch, RescanSeries, RefreshSeries).

Starts a new command
- **update_episode**: Updates an episode (e.g., marking it as monitored)
- **update_series**: Updates an existing series


## Installation & Usage

To install and use the **Sonarr (TV)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sonarr-tv](https://vinkius.com/mcp/sonarr-tv)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
