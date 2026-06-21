# Freesound MCP Server

Search, download, and manage audio samples from the Freesound database directly within your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/freesound)

## Overview
**Category:** design-creative
**Tools Count:** 10

## Description
Connect your **Freesound** account to any AI agent and access the world's largest collection of Creative Commons licensed audio samples through natural conversation.

### What you can do

- **Advanced Search** — Find specific sounds using text queries and Solr-style filters for duration, tags, or license types.
- **Metadata Retrieval** — Fetch detailed information, analysis, and tags for any sound or pack in the database.
- **User & Pack Insights** — Explore user profiles, their public uploads, and organized sound packs.
- **Audio Management** — Download high-quality original files, upload new recordings, and describe them with metadata directly from your workflow.
- **Moderation Tracking** — Check the status of your pending uploads and manage your personal library.

### How it works

1. Subscribe to this server
2. Enter your Freesound API Key or OAuth Token
3. Start searching and downloading audio from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sound Designers & Musicians** — Quickly find textures and samples without leaving your DAW or creative environment.
- **Game Developers** — Search for specific sound effects (SFX) and integrate them into your project assets instantly.
- **Content Creators** — Find the perfect background noise or transition effect using natural language descriptions.


## Available Tools
- **describe_sound**: Add metadata to an uploaded sound
- **download_sound**: Triggers a download of the original file.

Download the original high-quality sound file
- **get_me**: Get information about the currently authenticated OAuth2 user
- **get_pack**: Get information about a sound pack
- **get_pending_uploads**: Check status of sounds in moderation
- **get_sound**: Get details for a specific sound
- **get_user_sounds**: Get sounds uploaded by a specific user
- **get_user**: Get information about a Freesound user
- **search_sounds**: Supports Solr-style filters.

Search for sounds on Freesound
- **upload_sound**: Upload an audio file to Freesound


## Installation & Usage

To install and use the **Freesound** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freesound](https://vinkius.com/mcp/freesound)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
