# ContentGroove MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/contentgroove)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to automatically generate video highlights, splice long-form clips, and manage video projects natively with ContentGroove.

## Description
Integrate **ContentGroove**, an intelligent video processing engine, directly into your conversational workflow. Automate the process of finding the best highlights from massive podcasts. Use conversational text to command your AI to slice, transcribe, and pull highly engaging snippets from long-form videos.

### What you can do

- **Project Management** — Instruct your AI to list tracked video projects to verify rendering status.
- **Automated Video Splicing** — Request the bot to target a large video, locate engaging discussions, and divide them into independent bite-sized clips natively.
- **Metadata Extraction** — Extract logically synced auto-transcribed subtitles alongside newly generated assets directly into your chat workspace.

### How it works

1. Install this integration into your AI platform.
2. Authorize using a dedicated API Key.
3. Chat your rendering constraints to seamlessly slice video content.

### Who is this for?

- **Social Media Managers** — Slice weekly podcasts into multiple independent clips by firing precise text requests.
- **Content Editors** — Instantly review auto-parsed text captions that overlap visual snippets before deploying to marketing pipelines.
- **Event Marketers** — Feed keynote events and command AI tools to extract the most engaging 2-minute segments immediately.


## Available Tools (8)
- **create_media_from_url**: Import a video from a URL to generate AI highlights
- **create_direct_upload**: Generate a signed URL for direct video upload
- **get_clip_details**: Get details of a specific highlight clip
- **get_media_clips**: List all clips for a specific video
- **get_media_details**: Get details of a specific media project
- **get_media_status**: Check processing status of a media
- **list_all_clips**: List all AI-generated clips
- **list_media**: List all media projects in ContentGroove


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ContentGroove** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the 5 most engaging viral slices from project 'vid9x3a' for a social media campaign."

**🤖 AI Agent:**
> Video slices identified and retrieved. From target 'vid9x3a', I've loaded 5 core highlight moments processed by ContentGroove. Would you prefer reviewing the direct links or looking at the extracted transcript captions?

---

**👤 You:**
> "Check the status of my latest video project render queue."

**🤖 AI Agent:**
> I checked ContentGroove. Your latest project titled 'Webinar Highlights 2024' is currently rendering slice elements at 82%. Should I notify you once it finishes completely?

---

**👤 You:**
> "List all recent AI-generated clips across my account."

**🤖 AI Agent:**
> I've fetched your clips. Here are the 5 most recent highlights from across your projects, including 'Interview with CEO' and 'Product Launch Keynote'. Which one would you like to inspect?


## ❓ FAQ

**Q: How do I generate an API Key inside ContentGroove?**
Log into your active ContentGroove dashboard. Navigate to the **Settings** menu. From there, locate the section labeled **API Keys** and click 'Generate'. Securely copy the resulting string to connect your AI.

**Q: Does AI video processing incur additional costs on ContentGroove?**
Every operation routed through the AI integration relies on your base ContentGroove tier limits. AI-invoked splicing acts as standard manual generation costs; ensure constraints are observed so you stay within your processing credits limit.

**Q: Can I publish video clips straight from the integration?**
No, this integration strictly isolates the video editing capabilities and project listing utilities. To post on major platforms directly from chat, ensure you link subsequent social network MCP integrations into your workflow.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contentgroove](https://vinkius.com/mcp/contentgroove)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ContentGroove** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `contentgroove` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ContentGroove** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "contentgroove": {
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
