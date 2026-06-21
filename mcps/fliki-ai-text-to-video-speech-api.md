# Fliki (AI Text-to-Video & Speech API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fliki-ai-text-to-video-speech-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Create high-quality videos and AI voices from text scripts using Fliki — generate content, list voices, and track rendering status.

## Description
Transform your text into engaging video content with the **Fliki** MCP server. This integration allows your AI agent to orchestrate full video production workflows through natural conversation.

### What you can do

- **Video Generation** — Create new videos from text scripts with customizable voices, aspect ratios (16:9, 9:16, 1:1), and background music.
- **Status Tracking** — Monitor the lifecycle of your video generation tasks, from queued and processing to completed with a public download link.
- **Voice Discovery** — Access a comprehensive list of available AI voices and their supported languages to find the perfect match for your brand.

### How it works

1. Subscribe to this server
2. Enter your Fliki API Key
3. Start generating multimedia content from Claude, Cursor, or any MCP-compatible client

No more manual video editing for simple social media clips or voiceovers. Your AI acts as a creative director and video editor.

### Who is this for?

- **Content Creators** — instantly turn blog posts or scripts into video drafts without leaving the chat interface.
- **Marketing Teams** — automate the creation of promotional clips in different aspect ratios for various social platforms.
- **Developers** — integrate automated video and speech generation into your existing AI-driven workflows.


## Available Tools
- **generate_video**: Provide the script content and optional voice, aspect ratio, and background music.

Generate a video based on a provided script or text
- **get_video**: Get the status and download link for a generated video
- **list_voices**: List available AI voices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fliki (AI Text-to-Video & Speech API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the available AI voices and their languages."

**🤖 AI Agent:**
> I've retrieved the list of voices. You can choose from 'Sara' (English), 'Joao' (Portuguese), 'Elena' (Spanish), and many others. Which language or style are you looking for?

---

**👤 You:**
> "Generate a 9:16 video for TikTok with the script: 'Top 3 productivity tips for developers' using the voice 'Sara'."

**🤖 AI Agent:**
> I've started the video generation for your TikTok script. The task ID is 'flk_v8291'. I will monitor the progress and let you know when the download link is ready.

---

**👤 You:**
> "Check the status and get the download link for video ID 'flk_v8291'."

**🤖 AI Agent:**
> The video generation for 'flk_v8291' is now 'completed'. You can download your video here: [https://fliki.ai/download/v8291].


## ❓ FAQ

**Q: How can I see which AI voices are available for my video?**
Use the `list_voices` tool. It will return a full list of available AI voices along with their supported languages, helping you choose the right one for the `generate_video` action.

**Q: Can I track the progress of a video I just started generating?**
Yes! After starting a generation, use the `get_video` tool with the unique video ID. It will tell you if the video is 'queued', 'processing', or 'completed'.

**Q: How do I specify the video format, like for Instagram Reels or YouTube?**
When using `generate_video`, you can provide the `aspectRatio` parameter. Use '9:16' for Reels/TikTok, '16:9' for YouTube, or '1:1' for square posts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fliki-ai-text-to-video-speech-api](https://vinkius.com/mcp/fliki-ai-text-to-video-speech-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fliki (AI Text-to-Video & Speech API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fliki-ai-text-to-video-speech-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fliki (AI Text-to-Video & Speech API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fliki-ai-text-to-video-speech-api": {
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
