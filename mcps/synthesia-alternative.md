# Synthesia MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/synthesia-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/synthesia-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/synthesia-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Produce professional AI videos with lifelike avatars that present in 140+ languages without cameras, studios, or actors.

## Description
Connect your **Synthesia** AI video account to any AI agent and simplify how you create professional avatar-led videos, manage video templates, and monitor production status through natural conversation.

### What you can do

- **AI Video Generation** — Create high-quality videos by providing a script and selecting an avatar programmatically via AI.
- **Template Automation** — Generate videos by filling dynamic variables in pre-defined Synthesia Studio templates.
- **Avatar Directory** — List available stock avatars and retrieve detailed metadata to choose the right persona for your content.
- **Production Monitoring** — Check real-time processing status and retrieve final video links directly from the agent.
- **History Oversight** — List and query all previously generated videos and manage your production library.
- **Workflow Webhooks** — Manage notification endpoints to receive real-time updates when your videos are finished.

### How it works

1. Subscribe to this server
2. Enter your Synthesia API Key (found in your account settings under API)
3. Start generating professional AI videos from Claude, Cursor, or any MCP client

### Who is this for?

- **Content Creators & Marketers** — quickly generate personalized videos for social media or internal training via simple AI commands.
- **Learning & Development Teams** — automate the creation of instructional videos using pre-defined templates.
- **Ops & Product Teams** — monitor production status and manage video assets directly from the workspace via the AI assistant.


## Available Tools
- **create_video_from_template**: Generate video using a Synthesia template
- **create_video**: Create a new AI avatar video
- **create_webhook**: completed or video.failed.

Create a new notification webhook
- **delete_video**: Permanently delete a video
- **delete_webhook**: Remove an existing webhook
- **get_video_details**: Get details and status for a video
- **list_avatars**: List available AI avatars
- **list_templates**: List your video templates
- **list_videos**: List your generated videos
- **list_webhooks**: List configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Synthesia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all videos generated in my Synthesia account."

**🤖 AI Agent:**
> I've retrieved your video history. You have 5 videos including 'Onboarding Welcome', 'Quarterly Update', and 'Sales Pitch v2'. Which one would you like to see the status or download link for?

---

**👤 You:**
> "Generate a video from template 'temp_88231' with script: 'Welcome to the team, Sarah!'."

**🤖 AI Agent:**
> Video generation triggered! I've started creating a new video using template temp_88231 and your custom script. The video ID is vid_10293. I'll let you know when the production is complete.

---

**👤 You:**
> "Show me the available stock avatars for marketing videos."

**🤖 AI Agent:**
> Fetching avatars... You have access to dozens of personas including 'Anna' (Business Professional), 'Marcus' (Casual), and 'Helena' (Tech Guide). Would you like to see the full metadata for any of them?


## Installation & Usage

To install and use the **Synthesia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/synthesia-alternative](https://vinkius.com/mcp/synthesia-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
