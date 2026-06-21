# Mastodon MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mastodon)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mastodon-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mastodon-mcp)
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


## Installation & Usage

To install and use the **Mastodon** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mastodon](https://vinkius.com/mcp/mastodon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
