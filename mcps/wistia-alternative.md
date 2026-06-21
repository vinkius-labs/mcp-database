# Wistia MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wistia-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wistia-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wistia-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage videos, projects, and performance analytics on Wistia with AI agents.

## Description
Connect your **Wistia** video marketing account to any AI agent to automate your media library management and performance monitoring through natural conversation. Wistia provides a premier platform for B2B video hosting, delivery, and detailed engagement tracking.

### What you can do

- **Media Orchestration** — List and retrieve detailed metadata for your videos (medias), including titles, descriptions, and statuses.
- **Project Management** — Organize your content by creating and managing hierarchical projects (folders) directly from the AI interface.
- **Engagement Analytics** — Retrieve real-time performance stats for specific videos or get an aggregated overview of your account-wide metrics.
- **Metadata Control** — Programmatically update video details and manage captions to ensure your media library is always optimized.
- **Asset Delivery** — Fetch player configurations and thumbnail URLs to streamline content distribution across your digital channels.

### How it works

1. Subscribe to this server
2. Enter your Wistia API Token from your account settings
3. Start managing your video assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Teams** — automate the monitoring of video engagement and organize media assets via natural language.
- **Video Producers** — quickly update video titles and retrieve media links without leaving the project workspace.
- **Business Analysts** — get instant account-wide video performance reports and visitor metrics straight through the chat.


## Available Tools
- **create_project**: Create a new project
- **get_account_analytics**: Get account-wide stats
- **get_video_details**: Get metadata for a video
- **get_project_details**: Get metadata for a project
- **get_video_stats**: Get video analytics
- **list_video_captions**: List captions for a video
- **list_videos**: List all videos (medias)
- **list_projects**: List your Wistia projects
- **update_video_details**: Modify video metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wistia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in my Wistia account."

**🤖 AI Agent:**
> I've retrieved your projects. You have 4 active folders: 'Product Demos', 'Customer Testimonials', 'Internal Training', and '2024 Ad Campaign'. Which one should we check?

---

**👤 You:**
> "Show the engagement stats for video ID 'vid123'."

**🤖 AI Agent:**
> Fetching analytics... Video 'vid123' has 1,250 total plays, with an average engagement of 68% and 420 unique visitors. Would you like a more detailed breakdown?


## Installation & Usage

To install and use the **Wistia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wistia-alternative](https://vinkius.com/mcp/wistia-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
