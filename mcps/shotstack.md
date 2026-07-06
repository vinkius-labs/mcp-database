# Shotstack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shotstack)
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


## Available Tools (10)
- **list_ingested_sources**: List all ingested media sources
- **list_templates**: List available video templates
- **render_video**: Returns a render ID.

Start a new video render job
- **create_video_template**: Save an edit as a reusable template
- **get_hosted_asset_details**: Get details for a hosted file
- **get_render_status**: Check the status of a render job
- **ingest_media_source**: Upload or fetch a source asset
- **list_assets_from_render**: ) associated with a specific job ID.

Find all files created by a specific render
- **list_hosted_assets**: List all hosted media files
- **list_recent_renders**: List recent render history


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


## ❓ FAQ

**Q: Can my AI automatically check the progress of a video render just by providing its ID?**
Yes! Use the `get_render_status` tool with the Render ID. Your agent will respond with the current status (e.g., 'rendering', 'done') and the final video URL if completed.

**Q: How do I list all my available cloud video templates?**
Simply ask the agent to run the `list_templates` action. It will retrieve the full catalog of video templates configured in your Shotstack account.

**Q: How do I find my Shotstack API Key?**
Log in to your [**Shotstack dashboard**](https://dashboard.shotstack.io/keys) and navigate to the **API Keys** section. You will find both **Stage** and **Production** keys there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shotstack](https://vinkius.com/mcp/shotstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shotstack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shotstack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shotstack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shotstack": {
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
