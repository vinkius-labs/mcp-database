# Pixelfed (Instagram Alternative) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pixelfed-instagram-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage your Pixelfed presence — post photos, interact with the community, and track notifications directly from any AI agent.

## Description
Connect your **Pixelfed** account to any AI agent to manage your decentralized photo-sharing feed through natural conversation.

### What you can do

- **Post & Media** — Create new statuses with text and upload media directly to your profile using `create_status` and `upload_media`.
- **Social Interaction** — Follow or unfollow accounts, like posts with `favourite_status`, and share content with `reblog_status`.
- **Timeline Access** — Browse your home feed, public timelines, or specific hashtag trends via `get_home_timeline` and `get_tag_timeline`.
- **Account Management** — Inspect account details, followers, and following lists with `get_account` and `get_followers`.
- **Notifications** — Stay updated with real-time notifications from your network using `get_notifications`.

### How it works

1. Subscribe to this server
2. Enter your Pixelfed Instance URL and Personal Access Token
3. Start sharing and interacting from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — automate posting schedules and monitor engagement without leaving your workspace
- **Social Media Managers** — track multiple decentralized feeds and interact with the community efficiently
- **Fediverse Enthusiasts** — stay connected to the decentralized web through a unified AI interface


## Available Tools (17)
- **create_status**: Supports text content, media IDs, and visibility settings.

Create a new post (status)
- **delete_status**: Delete a status (post)
- **favourite_status**: Favourite (like) a status
- **follow_account**: Follow an account
- **get_account**: Get details for a specific account
- **get_followers**: Get followers of an account
- **get_following**: Get accounts followed by an account
- **get_home_timeline**: Get home timeline
- **get_notifications**: Get notifications
- **get_public_timeline**: Get public timeline
- **get_status**: Get a specific status (post)
- **get_tag_timeline**: Get tag timeline
- **reblog_status**: Reblog (share) a status
- **unfavourite_status**: Unfavourite (unlike) a status
- **unfollow_account**: Unfollow an account
- **upload_media**: Returns a media_id to be used when creating a status.

Upload media
- **verify_credentials**: Verify authenticated user credentials


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pixelfed (Instagram Alternative)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the latest posts from my home timeline on Pixelfed."

**🤖 AI Agent:**
> I've retrieved your home timeline. There are new photos from 'nature_lover' and 'tech_daily'. Would you like to see the details of the most recent post?

---

**👤 You:**
> "Post a new status saying 'Exploring the Fediverse with MCP!' with public visibility."

**🤖 AI Agent:**
> Status created successfully! Your post is now live on your Pixelfed profile with public visibility.

---

**👤 You:**
> "Check my recent notifications and tell me if I have any new followers."

**🤖 AI Agent:**
> You have 3 new notifications. 'art_fan' just followed you, and 'photo_pro' liked your latest post. Would you like to follow 'art_fan' back?


## ❓ FAQ

**Q: Can I upload images and post them to my feed using the AI?**
Yes! First, use the `upload_media` tool to upload your file and get a media ID. Then, use the `create_status` tool and include that ID in the `media_ids` array to publish your post.

**Q: How do I see what's trending on my Pixelfed instance?**
You can use the `get_tag_timeline` tool with a specific hashtag to see related posts, or use `get_public_timeline` to see the most recent public posts across the instance.

**Q: Is it possible to manage my followers through this integration?**
Absolutely. You can use `get_followers` and `get_following` to list accounts, and use `follow_account` or `unfollow_account` to manage your connections.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pixelfed-instagram-alternative](https://vinkius.com/mcp/pixelfed-instagram-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pixelfed (Instagram Alternative)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pixelfed-instagram-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pixelfed (Instagram Alternative)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pixelfed-instagram-alternative": {
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
