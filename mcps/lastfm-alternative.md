# Last.fm MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lastfm-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lastfm-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lastfm-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Manage your music profile via Last.fm — get track metadata, scrobble songs, update your now playing status, and query user profiles.

## Description
Connect your **Last.fm** account to any AI agent and take control of your music scrobbling and metadata discovery through natural conversation.

### What you can do

- **Track Metadata** — Fetch detailed information for any track using `get_track_info`, including playcounts and artist details.
- **Scrobbling** — Log your listening history with `scrobble_track` to keep your profile up to date.
- **Now Playing** — Use `update_now_playing` to notify your followers of what you're currently listening to.
- **User Insights** — Retrieve profile data and stats for any user with `get_user_info`.
- **Tag Discovery** — Explore genres and music tags using `get_tag_info` to find new context for your favorite sounds.

### How it works

1. Subscribe to this server
2. Enter your Last.fm API Key and Shared Secret
3. Start managing your music profile from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Music Lovers** — scrobble tracks and check stats without opening a dedicated app.
- **Developers** — access rich music metadata directly within your coding environment.
- **Curators** — explore tags and user profiles to discover new trends and genres.


## Available Tools
- **update_now_playing**: fm that a user has started listening to a track. Requires session key.

Update Now Playing status on Last.fm
- **scrobble_track**: Requires session key. Track must be > 30s and played for at least half its duration or 4 mins.

Scrobble a track to Last.fm
- **get_tag_info**: fm.

Get metadata for a tag
- **get_track_info**: fm using artist and track name, or MBID.

Get metadata for a track
- **get_user_info**: fm user.

Get information about a user profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Last.fm** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get metadata for the track 'Blinding Lights' by The Weeknd."

**🤖 AI Agent:**
> I've fetched the info for 'Blinding Lights'. It has over 500 million plays on Last.fm and is part of the album 'After Hours'. Would you like to see the artist's top tags?

---

**👤 You:**
> "Update my now playing status to 'Levitating' by Dua Lipa."

**🤖 AI Agent:**
> Successfully updated your status! Your Last.fm profile now shows you are listening to 'Levitating' by Dua Lipa.

---

**👤 You:**
> "Show me the profile details for user 'music_fan_123'."

**🤖 AI Agent:**
> I've retrieved the profile for 'music_fan_123'. They have been a member since 2015 and have a total playcount of 45,000 tracks. Their top artist is Radiohead.


## Installation & Usage

To install and use the **Last.fm** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lastfm-alternative](https://vinkius.com/mcp/lastfm-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
