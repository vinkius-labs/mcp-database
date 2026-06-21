# Audiomack Music MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/audiomack-music)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/audiomack-music-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/audiomack-music-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Explore and discover music via Audiomack — search for songs, albums, and trending artists directly from any AI agent.

## Description
Connect your AI agent to **Audiomack**, the leading platform for artist-first music discovery. This integration allows you to browse millions of tracks, track trending charts, and inspect detailed profiles for your favorite artists through natural conversation.

### What you can do

- **Music Discovery** — Search for songs and albums by title, artist name, or genre
- **Trending Charts** — Access real-time trending lists for the most popular tracks and playlists
- **Artist Insights** — Retrieve comprehensive metadata, including bios and social links for verified artists
- **Catalog Oversight** — Explore the complete discography of any artist on the platform
- **Account Access** — Securely lookup details for your own Audiomack developer account

### How it works

1. Subscribe to this server
2. Enter your **Audiomack Consumer Key** and **Secret** (obtained from the Audiomack Developer Portal)
3. Start exploring the world of music via chat

This integration uses Audiomack's REST API with secure OAuth 1.0a signing for all requests.

### Who is this for?

- **Music Enthusiasts** — find and explore new music without leaving the chat
- **Content Creators** — quickly verify artist info and track metadata for reviews or curation
- **Music Researchers** — analyze trends and artist growth across different genres


## Available Tools
- **get_authenticated_account**: Retrieve information about the authenticated Audiomack account
- **get_album_details**: Get detailed information for a specific album
- **get_artist_details**: Get comprehensive information for a specific artist
- **get_artist_music**: List all songs or albums for a specific artist
- **get_trending_music**: Retrieve the currently trending music on Audiomack
- **search_music**: Search for songs, albums, or artists on Audiomack


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Audiomack Music** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the latest trending songs on Audiomack."

**🤖 AI Agent:**
> Fetching trending songs... I found several popular tracks, including 'Million Dollar Baby' and 'Not Like Us'. Which one would you like more details on?

---

**👤 You:**
> "Show me the discography for artist 'Eminem'."

**🤖 AI Agent:**
> Retrieving data for Eminem... He has several albums available on Audiomack, including 'The Slim Shady LP', 'The Marshall Mathers LP', and 'The Eminem Show'.

---

**👤 You:**
> "Get details for the artist 'Kendrick Lamar' on Audiomack."

**🤖 AI Agent:**
> Inspecting Kendrick Lamar's profile... He is a verified artist with millions of plays. I've found his biography and links to his verified social profiles. Would you like to see his top trending tracks?


## Installation & Usage

To install and use the **Audiomack Music** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/audiomack-music](https://vinkius.com/mcp/audiomack-music)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
