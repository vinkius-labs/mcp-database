# Kapwing MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kapwing)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kapwing-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kapwing-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate video and image rendering via Kapwing — create media from JSON, track render progress, and manage assets directly from any AI agent.

## Description
Connect your **Kapwing** account to any AI agent to automate your video production and media rendering workflows through natural conversation.

### What you can do

- **Automated Rendering** — Initiate complex video or image renders using project JSON definitions including layers, text, and dimensions
- **Status Tracking** — Monitor the real-time progress of your renders and retrieve download URLs once processing is complete
- **Asset Management** — List and browse all renders associated with your account to keep track of your media history
- **Webhook Integration** — Optionally receive notifications at a specific URL when your media is ready

### How it works

1. Subscribe to this server
2. Enter your Kapwing API Key
3. Start generating and managing media from Claude, Cursor, or any MCP-compatible client

No more manual editing for repetitive tasks. Your AI acts as a video engineer, handling the rendering pipeline for you.

### Who is this for?

- **Content Creators** — automate the generation of repetitive video formats or social media assets
- **Developers** — integrate video rendering capabilities into your apps without leaving your coding environment
- **Marketing Teams** — scale content production by generating localized or personalized videos from templates


## Available Tools
- **create_render**: The project definition includes width, height, and layers (video, text, etc.).

Initiates the rendering process for a project
- **get_render_status**: ) and download URL for a specific render ID.

Retrieves the current status of a render
- **list_renders**: Returns a list of all renders associated with your account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kapwing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my recent Kapwing renders."

**🤖 AI Agent:**
> I've retrieved your render history. You have 3 recent renders: 'render_abc123' (Completed), 'render_def456' (Processing), and 'render_ghi789' (Completed). Would you like the download link for any of these?

---

**👤 You:**
> "Check the status of render ID 'render_550e8400'."

**🤖 AI Agent:**
> The render 'render_550e8400' is currently completed. You can download the final file here: [URL].

---

**👤 You:**
> "Create a new 1080x1920 render with a text layer saying 'New Collection' and a video background."

**🤖 AI Agent:**
> I've initiated the render with your specifications. The new Render ID is 'render_998877'. I'll monitor it for you, or you can check back in a few minutes.


## Installation & Usage

To install and use the **Kapwing** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kapwing](https://vinkius.com/mcp/kapwing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
