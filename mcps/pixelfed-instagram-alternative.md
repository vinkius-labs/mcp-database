# Pixelfed (Instagram Alternative) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pixelfed-instagram-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pixelfed-instagram-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pixelfed-instagram-alternative-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Pixelfed (Instagram Alternative)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pixelfed-instagram-alternative](https://vinkius.com/mcp/pixelfed-instagram-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
