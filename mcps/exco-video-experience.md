# EX.CO Video Experience MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/exco-video-experience)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage video libraries, track interactive content, and monitor analytics via the EX.CO API.

## Description
Integrate **EX.CO**, the leading video experience platform, directly into your AI workflow. Manage your video library and interactive content (quizzes, polls), track real-time performance analytics and engagement metrics, monitor distribution channels and playlists, and oversee your entire video strategy using natural language.

### What you can do

- **Video Oversight** — List and retrieve detailed information, durations, and metadata for all your hosted videos.
- **Interactive Content Intelligence** — Monitor quizzes, polls, and other interactive items, resolving configuration details and performance data.
- **Performance Management** — Access real-time video analytics, resolving total views, completions, and interaction rates via chat.
- **Content Auditing** — Retrieve high-level summaries of video volume, channel activity, and organizational content health instantly.

### How it works

1. Connect the EX.CO integration to your AI assistant.
2. Authorize using your EX.CO REST API Key (found in your account settings).
3. Orchestrate your video experience and content engagement strategy through intuitive conversation.

### Who is this for?

- **Content Creators & Marketers** — Quickly check video views and completion rates on the go.
- **Digital Publishers** — Research channel distribution and playlist metadata via chat.
- **Operations Teams** — Monitor interactive content performance and organizational EX.CO metadata instantly.


## Available Tools (10)
- **get_ex_co_account_metadata**: Retrieve metadata and limits for your EX.CO account
- **get_video_analytics_summary**: Get a high-level summary of video performance and engagement
- **get_content_detailed_intelligence**: Get detailed settings and performance data for a specific content item
- **quick_video_performance_audit**: Retrieve a high-level summary of videos and analytics
- **get_video_detailed_data**: Get detailed settings and metadata for a specific video
- **list_video_distribution_channels**: List all video channels configured in your organization
- **list_interactive_content**: List all interactive content items (quizzes, polls, etc.) in your account
- **list_video_playlists**: List all video playlists created in your account
- **list_successfully_published_videos**: Identify videos that are currently in a "Published" status
- **list_video_library**: CO API.

List all videos in your EX.CO library


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EX.CO Video Experience** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all videos in my library."

**🤖 AI Agent:**
> I've found 15 videos in your EX.CO library, including 'Product Launch 2024' and 'Tutorial - Getting Started'. 12 are currently 'Published'. Would you like to see the analytics for the Product Launch video?

---

**👤 You:**
> "Show me analytics summary for this week."

**🤖 AI Agent:**
> This week across your library, you have 15,000 total views and a 65% completion rate. The video 'Interactive Quiz - Q1' has the highest engagement (12%). Would you like to see the channel distribution breakdown?

---

**👤 You:**
> "Search for interactive content matching 'Quiz'."

**🤖 AI Agent:**
> I've found 3 interactive items matching 'Quiz': 'Customer Feedback Quiz', 'Product Knowledge Quiz', and 'Fun Personality Quiz'. All are currently 'Active'. Would you like the detailed performance for the Customer Feedback Quiz?


## ❓ FAQ

**Q: How do I get an EX.CO API Key?**
Log in to your EX.CO platform, navigate to **Settings > API Integration**, and you can generate or retrieve your unique **REST API Key** from there. Ensure you have the necessary organizational permissions.

**Q: Does the integration show real-time views?**
Yes, you can use the get_video_analytics_summary tool to retrieve the latest view counts, completions, and interaction metrics across your entire video library.

**Q: Can the agent upload new videos?**
This integration currently focuses on listing and auditing videos, interactive content, and analytics. Uploading or editing video assets should be managed via the EX.CO platform dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/exco-video-experience](https://vinkius.com/mcp/exco-video-experience)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EX.CO Video Experience** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `exco-video-experience` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EX.CO Video Experience** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "exco-video-experience": {
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
