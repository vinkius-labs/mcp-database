# Wistia MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wistia-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage videos, projects, and performance analytics on Wistia with AI agents.

## Description
Connect your **Wistia** video marketing account to any AI agent to automate your media library management and performance monitoring through natural conversation. Wistia provides a premier platform for B2B video hosting, delivery, and detailed engagement tracking.

### What you can do

- **Media Orchestration** — List and retrieve detailed metadata for your videos (medias), including titles, descriptions, and statuses.
- **Project Management** — Organize your content by creating and managing hierarchical projects (folders) directly from the AI interface.
- **Engagement Analytics** — Retrieve real-time performance stats for specific videos or get an aggregated overview of your account-wide metrics.
- **Metadata Control** — Programmatically update video details and manage captions to ensure your media library is always optimized.
- **Asset Delivery** — Fetch player configurations and thumbnail URLs to streamline content distribution across your digital channels.

### How it works

1. Subscribe to this server
2. Enter your Wistia API Token from your account settings
3. Start managing your video assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Teams** — automate the monitoring of video engagement and organize media assets via natural language.
- **Video Producers** — quickly update video titles and retrieve media links without leaving the project workspace.
- **Business Analysts** — get instant account-wide video performance reports and visitor metrics straight through the chat.


## Available Tools (9)
- **list_video_captions**: List captions for a video
- **list_videos**: List all videos (medias)
- **list_projects**: List your Wistia projects
- **update_video_details**: Modify video metadata
- **create_project**: Create a new project
- **get_account_analytics**: Get account-wide stats
- **get_video_details**: Get metadata for a video
- **get_project_details**: Get metadata for a project
- **get_video_stats**: Get video analytics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wistia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in my Wistia account."

**🤖 AI Agent:**
> I've retrieved your projects. You have 4 active folders: 'Product Demos', 'Customer Testimonials', 'Internal Training', and '2024 Ad Campaign'. Which one should we check?

---

**👤 You:**
> "Show the engagement stats for video ID 'vid123'."

**🤖 AI Agent:**
> Fetching analytics... Video 'vid123' has 1,250 total plays, with an average engagement of 68% and 420 unique visitors. Would you like a more detailed breakdown?


## ❓ FAQ

**Q: How do I find my Wistia API Token?**
Log in to Wistia, navigate to **Account Settings** > **API**, and generate a new token or copy an existing one from the list.

**Q: What is a 'hashed_id'?**
A `hashed_id` is a unique, short identifier assigned to every video and project in Wistia, typically found in the URL when viewing an asset.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wistia-alternative](https://vinkius.com/mcp/wistia-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wistia** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wistia-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wistia** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wistia-alternative": {
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
