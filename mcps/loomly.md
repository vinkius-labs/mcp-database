# Loomly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/loomly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Plan and approve social media content with a collaborative calendar that streamlines reviews and keeps your brand consistent.

## Description
Connect your **Loomly** account to any AI agent and manage social media through natural conversation.

### What you can do

- **Calendar Management** — Browse content calendars and scheduled posts
- **Post Scheduling** — Create and schedule posts across social channels
- **Content Tracking** — Monitor posts through approval workflows
- **Engagement Analytics** — Track likes, shares, comments, and reach
- **Channel Management** — Monitor connected social accounts

### How it works

1. Subscribe to this server
2. Enter your Loomly Access Token
3. Start managing social media from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Social Media Managers** — schedule posts and track performance
- **Marketing Teams** — manage content calendars and approvals
- **Agencies** — coordinate multi-client social calendars


## Available Tools
- **create_new_post**: Add a new post to a calendar
- **get_calendar_details**: Get metadata for a calendar
- **get_user_profile**: Get your Loomly profile
- **get_post_details**: Get details for a post
- **list_media_assets**: List media in the library
- **list_calendars**: List your Loomly calendars
- **list_post_interactions**: List comments and replies
- **list_calendar_posts**: List posts in a calendar


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Loomly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show this week's content calendar and upcoming scheduled posts."

**🤖 AI Agent:**
> This week: 12 posts scheduled. Mon: Instagram Story (10 AM), LinkedIn article (2 PM). Tue: Twitter thread (9 AM), Facebook post (12 PM). Wed: Instagram Reel (11 AM). Thu: LinkedIn post (3 PM), Twitter (10 AM). Fri: Instagram carousel (12 PM), Facebook (2 PM). Status: 8 approved ✅, 3 pending review, 1 draft. Next: 'Product Launch Teaser' — Instagram, tomorrow 10 AM.

---

**👤 You:**
> "Show post performance analytics for this month."

**🤖 AI Agent:**
> This month: 42 posts published. Total reach: 145K. Engagement: 8.2K (5.6% rate ⭐). Top: 'Product Demo Video' — Instagram Reel (28K reach, 2.1K likes, 89 comments). Worst: 'Blog link share' — Twitter (450 reach, 3 likes). By channel: Instagram (18 posts, 6.8% eng), LinkedIn (10, 4.2%), Twitter (8, 3.1%), Facebook (6, 5.5%). Best time: Tue 10 AM.

---

**👤 You:**
> "Show posts pending approval and connected social channels."

**🤖 AI Agent:**
> Pending approval: 3 posts. 1) 'Q2 Roadmap Update' — LinkedIn (Sarah submitted, awaiting manager). 2) 'Customer Spotlight' — Instagram (Mike, awaiting design). 3) 'Weekend Sale' — Facebook (Lisa, awaiting copy edit). Channels: 5 connected. Instagram (@brand, 12K followers), LinkedIn (Company, 8.5K), Twitter (@brand, 5.2K), Facebook (Page, 15K), TikTok (@brand, 3.1K).


## ❓ FAQ

**Q: Can I schedule posts and manage content calendars?**
Yes. Create and schedule posts across connected social channels. Browse content calendars with status and approval workflows.

**Q: Can I track engagement and social analytics?**
Yes. Monitor likes, shares, comments, and reach per post. Track engagement trends and best performing content.

**Q: What API does Loomly use?**
Bearer authentication against `api.loomly.com/v1`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/loomly](https://vinkius.com/mcp/loomly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Loomly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `loomly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Loomly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "loomly": {
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
