# Shotstack MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shotstack)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/shotstack-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/shotstack-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Render and edit videos programmatically with a cloud API that generates personalized video content at scale from templates.

## Description
Connect your **Shotstack** account to any AI agent and take full control of your high-volume video editing and media orchestration through natural conversation. Shotstack provides a powerful API-first platform for rendering videos, managing cloud templates, and ingesting assets directly from your chat interface.

### What you can do

- **Video Rendering Orchestration** — Trigger professional video renders from JSON-based templates or custom edits programmatically.
- **Template Lifecycle Management** — Create and monitor cloud-based video templates to ensure consistent automated outputs directly from the AI interface.
- **Asset & Ingest Control** — Ingest source media and manage your hosted assets to maintain a clear overview of your production resources.
- **Render Intelligence** — Retrieve real-time render statuses and detailed metadata to track the progress of your video pipeline via natural language.
- **Operational Monitoring** — List available renders, templates, and source assets using simple AI commands to ensure your production is optimized.

### How it works

1. Subscribe to this server
2. Enter your Shotstack API Key from your dashboard (Stage or Production)
3. Start generating cloud videos from Claude, Cursor, or any MCP-compatible client

No more manual status checking or template hunting. Your AI acts as a dedicated video producer or media coordinator.

### Who is this for?

- **Video Developers** — quickly test render configurations and monitor template performance without writing complex scripts.
- **Content Marketers** — automate the generation of personalized video content and monitor render progress via natural conversation.
- **Operations Teams** — streamline the management of cloud assets and monitor production usage directly within the chat.


## Available Tools
- **create_video_template**: Save an edit as a reusable template
- **get_hosted_asset_details**: Get details for a hosted file
- **get_render_status**: Check the status of a render job
- **ingest_media_source**: Upload or fetch a source asset
- **list_assets_from_render**: ) associated with a specific job ID.

Find all files created by a specific render
- **list_hosted_assets**: List all hosted media files
- **list_recent_renders**: List recent render history
- **list_ingested_sources**: List all ingested media sources
- **list_templates**: List available video templates
- **render_video**: Returns a render ID.

Start a new video render job


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shotstack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the status of my latest video render in Shotstack."

**🤖 AI Agent:**
> I've retrieved the render status. Your video 'PROMO_V1' (ID: abc-123) is currently 75% complete. I'll let you know once the final asset URL is available.

---

**👤 You:**
> "List all video templates in my Shotstack account."

**🤖 AI Agent:**
> Retrieving templates... I found 5 cloud templates including 'Social_Post_Template', 'Intro_Video', and 'Outro_Video'. Would you like to use any of them for a new render?

---

**👤 You:**
> "List all hosted assets in my Shotstack Serve account."

**🤖 AI Agent:**
> Fetching assets... You have 12 hosted assets including 'Logo_Animation.mp4' and 'Background_Music.mp3'. Would you like to get the public URL for any of them?


## Installation & Usage

To install and use the **Shotstack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shotstack](https://vinkius.com/mcp/shotstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
