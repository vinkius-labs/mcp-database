# Tavus Video Replicas MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tavus-video-replicas)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tavus-video-replicas-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tavus-video-replicas-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Generate personalized AI videos via Tavus — manage replicas, create videos from scripts, and track generation status.

## Description
Connect your AI agent to **Tavus**, the leading platform for automated personalized video generation. This integration allows you to leverage AI replicas to create high-quality, talking-head videos for sales, marketing, and customer success directly from your conversation.

### What you can do

- **Replica Management** — List and inspect your trained AI video replicas
- **Video Generation** — Create new videos by providing a script and selecting a replica
- **Status Tracking** — Monitor the progress of video generation tasks in real-time
- **Content Library** — Access a list of all your generated videos and their download links
- **Resource Cleanup** — Permanently delete replicas or videos no longer needed

### How it works

1. Subscribe to this server
2. Enter your **Tavus API Key** (v2)
3. Start generating personalized video content through natural language

### Who is this for?

- **Marketing Teams** — automate the creation of personalized video campaigns at scale
- **Sales Professionals** — generate custom outreach videos for prospects using AI clones
- **Customer Success** — create personalized onboarding and support videos for clients


## Available Tools
- **delete_replica**: Permanently delete a specific replica
- **delete_video**: Permanently delete a specific generated video
- **generate_replica_video**: Generate a new AI video using a specific replica
- **get_replica_details**: Get comprehensive details for a specific replica
- **get_video_details**: Get detailed information for a specific generated video
- **list_replicas**: Retrieve a list of all your AI video replicas
- **list_generated_videos**: Retrieve a list of all generated videos


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tavus Video Replicas** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my Tavus replicas."

**🤖 AI Agent:**
> Fetching replicas... I found 2 replicas: 'Sales Persona' (ID: rep_123) and 'Founder Clone' (ID: rep_456). Both are ready for use.

---

**👤 You:**
> "Generate a video with replica 'rep_123' saying 'Hello, welcome to our platform!'."

**🤖 AI Agent:**
> Generation task started! Video ID is 'vid_789'. You can check the status in a few minutes to get the download link.


## Installation & Usage

To install and use the **Tavus Video Replicas** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tavus-video-replicas](https://vinkius.com/mcp/tavus-video-replicas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
