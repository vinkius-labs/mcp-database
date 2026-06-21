# Pixelfed (Instagram Alternative) MCP Server

Manage your Pixelfed presence — post photos, interact with the community, and track notifications directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pixelfed-instagram-alternative)

## Overview
**Category:** communication-messaging
**Tools Count:** 17

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


## Installation & Usage

To install and use the **Pixelfed (Instagram Alternative)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pixelfed-instagram-alternative](https://vinkius.com/mcp/pixelfed-instagram-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
