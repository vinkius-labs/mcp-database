# Freesound MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freesound)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/freesound-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/freesound-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Search, download, and manage audio samples from the Freesound database directly within your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freesound** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for high-quality cinematic impact sounds on Freesound."

**🤖 AI Agent:**
> I found several cinematic impact sounds. The top result is 'Heavy Cinematic Hit' (ID: 12345) with tags like 'impact', 'cinematic', and 'bass'. Would you like to see more details or download it?

---

**👤 You:**
> "Get the metadata and tags for sound ID 45678."

**🤖 AI Agent:**
> Sound 45678 is titled 'Electric Hum'. It is a 44.1kHz WAV file with tags: 'noise', 'electronic', 'loop'. It has been downloaded 1,200 times.

---

**👤 You:**
> "Show me the sounds uploaded by user 'audio_pro'."

**🤖 AI Agent:**
> User 'audio_pro' has uploaded 12 sounds, including 'Studio Kick' and 'Snare Hit'. Would you like the specific IDs or descriptions for these sounds?


## Installation & Usage

To install and use the **Freesound** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freesound](https://vinkius.com/mcp/freesound)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
