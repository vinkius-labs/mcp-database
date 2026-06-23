# SoundCloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/soundcloud)
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


## Available Tools (8)
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


## ❓ FAQ

**Q: How do I find my SoundCloud Client ID and Access Token?**
Log in to the [**SoundCloud Developer Portal**](https://developers.soundcloud.com/), create an App to get a Client ID, and perform the OAuth flow to generate an Access Token. Copy and paste them below.

**Q: Can the agent list my private tracks?**
Yes. If your Access Token has the necessary permissions, your agent will be able to retrieve both public and private tracks associated with your account.

**Q: Is it possible to search for tracks via the agent?**
Yes. The `search_tracks` tool allows your agent to query the entire SoundCloud public library using any search string, returning matching track metadata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/soundcloud](https://vinkius.com/mcp/soundcloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SoundCloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `soundcloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SoundCloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "soundcloud": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
