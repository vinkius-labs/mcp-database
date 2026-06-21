# Tencent Cloud VOD / 腾讯云点播 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tencent-cloud-vod)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tencent-cloud-vod-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tencent-cloud-vod-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Tencent's dominant video-on-demand platform — manage media, track tasks, and audit storage via AI.

## Description
Empower your AI agent to orchestrate your video-on-demand infrastructure and digital asset management with **Tencent Cloud VOD** (云点播), the dominant video processing platform in China. By connecting Tencent VOD to your agent, you transform complex media management, background task tracking, and storage auditing into a natural conversation. Your agent can instantly retrieve detailed video metadata, update media titles and descriptions, search through massive media libraries, and monitor processing tasks without you ever needing to navigate the comprehensive Tencent Cloud Console. Whether you are conducting a digital media audit or coordinating a content distribution refresh, your agent acts as a real-time VOD operations assistant, providing accurate results from a single, authorized source.

### What you can do

- **Media Orchestration** — Retrieve metadata for multiple FileIds, update media info, and delete obsolete assets.
- **Content Discovery** — Search for media files using keywords, classes, and tags with advanced sorting.
- **Task Auditing** — Track the real-time status and technical details of asynchronous VOD background tasks.
- **Storage Monitoring** — Access comprehensive storage volume statistics for specific time ranges.
- **Classification Management** — Retrieve and audit the complete media classification tree for your project.

### How it works

1. Subscribe to this server
2. Enter your Tencent Cloud SecretId, SecretKey, and optionally SubAppId
3. Start managing your video infrastructure through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Video Operations Teams** — automate media metadata management and monitor processing health through natural language.
- **Content Managers** — search and audit large-scale media archives directly from your AI-powered workspace.
- **Developers** — integrate professional-grade video-on-demand capabilities into your AI-driven daily routines.
- **Tencent Cloud Power Users** — integrate your existing VOD workflows into your AI-driven daily routines.


## Available Tools
- **delete_media_file**: Remove media from VOD
- **get_media_info**: Get video metadata
- **get_storage_stats**: Get storage usage data
- **get_task_detail**: Track VOD task
- **list_media_classes**: List all media classes
- **list_recent_media**: List recently updated media
- **search_media_files**: Search VOD library
- **update_media_info**: Modify media properties


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tencent Cloud VOD / 腾讯云点播** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for media files containing 'Product Launch' in my VOD library."

**🤖 AI Agent:**
> I've searched your VOD library. I found 3 files matching 'Product Launch', including '2023_Product_Launch_HQ' (FileId: `88210934`). Would you like me to retrieve the full technical metadata for these files?

---

**👤 You:**
> "Check the status of VOD task 'task-1234567890'."

**🤖 AI Agent:**
> The VOD task `task-1234567890` is currently 'FINISH'. It was a Transcode task that completed successfully at 14:30. Should I check if the resulting media files are now indexed in your library?

---

**👤 You:**
> "Show me our VOD storage usage stats for the last 30 days."

**🤖 AI Agent:**
> I've retrieved your storage usage data. Over the last 30 days, your peak storage reached 1.2 TB, with an average daily increase of 5 GB. Your current active SubAppId is set to 'Root Application'. Would you like a daily breakdown of these metrics?


## Installation & Usage

To install and use the **Tencent Cloud VOD / 腾讯云点播** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tencent-cloud-vod](https://vinkius.com/mcp/tencent-cloud-vod)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
