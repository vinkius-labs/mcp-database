# Last.fm MCP Server

Manage your music profile via Last.fm — get track metadata, scrobble songs, update your now playing status, and query user profiles.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/lastfm-alternative)

## Overview
**Category:** audio-music
**Tools Count:** 5

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


## Installation & Usage

To install and use the **Last.fm** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lastfm-alternative](https://vinkius.com/mcp/lastfm-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
