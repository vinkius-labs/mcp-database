# Vadoo AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vadoo-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate videos, captions, and podcasts automatically using AI.

## Description
Connect your AI agent to **Vadoo AI** to natively generate multimedia content, clip long videos, and synthesize podcasts directly via text prompts.

### What you can do

- **Video Generation** — Create high-quality videos just by typing a descriptive prompt and selecting a voice.
- **Clips & Captions** — Provide a long video URL and let the AI automatically extract engaging short clips or generate precise subtitles.
- **Podcast Creation** — Synthesize entire podcast episodes based on a specific topic or script without recording any audio.
- **Task Tracking** — Query the generation status of your multimedia tasks in real-time.

### How it works

1. Retrieve your API Key from the Vadoo AI dashboard.
2. Provide the key to this integration.
3. Instruct your AI agent to generate a video about 'Space Exploration' or create clips from a YouTube link.

### Who is this for?

- **Content Creators** — Scale your social media output by generating clips and captions on the fly.
- **Marketers** — Create promotional videos and podcasts dynamically.
- **Developers** — Hook multimedia generation endpoints directly into your pipelines.


## Available Tools
- **vadooai_check_generation_status**: Check video generation status
- **vadooai_check_video_status**: Get details of a completed video
- **vadooai_create_clips**: Create short clips from video
- **vadooai_generate_caption**: Generate video captions
- **vadooai_generate_podcast**: Generate AI podcast
- **vadooai_generate_video**: Generate AI video from prompt


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vadoo AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a video about the history of artificial intelligence."

**🤖 AI Agent:**
> Here is the information you requested based on the execution of the tools.

---

**👤 You:**
> "Create short clips from this YouTube video URL: https://youtu.be/example"

**🤖 AI Agent:**
> Here is the information you requested based on the execution of the tools.

---

**👤 You:**
> "Check the status of my video generation task ID 88992."

**🤖 AI Agent:**
> Here is the information you requested based on the execution of the tools.


## ❓ FAQ

**Q: Can I generate an entire podcast just from a topic string?**
Yes. By invoking the 'vadooai_generate_podcast' tool and supplying a simple topic, the API synthesizes the audio and returns a task ID to track it.

**Q: How do I download the generated video?**
Use the 'vadooai_check_video_status' tool with your Task/Video ID. Once generation is complete, the API will return the direct download URL.

**Q: Is it possible to extract short clips from a YouTube URL?**
Yes. Provide the video URL to the 'vadooai_create_clips' tool, and Vadoo AI will automatically parse the video and generate short-form clips.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vadoo-ai](https://vinkius.com/mcp/vadoo-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vadoo AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `vadoo-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vadoo AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vadoo-ai": {
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
