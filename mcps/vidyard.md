# Vidyard MCP Server

Manage video assets, players, and hosting on Vidyard — the leading video messaging platform for business.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/vidyard)

## Overview
**Category:** marketing-automation
**Tools Count:** 10

## Description
Connect your **Vidyard** account to any AI agent and manage your business video library through natural conversation.

### What you can do

- **Video Library** — List all video assets stored in your Vidyard dashboard and retrieve unique video IDs
- **Metadata & Details** — Get technical metadata for any video including length, encoding status, and descriptions
- **Player Management** — Create, update, and manage video players (facades) to customize how your content is embedded
- **Video Organization** — Attach videos to specific players and organize your content for different marketing or sales needs
- **Direct Stream Access** — Retrieve direct stream URLs and raw MP4 download links for various video qualities (480p, 720p, etc.)
- **Asset Management** — Rename players or permanently delete video assets and player containers from your dashboard

### How it works

1. Subscribe to this server
2. Enter your Vidyard API Token
3. Start managing your video library through Claude, Cursor, or any MCP-compatible client

No more manual browsing through complex video dashboards. Your AI agent becomes your video asset manager.

### Who is this for?

- **Marketing Teams** — organize video players for different campaigns and retrieve embed codes through chat
- **Sales Professionals** — quickly find and share specific videos or product demos with prospects
- **Content Creators** — manage video assets, check encoding status, and retrieve source files for distribution
- **Support Engineers** — find relevant tutorial videos and manage player branding for knowledge base articles


## Available Tools
- **create_empty_player**: Creates a new, empty video player container
- **delete_video_player**: Note that the original video assets are not deleted.

Permanently deletes a video player
- **delete_video_asset**: This action is irreversible.

Permanently deletes a video asset from Vidyard
- **get_video_source_files**: Retrieves direct stream URLs for various video qualities (480p, 720p, etc.)
- **get_player_details**: Retrieves details for a specific video player
- **get_video_details**: Retrieves technical metadata for a specific video asset
- **list_video_players**: Lists all configured video players (facades) in the account
- **list_videos**: Lists all video assets stored in the Vidyard dashboard
- **attach_video_to_player**: Requires both player ID and video ID.

Adds a video asset into a specific player container
- **update_player_name**: Updates the display name or title of an existing player


## Installation & Usage

To install and use the **Vidyard** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vidyard](https://vinkius.com/mcp/vidyard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
