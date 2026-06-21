# Mastodon MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mastodon)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Automate social interactions on the Fediverse — post statuses, manage follows, and track trending content directly from your AI agent.

## Description
Connect your **Mastodon** account to any AI agent and manage your decentralized social presence through natural conversation.

### What you can do

- **Status Management** — Post new toots, reply to threads, and manage visibility settings (public, unlisted, private, direct) using `post_status`.
- **Engagement** — Favorite, bookmark, and reblog content to interact with your community effortlessly.
- **Timeline Discovery** — Access your home timeline, public feeds, or specific tag streams to stay updated on the latest discussions.
- **Account Control** — Follow or unfollow users, manage blocks and mutes, and update your profile metadata directly.
- **Trending Insights** — Query trending tags, links, and statuses to understand what's happening across the instance.

### How it works

1. Subscribe to this server
2. Enter your Mastodon Personal Access Token
3. Start interacting with the Fediverse from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — Schedule or draft posts and engage with followers without leaving your workflow.
- **Social Researchers** — Analyze trending topics and public timelines using AI-driven queries.
- **Community Managers** — Monitor notifications and manage account relationships efficiently.


## Available Tools
- **clear_notifications**: Clear all notifications
- **unfollow_account**: Unfollow a Mastodon account
- **block_account**: Block a Mastodon account
- **bookmark_status**: Bookmark a Mastodon status
- **check_health**: Check server health status
- **create_app**: Create a new Mastodon application
- **delete_status**: Delete a Mastodon status
- **dismiss_notification**: Dismiss a single notification
- **favourite_status**: Favourite a Mastodon status
- **follow_account**: Follow a Mastodon account
- **get_account_statuses**: Get statuses posted by a Mastodon account
- **get_account**: Get a Mastodon account profile
- **get_home_timeline**: View statuses from followed users
- **get_instance_info**: Get general information about the server
- **get_instance_rules**: View server rules
- **get_list_timeline**: View statuses in a specific list
- **get_notifications_v1**: View notifications for the user (v1)
- **get_notifications_v2**: View grouped notifications for the user (v2, Mastodon 4.3+)
- **get_public_timeline**: View public statuses (local or federated)
- **get_status_context**: View thread ancestors and descendants for a status
- **get_status**: View a single Mastodon status
- **get_tag_timeline**: View statuses containing a specific hashtag
- **get_trending_links**: View trending links
- **get_trending_statuses**: View trending statuses
- **get_trending_tags**: View trending hashtags
- **mute_account**: Mute a Mastodon account
- **post_status**: Post a new status (toot) to Mastodon
- **reblog_status**: Boost (reblog) a Mastodon status
- **register_account**: Register a new Mastodon account
- **search**: Search for accounts, statuses, and hashtags
- **update_credentials**: Update Mastodon profile credentials
- **verify_credentials**: Verify Mastodon account credentials


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mastodon** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Post a new status saying 'Hello from my AI agent!' with public visibility."

**🤖 AI Agent:**
> I've posted your status using `post_status`. It is now live on your profile with public visibility.

---

**👤 You:**
> "Show me the top 5 trending tags on this instance."

**🤖 AI Agent:**
> Fetching trends... The top tags currently are #Technology, #Art, #Fediverse, #News, and #Photography.

---

**👤 You:**
> "Verify my account and show my profile details."

**🤖 AI Agent:**
> Credentials verified! Your account is '@user@instance.social', with 150 followers and 200 following. Your bio is currently set to 'AI Enthusiast'.


## ❓ FAQ

**Q: Can I post a status with a content warning (spoiler text)?**
Yes. When using the `post_status` tool, you can provide a `spoiler_text` string which will act as a content warning for your followers.

**Q: How do I verify if my access token is working correctly?**
You can use the `verify_credentials` tool. It will test your current token and return your authenticated profile information if successful.

**Q: Is it possible to see what is currently trending on my instance?**
Absolutely. Use the `get_trending_tags` tool to retrieve the most popular hashtags used on your instance recently.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mastodon](https://vinkius.com/mcp/mastodon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mastodon** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mastodon` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mastodon** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mastodon": {
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
