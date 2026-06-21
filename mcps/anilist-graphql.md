# AniList GraphQL MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/anilist-graphql)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/anilist-graphql-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/anilist-graphql-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the world's largest anime and manga database — search titles, characters, staff, and manage your personal lists via GraphQL.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AniList GraphQL** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the anime 'Cowboy Bebop' and show its details."

**🤖 AI Agent:**
> I found 'Cowboy Bebop' (ID: 1). It's a classic Sci-Fi/Action series by Sunrise. Would you like to see the full character list or the airing history?

---

**👤 You:**
> "Who is the character 'L' from Death Note?"

**🤖 AI Agent:**
> Using `get_character`, I found L Lawliet. He is a world-renowned detective who takes on the challenge of catching the serial killer known as Kira. Would you like to see his voice actors?

---

**👤 You:**
> "Show me information about the animation studio MAPPA."

**🤖 AI Agent:**
> I've retrieved the data for Studio MAPPA (ID: 569) using `get_studio`. They are known for works like 'Jujutsu Kaisen' and 'Attack on Titan: The Final Season'.


## Installation & Usage

To install and use the **AniList GraphQL** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/anilist-graphql](https://vinkius.com/mcp/anilist-graphql)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
