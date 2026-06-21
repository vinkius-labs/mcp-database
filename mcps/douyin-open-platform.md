# Douyin Open Platform MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/douyin-open-platform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/douyin-open-platform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/douyin-open-platform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Orchestrate Douyin (TikTok China) content — manage videos, handle comments, and track user analytics directly from any AI agent.

## Description
Connect your AI agents to the **Douyin Open Platform**, the primary ecosystem for short-video content and social engagement in China. This MCP provides 10 tools to automate video library management, comment moderation, and deep audience analytics directly through natural conversation.

### What you can do

- **Video Management** — List uploaded content and retrieve granular performance metrics like play counts and engagement rates
- **Community Interaction** — Monitor video comments and reply to followers to maintain active social presence
- **User Insights** — Access authorized user profiles, follower lists, and demographic distributions
- **Data Analytics** — Track historical live streaming statistics and fan growth trends for data-driven decisions
- **Content Discovery** — Search for public videos and trending content using specific keywords

### How it works

1. Subscribe to this server
2. Log in to the [**Douyin Developer Platform**](https://developer.open-douyin.com/)
3. Create an application and obtain your **Client Key** and **Client Secret**
4. Apply for necessary scopes (e.g., `video.list`, `video.data`, `item.comment`)
5. Generate a **User Access Token** via the OAuth 2.0 flow
6. Insert your credentials and token into the fields below to start managing your Douyin ecosystem.

### Who is this for?

- **Content Creators** — automate the monitoring of video performance and engagement across multiple accounts
- **Marketing Agencies** — retrieve demographic data and social trends for the Chinese market
- **Social Media Managers** — manage large volumes of comments and interact with fans efficiently


## Available Tools
- **get_audience_analytics**: Retrieve demographic data for account followers
- **get_live_analytics**: Retrieve historical live streaming data
- **get_user_info**: Retrieve authorized user profile details
- **get_video_analytics**: Retrieve performance metrics for specific videos
- **list_comments**: List comments for a specific video
- **list_fans**: List fans/followers of the authorized user
- **list_following**: List users that the authorized user is following
- **list_videos**: List videos uploaded by the authorized user
- **reply_comment**: Reply to a comment on a video
- **search_videos**: Search for public videos on Douyin


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Douyin Open Platform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 videos uploaded to my Douyin account and show their play counts."

**🤖 AI Agent:**
> I've retrieved your recent videos. 1. 'Spring Collection' (15.4K views), 2. 'Behind the Scenes' (8.2K views), 3. 'Q&A Session' (12.1K views)... Would you like to see the demographic breakdown for any of these?

---

**👤 You:**
> "Show me the comments for video ID 'item_abc123'."

**🤖 AI Agent:**
> Fetching comments for video 'Tech Review'... I found several top comments: 1. 'Great video!' (120 likes), 2. 'Where can I buy this?' (85 likes), 3. 'Love the editing' (42 likes). Would you like to reply to any of these?

---

**👤 You:**
> "Search for videos matching 'robotics' on Douyin."

**🤖 AI Agent:**
> Searching the Douyin public feed... I've found 3 trending videos about robotics: 1. 'Humanoid Robot Demo', 2. 'DIY Robot Arm', 3. 'Boston Dynamics Update'. Which one would you like to explore?


## Installation & Usage

To install and use the **Douyin Open Platform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/douyin-open-platform](https://vinkius.com/mcp/douyin-open-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
