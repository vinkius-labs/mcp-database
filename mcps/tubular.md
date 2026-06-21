# Tubular MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tubular)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Analyze social video performance across YouTube, Facebook, and TikTok with audience insights and competitive benchmarking.

## Description
Connect your **Tubular Labs** video intelligence account to any AI agent and simplify how you analyze digital video trends, creator performance, and cross-platform audience metrics through natural conversation.

### What you can do

- **Video Insights** — Retrieve detailed performance metrics and trending data for individual videos or categories across social platforms.
- **Creator Intelligence** — Search for creators and fetch high-level performance summaries, trends, and audience ratings.
- **Audience Demographics** — Analyze audience breakdowns (age, gender, location) for specific videos or creators to refine your targeting.
- **Sponsorship Tracking** — List brand sponsors and monitor sponsored video campaigns to understand the competitive landscape.
- **Audience Overlap** — Analyze shared audience between two creators or content properties to identify partnership opportunities.
- **Operational Monitoring** — Check API health and rate limits to ensure your intelligence engine is always running.

### How it works

1. Subscribe to this server
2. Enter your Tubular API Key (found in your developer settings)
3. Start analyzing the video ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **Media Agencies & Brands** — quickly identify high-performing creators and analyze sponsored content trends via simple AI commands.
- **Content Strategists** — monitor video trends and cross-platform audience demographics directly from the workspace.
- **Data Analysts** — retrieve granular video metrics and creator audience ratings via the AI assistant.


## Available Tools
- **get_audience_overlap**: Analyze shared audience between entities
- **get_audience_ratings**: Get reach and engagement ratings
- **get_creator_summary**: Get summary for a specific creator
- **get_creator_trends**: Get trends for a specific creator
- **check_api_health**: Check API health status
- **list_sponsored_campaigns**: List sponsored video campaigns
- **list_sponsors**: List sponsors and brand partners
- **get_api_rate_limits**: Get current API rate limits
- **search_creators**: g., name or keywords).

Search for creators
- **get_video_demographics**: ) for a specific video.

Get audience demographics for a video
- **get_video_insights**: Get insights for a specific video
- **get_video_trends**: List trending videos


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tubular** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for top gaming creators in my region."

**🤖 AI Agent:**
> I've searched the creator directory. Here are the top gaming creators: 'ProGamerX' (2.5M reach), 'EliteStreamer' (1.8M reach), and 'JoystickGuru'. Would you like performance trends for any of them?

---

**👤 You:**
> "Show me the audience overlap between creator 'A-101' and 'B-552'."

**🤖 AI Agent:**
> Analyzing overlap... Creator 'A-101' and 'B-552' share 15% of their audience. This suggests a potential opportunity for a unique collaboration with low redundancy. Shall I retrieve the demographic breakdown for the shared group?

---

**👤 You:**
> "List all active sponsored video campaigns from 'TechBrand Inc'."

**🤖 AI Agent:**
> Fetching campaigns... 'TechBrand Inc' currently has 3 active sponsored video campaigns: 'Holiday Tech Guide', 'Summer Unboxing Series', and 'Home Office Overhaul'. Would you like engagement metrics for the 'Holiday Tech Guide'?


## ❓ FAQ

**Q: Can I see the audience demographics for a specific YouTube video?**
Yes! Use the `get_video_demographics` tool and provide the Video ID. Your agent will retrieve the age and gender breakdowns for that specific piece of content.

**Q: How do I analyze the shared audience between two different creators?**
Use the `get_audience_overlap` tool and provide the IDs for both entities. The agent will return the percentage and metrics of the audience that both creators share.

**Q: Is it possible to see which brands are sponsoring a specific creator?**
Absolutely. Run the `list_sponsored_campaigns` query or search for sponsors using the `list_sponsors` tool to retrieve data on brand partnerships within the video ecosystem.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tubular](https://vinkius.com/mcp/tubular)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tubular** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tubular` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tubular** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tubular": {
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
