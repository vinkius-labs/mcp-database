# D-ID MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/d-id)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/d-id-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/d-id-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Create AI videos via D-ID — generate talking avatars from text or audio, list stock presenters, and monitor credit balance directly from any AI agent.

## Description
Connect your **D-ID** account to any AI agent and take full control of your AI video generation and digital human workflows through natural conversation.

### What you can do

- **Talking Avatar Generation** — Create high-quality videos where an AI avatar speaks your text with precise lip-sync and natural expressions using Microsoft or Amazon TTS
- **Audio-to-Video Sync** — Provision talking avatars from pre-recorded audio files, allowing the agent to generate videos that match your literal audio boundaries
- **Digital Presenters** — List and retrieve available D-ID stock presenters including pre-built digital humans and background options for fast video production
- **Media Uploads** — Upload face images to D-ID servers to use them as custom avatar sources for your personalized video content
- **Run Monitoring** — Track the status of your talks and clips (created, started, done, error) and retrieve final result URLs when processing is complete
- **Credit Auditing** — Get your current D-ID credit balance and plan info to verify remaining limits and manage video generation quotas

### How it works

1. Subscribe to this server
2. Enter your D-ID API Key (found in D-ID Studio > Account Settings)
3. Start generating AI videos from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — generate personalized video messages and social media content without manual editing
- **Marketers** — create localized talking head videos for different markets using various TTS providers and voices
- **Product Teams** — quickly prototype digital human interactions and verify video outputs through natural language
- **Developers** — test and debug D-ID video generation pipelines and presenter mappings directly from the chat


## Available Tools
- **create_talk**: Create a talking avatar video using D-ID. An AI avatar speaks your text with lip-sync and natural expressions
- **create_talk_audio**: Create a D-ID talking avatar from a pre-recorded audio file. Avatar lip-syncs to your audio
- **get_talk**: Wait for creation to finish.

Get status of a D-ID talk. Returns status (created/started/done/error), result_url when done
- **list_talks**: List all D-ID talks. Returns talk IDs, statuses, and creation timestamps
- **delete_talk**: Delete a D-ID talk
- **create_clip**: Create a D-ID clip using a stock presenter (no image needed). Pre-built digital humans with backgrounds
- **get_clip**: Get status of a D-ID clip. Returns status and result URL
- **list_presenters**: List available D-ID presenters. Returns presenter IDs, names, and preview images
- **upload_image**: Upload a face image to D-ID for use as avatar source. Returns image URL
- **get_credits**: Get current D-ID credit balance and plan info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **D-ID** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a talking avatar video with script: 'Welcome to our new platform!'"

**🤖 AI Agent:**
> Talk generation started! I've used a default presenter and voice to process your script. Talk ID: 'tlk_abc123'. I will monitor the status and let you know when the result URL is ready.

---

**👤 You:**
> "List all available D-ID presenters"

**🤖 AI Agent:**
> I found 15 presenters. Available stock humans include 'Amy' (ID: presenter_1), 'Brian' (ID: presenter_2), and 'Claire' (ID: presenter_3). You can use these IDs to create clips instantly.

---

**👤 You:**
> "How many credits do I have left in D-ID?"

**🤖 AI Agent:**
> You currently have 45 credits remaining on your 'Pro' plan. Based on your settings, this is enough to generate approximately 15 minutes of new AI video content.


## Installation & Usage

To install and use the **D-ID** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/d-id](https://vinkius.com/mcp/d-id)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
