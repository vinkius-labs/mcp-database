# HeyGen MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/heygen-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Create AI-generated videos with realistic digital avatars that speak in any language for training, marketing, and communication.

## Description
Connect your **HeyGen** account to any AI agent and take full control of your AI video production and avatar workflows through natural conversation.

### What you can do

- **Avatar Video Generation** — Create high-quality videos by selecting from a diverse range of AI avatars and professional voices
- **One-Shot Production** — Use the AI Video Agent to generate complete videos from a single text prompt automatically
- **Template Automation** — Generate personalized videos at scale by replacing variables in your predefined HeyGen templates
- **Asset Management** — Upload media assets (images, audio, video) and manage your creation library programmatically
- **Status Monitoring** — Track the progress of video generation jobs and retrieve instant download links upon completion

### How it works

1. Subscribe to this server
2. Retrieve your API Key from your HeyGen Dashboard (Settings > API)
3. Start generating and managing AI videos from Claude, Cursor, or any MCP client

No more manual editing or complex timeline management for simple avatar videos. Your AI acts as your dedicated video producer.

### Who is this for?

- **Content Marketers** — scale video content production for social media and ads using automated avatar generation
- **Sales Teams** — create personalized video outreach at scale by automating template-based video creation
- **Educational Designers** — convert text lessons into engaging avatar-led videos without filming or recording


## Available Tools (12)
- **list_available_avatars**: List AI actors
- **list_video_templates**: List design templates
- **list_generated_videos**: List past creations
- **list_available_voices**: List AI voices
- **test_heygen_auth**: Verify credentials
- **upload_media_asset**: Add image/audio source
- **generate_from_prompt**: One-shot prompt to video
- **remove_video_record**: Delete video
- **create_from_template**: Use template for video
- **generate_ai_video**: Create avatar video
- **get_api_status**: Check connection
- **get_video_progress**: Check video status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HeyGen** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a video from prompt: 'A professional man introducing our new AI cloud services'."

**🤖 AI Agent:**
> Triggering Video Agent... I've started a new generation job with your prompt. The task ID is 'v123456789'. I'll monitor it for you and provide the download link as soon as it's ready.

---

**👤 You:**
> "Show me a list of all available English voices in HeyGen."

**🤖 AI Agent:**
> Fetching English voices... I found 15 high-quality options. Popular choices include 'Aria' (Female, Professional) and 'Davis' (Male, Narrative). Which one would you like to use for your next video?

---

**👤 You:**
> "Check the status of video job 'v123456789'."

**🤖 AI Agent:**
> Checking status... Video 'v123456789' is now 100% complete! You can download it here: [download_url]. The video features a professional avatar with high-fidelity synthesis.


## ❓ FAQ

**Q: How do I choose the right avatar for my video?**
Use the `list_available_avatars` tool to browse all options. Your agent will provide the names and unique `avatar_id` for each character, which you can then use in your generation requests.

**Q: Can I generate a video without specifying an avatar or voice?**
Yes! Use the `generate_from_prompt` tool (Video Agent). Simply describe what you want, and HeyGen will automatically select the best-matching avatar and voice for your content.

**Q: Is it possible to automate personalized videos for multiple customers?**
Absolutely. Use the `create_from_template` tool by providing a `templateId` and a set of variables. Your AI agent can iterate through your customer list and trigger unique videos for each person.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heygen-alternative](https://vinkius.com/mcp/heygen-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HeyGen** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `heygen-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HeyGen** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heygen-alternative": {
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
