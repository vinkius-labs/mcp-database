# Videco MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/videco)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Create and manage personalized videos via Videco u2014 launch campaigns, capture leads, and track analytics from your AI agent.

## Description
Connect your **Videco** account to any AI agent and manage personalized videos, campaigns, leads, and analytics through natural conversation.

### What you can do

- **Video Management** u2014 Create, list, and review personalized videos from your template library
- **Campaign Management** u2014 Create and monitor video campaigns with audience targeting and delivery metrics
- **Lead Tracking** u2014 Access all leads captured from video interactions with engagement scores
- **Video Analytics** u2014 View detailed metrics including views, watch time, drop-off points, and CTA click rates
- **Template-Based Creation** u2014 Generate new personalized videos instantly from existing templates

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Videco account settings
3. Start managing video campaigns from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales Teams** u2014 create personalized prospecting videos and track engagement per lead
- **Marketing Teams** u2014 launch video campaigns and monitor conversion metrics
- **Customer Success** u2014 send personalized onboarding videos and track completion rates


## Available Tools
- **check_videco_status**: Verify Videco API connectivity
- **create_campaign**: Create a campaign
- **create_video**: Create a personalized video
- **get_video_analytics**: Get video analytics
- **get_campaign**: Get campaign details
- **get_lead**: Get lead details
- **get_video**: Get video details
- **list_campaigns**: List all campaigns
- **list_leads**: List all leads
- **list_videos**: List all videos


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Videco** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my personalized videos."

**🤖 AI Agent:**
> You have 12 videos. The most viewed is 'Welcome Onboarding' with 3,400 views (4.2% CTR). 3 videos were created this month. Would you like analytics for any video?

---

**👤 You:**
> "Show analytics for video VID-2048."

**🤖 AI Agent:**
> Video VID-2048 'Product Demo': 1,200 views, avg watch time 2:34, completion rate 68%, CTA click rate 5.1%. 42 leads captured. Best performing day: Tuesday. Want to see lead details?

---

**👤 You:**
> "Create a campaign called 'Spring Launch' with video VID-2048."

**🤖 AI Agent:**
> Campaign 'Spring Launch' created with video VID-2048. Campaign ID: CMP-891. Ready to deploy. Would you like to set a target audience or schedule?


## ❓ FAQ

**Q: How do I create a personalized video via AI?**
Use the `create_video` tool with a name and template ID. The personalized video is generated instantly from your Videco templates.

**Q: Can I track video engagement and leads?**
Yes. Use `get_video_analytics` for views, watch time, and CTR, and `list_leads` to see all captured lead contacts with engagement scores.

**Q: How do I create and manage video campaigns?**
Use `create_campaign` with a name and video ID to launch a campaign, then `list_campaigns` and `get_campaign` to track performance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/videco](https://vinkius.com/mcp/videco)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Videco** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `videco` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Videco** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "videco": {
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
