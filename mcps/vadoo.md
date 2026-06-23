# Vadoo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vadoo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Host and optimize video content for the web with AI-powered SEO, automatic subtitles, and engagement analytics for creators.

## Description
Connect your **Vadoo AI** account to any AI agent and simplify how you generate, edit, and optimize your video content through natural conversation.

### What you can do

- **AI Video Generation** — Create high-quality videos from simple text prompts or scripts instantly.
- **Viral Clip Creation** — Extract short, social-media-ready clips from long-form video URLs (like YouTube).
- **Automated Captioning** — Generate and overlay captions onto your videos to increase engagement and accessibility.
- **AI Podcasts** — Trigger the creation of conversational 2-person podcasts from any topic or text source.
- **Content Library** — List all your generated videos and retrieve direct download links and metadata.

### How it works

1. Subscribe to this server
2. Enter your Vadoo AI API Key (found in your account dashboard)
3. Start generating and editing your video content from Claude, Cursor, or any MCP client

### Who is this for?

- **Content Creators & YouTubers** — quickly generate viral shorts and captions via simple AI commands.
- **Marketing Teams** — automate the creation of promotional videos and social media assets.
- **Podcasters** — transform text-based topics into interactive AI-generated conversational audio.


## Available Tools (6)
- **add_captions**: Add captions to a video
- **create_clips**: Generate viral clips from a video
- **generate_podcast**: Generate an AI podcast
- **generate_video**: Generate a new AI video
- **get_video_details**: Get details for a specific video
- **list_videos**: List your Vadoo AI videos


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vadoo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the AI videos I've generated so far."

**🤖 AI Agent:**
> I've retrieved your video library. You have 8 generated videos, including 'Marketing Intro', 'Product Demo v1', and 'AI News Weekly'. Which one would you like to get the download link for?

---

**👤 You:**
> "Create viral clips from this YouTube video: https://youtube.com/watch?v=123."

**🤖 AI Agent:**
> Processing video... I've initiated the clip creation for the provided URL. Vadoo AI is now identifying viral moments. I'll let you know once the clips are ready for review.

---

**👤 You:**
> "Generate a vertical AI video about 'The future of remote work'."

**🤖 AI Agent:**
> AI video generation started! I've triggered a new creation with a 9:16 aspect ratio. The project ID is vid_10293. The AI is now assembling the visuals and script.


## ❓ FAQ

**Q: Can I generate a video in a specific aspect ratio?**
Yes! When using the `generate_video` tool, you can specify the `ratio` parameter (e.g., '9:16' for vertical shorts or '16:9' for horizontal videos).

**Q: How do I turn a long YouTube video into viral clips?**
Use the `create_clips` action and provide the YouTube URL. Vadoo AI will analyze the content and automatically extract high-potential segments for social media.

**Q: Is it possible to add captions to an existing video ID?**
Absolutely. Use the `add_captions` tool and provide the Video ID. The AI will generate and overlay the subtitles onto that specific video in your library.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vadoo](https://vinkius.com/mcp/vadoo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vadoo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vadoo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vadoo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vadoo": {
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
