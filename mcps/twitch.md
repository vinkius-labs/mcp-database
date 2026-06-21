# Twitch MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/twitch)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Twitch channel — audit streams, followers, and clips via AI.

## Description
Empower your AI agent to orchestrate your entire streaming ecosystem on **Twitch**, the world's leading live streaming platform. By connecting Twitch to your agent, you transform complex channel management into a natural conversation. Your agent can instantly list live streams, audit your follower base, and retrieve top clips without you ever touching a dashboard. Whether you are a full-time creator or a community manager, your agent acts as a real-time channel coordinator, ensuring your community engagement is always monitored and your content library is organized.

### What you can do

- **Stream Auditing** — List live streams by user or game and retrieve real-time viewer counts and statuses.
- **Community Oversight** — Query your follower base, audit channel moderators, and check subscriber details instantly.
- **Content Management** — List all videos and top clips for any broadcaster to stay on top of your highlights.
- **Channel Intelligence** — Retrieve detailed metadata for channels and users to maintain strict organizational control.
- **Discovery Monitoring** — Search for channels and list top games to understand platform trends in real-time.

### How it works

1. Subscribe to this server
2. Enter your Twitch Client ID and Access Token
3. Start managing your channel data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Twitch Streamers** — monitor live stats and follower growth straight from your creation workflow.
- **Community Managers** — verify moderator lists and audit subscriber counts without manual dashboard logins.
- **Content Strategists** — perform rapid audits of top clips and trending games to plan your next broadcast.
- **Operations Leads** — automate channel querying to orchestrate cross-functional creator teams smoothly.


## Available Tools (10)
- **get_followed_channels**: Get channels followed by a user
- **get_channel_followers**: Get followers for a channel
- **get_channel_info**: Get channel information
- **get_clips**: Get clips for a broadcaster
- **get_streams**: Get live streams
- **get_subscriptions**: Get broadcaster subscriptions
- **get_top_games**: Get top games on Twitch
- **get_users**: Get information about Twitch users
- **get_videos**: Get videos for a user
- **search_channels**: Search for Twitch channels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Twitch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if user 'ninja' is currently live on Twitch."

**🤖 AI Agent:**
> Checking status... Yes, 'Ninja' is currently live! He is streaming 'Fortnite' to 15,000 viewers. Would you like the stream link?

---

**👤 You:**
> "Show me the top 5 games on Twitch right now."

**🤖 AI Agent:**
> The top 5 games currently are: 'Just Chatting', 'League of Legends', 'Grand Theft Auto V', 'VALORANT', and 'Counter-Strike'. Which game would you like to see live streams for?

---

**👤 You:**
> "List the last 5 videos for broadcaster ID 12345."

**🤖 AI Agent:**
> I've retrieved the recent videos for ID 12345. You have 5 archives, including 'Tuesday Night Chill' and 'Ranked Climb'. Would you like the duration and view count for any of them?


## ❓ FAQ

**Q: How do I find my Twitch Client ID and Access Token?**
Go to the [**Twitch Developer Console**](https://dev.twitch.tv/console), create an App, and generate a Client Secret to get an App Access Token or perform the OAuth flow for a User Token. Copy and paste them below.

**Q: Can the agent check if a channel is live?**
Yes. Use the `get_streams` tool providing the user login. Your agent will return real-time status, including viewer count and game title if the channel is live.

**Q: Is it possible to list top clips via the agent?**
Yes. The `get_clips` tool allows your agent to retrieve the most popular clips for a specific broadcaster, helping you identify trending content moments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/twitch](https://vinkius.com/mcp/twitch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Twitch** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `twitch` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Twitch** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "twitch": {
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
