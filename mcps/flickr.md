# Flickr MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flickr)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/flickr-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/flickr-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Browse, search, and manage photo collections on Flickr with access to one of the largest creative photography communities online.

## Description
Connect your **Flickr** account to any AI agent and take full control of your public photo discovery and image management workflows through natural conversation.

### What you can do

- **Visual Orchestration** — Search across billions of public photos programmatically using keywords and retrieve detailed technical metadata including dimensions and source URLs
- **Trend Intelligence** — Monitor real-time 'hot' tags and explore photos marked as 'interesting' by Flickr algorithms to keep your content strategies culturally relevant
- **User & Album Navigation** — List public albums (photosets) and retrieve complete photo directories for specific user IDs to maintain a high-fidelity visual context
- **Metadata Retrieval** — Access granular details for specific photos, including titles, descriptions, and capture dates directly through your agent
- **Community Discovery** — Search for public groups and retrieve photos from group pools to identify niche visual communities and content patterns

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the Flickr App Garden (Create an App)
3. Start discovering and managing public visual media from Claude, Cursor, or any MCP client

No more manual scrubbing through photo galleries to find specific references. Your AI acts as your dedicated visual research assistant.

### Who is this for?

- **Content Curators** — instantly find relevant public images for mood boards and research using natural language queries
- **Creative Strategists** — monitor visual trends and trending tags across the Flickr community without leaving your workspace
- **Developers** — integrate high-quality public photo search and album metadata into custom internal tools and dashboards


## Available Tools
- **get_group_photos**: Get photos from a group pool
- **get_hot_tags**: Get a list of currently hot tags
- **get_interesting_photos**: Get interesting photos from Flickr
- **get_photo_info**: Get details of a specific photo
- **get_album_photos**: Get photos in a specific album
- **get_recent_photos**: Get recent public photos
- **get_user_info**: Get information about a Flickr user
- **get_user_albums**: List public albums (photosets) for a user
- **get_user_popular_tags**: Get popular tags for a user
- **get_user_public_photos**: Get public photos of a user
- **search_groups**: Search for Flickr groups
- **search_photos**: Search for public photos on Flickr


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flickr** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for photos of 'Cyberpunk Architecture' on Flickr."

**🤖 AI Agent:**
> Retrieving photos... I've found 5 stunning images of Cyberpunk Architecture. They feature neon-lit cityscapes from Tokyo and Hong Kong. Would you like the direct source links for these photos?

---

**👤 You:**
> "Show me what tags are trending on Flickr right now."

**🤖 AI Agent:**
> Fetching hot tags... Currently, trending tags include 'spring2026', 'astrophotography', and 'street-style'. Would you like to see the most 'interesting' photos associated with any of these?

---

**👤 You:**
> "List the public albums for user '12345678@N00'."

**🤖 AI Agent:**
> Retrieving albums for user 12345678@N00... I've found 3 public photosets: 'Summer Trip 2025', 'Macro Nature', and 'Black & White Portraits'. Which album would you like to explore?


## Installation & Usage

To install and use the **Flickr** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flickr](https://vinkius.com/mcp/flickr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
