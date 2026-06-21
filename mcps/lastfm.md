# Last.fm MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lastfm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lastfm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lastfm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your music profile — audit listening habits, top tracks, and artists via AI.

## Description
Empower your AI agent to orchestrate your entire music data ecosystem with **Last.fm**, the world's leading music discovery service. By connecting Last.fm to your agent, you transform complex listening analytics into a natural conversation. Your agent can instantly list your top tracks, audit your favorite artists, and retrieve detailed music metadata without you ever touching a dashboard. Whether you are a dedicated audiophile or a music researcher, your agent acts as a real-time curator, ensuring your musical taste is always quantified and trends are monitored.

### What you can do

- **Habit Auditing** — List recent tracks and query your most-listened artists, albums, and songs across flexible time periods.
- **Metadata Oversight** — Retrieve detailed information for any artist, album, or track to maintain a deep understanding of your library.
- **Discovery Monitoring** — Browse top tags and charts to identify global music trends and find new inspiration.
- **Engagement Management** — List your loved tracks to stay on top of your personal musical highlights.
- **Profile Intelligence** — Retrieve detailed user metadata and account info to maintain strict organizational control.

### How it works

1. Subscribe to this server
2. Enter your Last.fm API Key
3. Start managing your music data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Music Enthusiasts** — monitor listening stats and top charts straight from your workflow.
- **Curation Teams** — verify if track and artist metadata are correctly identified and categorized.
- **Research Analysts** — perform rapid audits of music trends and user habits without manual dashboard logins.
- **Operations Leads** — automate music querying to orchestrate cross-functional creative teams smoothly.


## Available Tools
- **get_album_info**: Get metadata for an album
- **get_artist_info**: Get metadata for an artist
- **get_loved_tracks**: Get the loved tracks for a user
- **get_recent_tracks**: Get the recent tracks listened to by a user
- **get_top_albums**: Get the top albums for a user
- **get_top_artists**: Get the top artists for a user
- **get_top_tags**: fm based on the provided unique identifier or parameters.

Get the top tags on Last.fm
- **get_top_tracks**: Get the top tracks for a user
- **get_track_info**: Get metadata for a track
- **get_user_info**: fm user.

Get information about a Last.fm user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Last.fm** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my top 5 tracks this month on Last.fm."

**🤖 AI Agent:**
> I've retrieved your top tracks for the last month. Your #1 song is 'Midnight Jam' by Virtual Band. Would you like the play counts for the rest of the list?

---

**👤 You:**
> "Show me my recent tracks for user 'vinkius'."

**🤖 AI Agent:**
> I've found your recent listening history. You just finished listening to 'Session 42'. I can provide the timestamps for the last 10 tracks if you like.

---

**👤 You:**
> "Get information about the artist 'Radiohead'."

**🤖 AI Agent:**
> I've retrieved the metadata for 'Radiohead'. They have over 5 million listeners on Last.fm. Would you like to see their top tags and summary biography?


## Installation & Usage

To install and use the **Last.fm** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lastfm](https://vinkius.com/mcp/lastfm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
