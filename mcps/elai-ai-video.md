# Elai AI Video MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/elai-ai-video)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to generate AI videos, manage avatars, and track rendering status via the Elai.io API.

## Description
Integrate **Elai.io**, the leading AI video generation platform, directly into your AI workflow. Manage your video projects and rendering statuses, track available AI avatars and voices, monitor templates and languages, and oversee your video production using natural language.

### What you can do

- **Video Oversight** — List and retrieve detailed information and status for all your AI video projects and renders.
- **Avatar Intelligence** — Access the avatar registry to monitor available AI presenters, their unique identifiers, and preview thumbnails.
- **Content Management** — Monitor video templates, supported languages, and high-quality AI voices for automated narration.
- **Production Auditing** — Retrieve high-level summaries of rendering progress, remaining account minutes, and organizational metadata instantly.

### How it works

1. Connect the Elai.io integration to your AI assistant.
2. Authorize using your Elai.io API Key (found in your account settings).
3. Orchestrate your AI video production and avatar-led content through intuitive conversation.

### Who is this for?

- **Content Creators** — Quickly check video rendering status and avatar availability on the go.
- **Marketing Teams** — Monitor video production volumes and template usage via chat.
- **Operations Leads** — Research specific project details and organizational video metadata instantly.


## Available Tools (10)
- **create_new_ai_video**: Create a new AI video from a template or text script
- **get_elai_account_metadata**: Retrieve metadata and credit balance for your Elai account
- **get_video_details**: Get detailed settings and rendering status for a specific video
- **list_available_avatars**: List all AI avatars available for video generation
- **list_successfully_rendered_videos**: Identify videos that have finished rendering and are ready for download
- **list_latest_video_projects**: Identify the most recently created or updated video projects
- **list_video_templates**: List all video templates available in your account
- **list_ai_videos**: List all AI videos created in your Elai account
- **list_available_voices**: List all AI voices and languages supported for video narration
- **trigger_video_rendering**: Start the rendering process for a specific video project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Elai AI Video** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my AI video projects."

**🤖 AI Agent:**
> I've found 5 video projects, including 'Q3 Product Announcement' and 'Onboarding Tutorial'. 3 projects are 'Ready' and 2 are 'Rendering'. Would you like the link for the Product Announcement?

---

**👤 You:**
> "Show me the available AI avatars."

**🤖 AI Agent:**
> I've retrieved several available avatars, including 'James' (Business Professional), 'Elena' (Casual Tech), and 'Marcus' (Medical). Each has unique clothing options. Should I pull the thumbnail preview for James?

---

**👤 You:**
> "Check the status of video 'VID-12345'."

**🤖 AI Agent:**
> Video 'VID-12345' (Title: Team Intro) is currently 'Rendering'. It is at 65% completion and is expected to be ready in approximately 5 minutes. Should I notify you once it finishes?


## ❓ FAQ

**Q: How do I get an Elai.io API Key?**
Log in to your Elai.io account, navigate to **Account Settings** → **API**, and you can generate or retrieve your unique API Key from there. API access may require a specific plan.

**Q: Can the agent render videos automatically?**
Yes, you can use the trigger_video_rendering tool to start the rendering process for any existing video project directly via the agent.

**Q: Does the integration show final video URLs?**
Yes, once a video has finished rendering (status: ready), the agent can retrieve the final output URL through the get_video_details tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/elai-ai-video](https://vinkius.com/mcp/elai-ai-video)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Elai AI Video** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `elai-ai-video` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Elai AI Video** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "elai-ai-video": {
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
