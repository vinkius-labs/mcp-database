# Twitch MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/twitch)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/twitch-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/twitch-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Twitch** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/twitch](https://vinkius.com/mcp/twitch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
