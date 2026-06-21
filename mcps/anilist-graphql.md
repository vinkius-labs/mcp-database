# AniList GraphQL MCP Server

Access the world's largest anime and manga database — search titles, characters, staff, and manage your personal lists via GraphQL.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/anilist-graphql)

## Overview
**Category:** knowledge-management
**Tools Count:** 15

## Description
Connect your **AniList** account to any AI agent to explore the vast world of anime and manga. This MCP server leverages the AniList GraphQL API to provide deep insights into media, characters, and industry professionals.

### What you can do

- **Media Discovery** — Search for anime and manga titles, fetch detailed metadata, and check airing schedules using `search_media` and `get_media`.
- **Character & Staff Insights** — Retrieve comprehensive profiles for your favorite characters and the staff (voice actors, directors) behind them with `get_character` and `get_staff`.
- **User Profiles** — Access public user information or manage your own authenticated profile and lists using `get_user` and `get_viewer`.
- **Studio Information** — Look up animation studios and their production history via `get_studio`.

### How it works

1. Subscribe to this server
2. Enter your AniList Access Token (optional for public data, required for personal lists)
3. Start exploring the AniList database from Claude, Cursor, or any MCP client.

### Who is this for?

- **Anime Fans** — instantly retrieve series information, character bios, and voice actor details.
- **Content Creators** — gather accurate data for reviews, recommendations, or database management.
- **Developers** — integrate anime metadata directly into your coding environment for project context.


## Available Tools
- **delete_media_list_entry**: Delete a media list entry
- **get_airing_schedule**: Query airing schedule data
- **get_character**: Query a specific character
- **get_media**: Query a specific anime or manga
- **get_staff**: ).

Query a specific staff member
- **get_studio**: Query a specific studio
- **get_user**: Query a specific user
- **get_viewer**: Get the currently authenticated user
- **save_media_list_entry**: Create or update a media list entry
- **search_characters**: Search for characters
- **search_media**: Search for anime or manga
- **search_staff**: Search for staff members
- **toggle_favourite**: Toggle favorite status
- **toggle_follow**: Toggle following a user
- **update_user**: Update authenticated user settings


## Installation & Usage

To install and use the **AniList GraphQL** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/anilist-graphql](https://vinkius.com/mcp/anilist-graphql)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
