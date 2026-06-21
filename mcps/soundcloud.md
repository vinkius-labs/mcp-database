# SoundCloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/soundcloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/soundcloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/soundcloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your SoundCloud account — audit tracks, playlists, and followers via AI.

## Description
Empower your AI agent to orchestrate your entire audio ecosystem on **SoundCloud**, the world's largest open audio platform. By connecting SoundCloud to your agent, you transform complex track management into a natural conversation. Your agent can instantly list your uploads, audit playlist organization, and retrieve follower stats without you ever touching a dashboard. Whether you are an independent artist or a podcast producer, your agent acts as a real-time audio operator, ensuring your content is always organized and your community reach is monitored.

### What you can do

- **Track Auditing** — List all tracks in your account and retrieve detailed metadata, including duration, genre, and permalink URLs.
- **Playlist Oversight** — Browse your playlists to maintain a clear view of your track categorization and curation.
- **Community Management** — List your followers and following lists to stay on top of your community growth.
- **Favorites & Discovery** — Query your favorited tracks and search the global SoundCloud library for inspiration or collaboration.
- **Profile Intelligence** — Retrieve detailed user information and account details to maintain strict organizational control.

### How it works

1. Subscribe to this server
2. Enter your SoundCloud Client ID and Access Token
3. Start managing your audio assets through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Musicians & Artists** — monitor track performance and follower growth straight from your production workflow.
- **Podcasters** — verify if new episodes have been correctly added to playlists and are public.
- **Curation Leads** — perform rapid audits of track libraries and manage playlist organization without manual logins.
- **Operations Managers** — automate audio querying to orchestrate cross-functional creative teams smoothly.


## Available Tools
- **get_me**: Get authenticated user info from SoundCloud
- **get_track**: Get details for a specific track
- **list_favorites**: List favorited tracks for a user
- **list_followers**: List followers for a user
- **list_following**: List users followed by a user
- **list_playlists**: List playlists for a user
- **list_tracks**: List tracks for a user
- **search_tracks**: Search for public tracks on SoundCloud


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SoundCloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 tracks in my SoundCloud account."

**🤖 AI Agent:**
> I've retrieved your recent tracks. You have 5 uploads, including 'Midnight Jam' and 'Session 42'. Would you like the duration and play counts for any of them?

---

**👤 You:**
> "Show me my SoundCloud playlists."

**🤖 AI Agent:**
> You have 3 playlists in your account: 'Chill Beats', 'Workout Mix', and 'Demos'. I can list the tracks inside any of these playlists for you.

---

**👤 You:**
> "How many followers do I have on SoundCloud?"

**🤖 AI Agent:**
> Checking your audience... You currently have 250 followers. I can list the most recent ones for you if you'd like.


## Installation & Usage

To install and use the **SoundCloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/soundcloud](https://vinkius.com/mcp/soundcloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
