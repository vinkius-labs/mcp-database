# Descript MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/descript)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/descript-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/descript-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Equip your AI agent with direct access to Descript — manage projects, export transcripts, and retrieve media assets without opening the video editor.

## Description
Connect **Descript** to your AI agent and manage your video and podcast production pipeline conversationally.

### What you can do

- **Project Management** — List, search, and retrieve project details including compositions, transcripts, and media files.
- **Transcript Access** — Pull full transcriptions from any Descript project for repurposing into blog posts, social content, or subtitles.
- **Media Exports** — Retrieve exported audio and video files, download links, and export statuses.
- **Drive Organization** — Navigate your Descript drives and projects to find specific recordings or compositions.

### How it works

1. Subscribe to the Descript integration on the marketplace.
2. Generate an API token from your Descript account (Settings → API tokens → Create token).
3. Ask your AI agent to list projects, pull transcripts, or check export statuses.

### Who is this for?

- **Content Creators** — Repurpose video transcripts into blog posts, newsletters, and social media content without manual copying.
- **Podcast Producers** — Pull episode transcripts and metadata for show notes generation and SEO optimization.
- **Marketing Teams** — Access video project data and transcripts to fuel multi-channel content strategies from a single interface.


## Available Tools
- **list_projects**: List all Descript projects
- **get_project**: Get project details
- **list_drives**: List team drives
- **create_transcription**: Supports audio and video files.

Transcribe a media file
- **get_transcription**: Get transcription result
- **create_export**: Export a project
- **list_exports**: List project exports
- **list_templates**: List available templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Descript** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Descript projects."

**🤖 AI Agent:**
> I found 8 projects in your Descript drive: 'Q1 Product Demo' (last edited 2h ago), 'Podcast Ep 47' (last edited yesterday), 'Customer Interview - Acme', and 5 more.

---

**👤 You:**
> "Get the full transcript of 'Podcast Ep 47'."

**🤖 AI Agent:**
> Here's the transcript for 'Podcast Ep 47' (duration: 42:15). Speakers detected: Host (Sarah) and Guest (Mark). Full text with timestamps extracted. Would you like me to convert this into show notes or a blog post?

---

**👤 You:**
> "Check if my latest video export is ready for download."

**🤖 AI Agent:**
> Your export of 'Q1 Product Demo' is complete. Format: MP4 (1080p). File size: 245 MB. Download link is ready and valid for 24 hours.


## Installation & Usage

To install and use the **Descript** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/descript](https://vinkius.com/mcp/descript)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
