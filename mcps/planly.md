# Planly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/planly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Schedule and auto-publish social media posts across Instagram, TikTok, Twitter, and LinkedIn with a clean visual calendar.

## Description
Connect your **Planly** account to any AI agent and take full control of your social media orchestration and content scheduling through natural conversation. Planly is a comprehensive social media management tool, and this integration allows you to retrieve channel metadata, schedule posts in bulk, and manage media libraries directly from your chat interface.

### What you can do

- **Channel & Team Orchestration** — List all connected social channels and retrieve detailed team metadata programmatically to ensure your social presence is always synchronized.
- **Content Scheduling Intelligence** — Create and manage post schedules and groups directly from the AI interface to track engagement timings and multi-channel delivery.
- **Media Library Control** — Start and finish media uploads (images and videos) via natural language to maintain a high-fidelity content repository.
- **AI Assistant Integration** — Utilize Planly's internal AI capabilities to complete content ideas and generate captions using simple AI commands.
- **Operational Monitoring** — Track schedule statuses and manage system metadata to ensure your social media workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Planly API Key (Bearer Token) from your security settings
3. Start managing your social media automation from Claude, Cursor, or any MCP-compatible client

No more manual logging into dashboards to check post status. Your AI acts as a dedicated social media manager or content coordinator.

### Who is this for?

- **Social Media Managers** — quickly retrieve channel summaries and monitor schedule health without switching apps.
- **Marketing Teams** — automate the scheduling of cross-platform campaigns and track media assets via natural conversation.
- **Developers** — integrate real-time social scheduling data and media management directly within the chat.


## Available Tools (11)
- **delete_schedule**: Delete a scheduled post
- **finish_media_upload**: Finalize a media upload
- **get_schedule**: Get details for a specific scheduled post
- **list_analytics**: Get analytics for a social media channel
- **list_channels**: List connected social media channels
- **list_schedules**: List all scheduled posts
- **list_teams**: List all teams
- **start_media_upload**: Initiate a media upload
- **ai_generate_content**: Generate post content using AI
- **create_draft**: Create a post draft
- **create_schedule**: Create a new scheduled post


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Planly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active social channels in Planly."

**🤖 AI Agent:**
> I've retrieved your channels. You have 3 connected profiles: 'Instagram Main', 'Twitter Biz', and 'LinkedIn Page'. Which one would you like to schedule a post for?

---

**👤 You:**
> "Show me all posts scheduled for the next 7 days across all my social media channels."

**🤖 AI Agent:**
> 18 posts scheduled across your 4 connected channels for the next 7 days. Instagram: 6 posts (3 reels, 2 carousels, 1 story). Twitter/X: 5 tweets including 2 threads. LinkedIn: 4 articles and company updates. TikTok: 3 videos. Tomorrow has the highest density with 5 posts between 9 AM and 6 PM. 2 posts are missing captions and need attention before publishing.

---

**👤 You:**
> "Schedule a new Instagram carousel post for Thursday at 10 AM with AI-generated caption."

**🤖 AI Agent:**
> Carousel post scheduled for Thursday, May 22nd at 10:00 AM on Instagram (@yourbrand). 4 images uploaded and ordered. AI-generated caption: "Transform your workspace into a productivity powerhouse. Swipe to discover 4 essential design principles that top performers swear by." Hashtags auto-suggested: #WorkspaceDesign #Productivity #OfficeGoals #RemoteWork (reach estimate: 12K). First comment scheduled with additional hashtags.


## ❓ FAQ

**Q: Can my AI automatically find the scheduled posts for the next 7 days?**
Yes! Use the `list_schedules` tool. Your agent will respond with complete metadata for all upcoming posts, including channel names, scheduled times, and content previews in seconds.

**Q: How do I find my Planly API Key?**
Log in to your Planly account, navigate to **Settings** > **Security**, and you will find your unique secret API key (Bearer Token) there.

**Q: Can I use the AI to generate captions?**
Absolutely. Use the `ai_complete` tool. Provide your prompt or post idea, and the agent will utilize Planly's integrated AI to return professional copy options.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/planly](https://vinkius.com/mcp/planly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Planly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `planly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Planly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "planly": {
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
