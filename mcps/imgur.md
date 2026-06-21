# Imgur MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/imgur)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/imgur-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/imgur-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Manage Imgur content — upload images, organize albums, and browse the gallery directly from your AI agent.

## Description
Connect your **Imgur** account to any AI agent to automate image hosting, album organization, and gallery interactions through natural language.

### What you can do

- **Image Management** — Upload images via binary data, base64, or URLs, and update titles or descriptions instantly
- **Album Orchestration** — Create, delete, and manage albums, including adding multiple images to specific collections
- **Gallery Exploration** — Search the global Imgur gallery, fetch viral content, and manage your account favorites
- **Account Insights** — Retrieve public profile data, submissions, and private account settings
- **Engagement** — Create, delete, and vote on comments within the Imgur community

### How it works

1. Subscribe to this server
2. Enter your Imgur Client ID (and optional Access Token for private actions)
3. Start managing your media assets from Claude, Cursor, or any MCP client

### Who is this for?

- **Content Creators** — quickly upload and organize assets for social media or blogs
- **Developers** — manage application screenshots and assets directly from the terminal or IDE
- **Social Media Managers** — monitor gallery trends and manage community engagement efficiently


## Available Tools
- **add_images_to_album**: Add images to an existing album
- **create_album**: Create a new album
- **create_comment**: Create a new comment on an item
- **delete_album**: Delete an album with a given ID
- **delete_comment**: Delete a comment
- **delete_image**: Delete an image
- **get_account_gallery_favorites**: Get the user's gallery favorites
- **get_account_settings**: Get the current user's account settings (requires access token)
- **get_account_submissions**: Get images and albums submitted to the gallery by the user
- **get_account**: Get standard user information for an Imgur account
- **get_album**: Get information about a specific album
- **get_comment**: Get information about a specific comment
- **get_gallery**: Get the Imgur gallery
- **get_image**: Get information about a specific image
- **search_gallery**: Search the gallery for images and albums
- **submit_to_gallery**: Submit an image or album to the gallery
- **update_image**: Update the title or description of an image
- **upload_image**: Upload a new image
- **vote_comment**: Vote on a comment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Imgur** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Imgur gallery for 'vintage photography' and show me the results."

**🤖 AI Agent:**
> I've searched the gallery for 'vintage photography'. I found several high-quality matches, including a collection of 1950s street scenes (ID: abc123) and a set of film portraits (ID: def456).

---

**👤 You:**
> "Upload this image URL to Imgur: https://example.com/photo.jpg"

**🤖 AI Agent:**
> The image has been successfully uploaded! You can view it at https://imgur.com/xyz789. The image hash is xyz789.

---

**👤 You:**
> "Get the details and description for image hash xyz789."

**🤖 AI Agent:**
> Fetching details for xyz789... The image is titled 'Sunset over Mountains', has 1,200 views, and is currently set to public visibility.


## Installation & Usage

To install and use the **Imgur** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/imgur](https://vinkius.com/mcp/imgur)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
