# ContentStudio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/contentstudio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan, create, and schedule social media content across all channels with AI writing assistance and performance analytics.

## Description
Connect your **ContentStudio** account to any AI agent and take full control of your social media content workflows through natural conversation.

### What you can do

- **Post Management** — Create, schedule, list, and delete social media posts across multiple platforms simultaneously
- **Status Filtering** — Filter posts by status: draft, scheduled, published, or failed — to focus on what needs attention
- **Social Accounts** — View all connected social media profiles with platform type, follower counts, and connection status
- **Content Analytics** — Retrieve engagement metrics, follower growth, and per-post performance data (likes, shares, comments, reach)
- **Content Organization** — Browse categories for structured content planning
- **Media Library** — Access all uploaded images, videos, and files for reuse in future posts

### How it works

1. Subscribe to this server
2. Enter your ContentStudio API Key from your profile dropdown > API Key
3. Start managing your social content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Social Media Managers** — schedule posts across Instagram, Twitter, LinkedIn, and Facebook without opening ContentStudio
- **Marketing Teams** — track content performance and engagement metrics through conversational AI
- **Content Creators** — draft and queue posts using natural language while focusing on creative work


## Available Tools
- **check_contentstudio_status**: Verify connectivity
- **create_post**: Create a post
- **delete_post**: Delete a post
- **get_social_account**: Get social account details
- **get_analytics**: Get account analytics
- **get_post_analytics**: Get post analytics
- **get_post**: Get post details
- **list_social_accounts**: List social accounts
- **list_posts_by_status**: List posts by status
- **list_categories**: List categories
- **list_media**: List media library
- **list_posts**: List posts
- **list_workspaces**: List workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ContentStudio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a LinkedIn and Twitter post about our new product launch for tomorrow at 9am EST."

**🤖 AI Agent:**
> Post created and scheduled! Post ID: post_29401. Content: 'Exciting news — we're launching our newest product tomorrow! Stay tuned for details. #ProductLaunch #Innovation'. Scheduled for April 27 at 9:00 AM EST. Target accounts: LinkedIn (acc_112) and Twitter (acc_115). Would you like me to also add an image from your media library?

---

**👤 You:**
> "Show me all scheduled posts for this week and their engagement predictions."

**🤖 AI Agent:**
> Filtering by status 'scheduled'... You have 8 posts queued this week. Monday: 2 posts (LinkedIn case study, Instagram reel). Tuesday: 1 post (Twitter thread). Wednesday: 2 posts (LinkedIn carousel, Facebook announcement). Thursday: 1 post (Instagram story). Friday: 2 posts (LinkedIn article, Twitter poll). Would you like to see the content of any specific post or modify the schedule?

---

**👤 You:**
> "What were the top performing posts on our Instagram account last month?"

**🤖 AI Agent:**
> Fetching analytics for Instagram account (acc_118)... Your top 3 posts last month by engagement: 1) Product demo reel — 12,400 impressions, 842 likes, 156 comments. 2) Behind-the-scenes story — 9,200 impressions, 621 likes, 89 saves. 3) Customer testimonial carousel — 8,100 impressions, 534 likes, 72 shares. Total follower growth: +1,240 (3.2% increase). Would you like detailed analytics for any specific post?


## ❓ FAQ

**Q: Can I create and schedule posts to multiple social accounts at once?**
Yes! The `create_post` action accepts a JSON payload with content, media attachments, schedule date, and target account IDs. You can publish to Instagram, Twitter, LinkedIn, and Facebook simultaneously in a single command.

**Q: Can I track how individual posts are performing?**
Yes. Use `get_post_analytics` with a specific Post ID to retrieve likes, shares, comments, impressions, and reach for that post. For account-wide metrics, use `get_analytics` with the Social Account ID to see follower growth, engagement rates, and top-performing content.

**Q: Can I filter posts by their publishing status?**
Yes. The `list_posts_by_status` tool accepts a status parameter — 'draft', 'scheduled', 'published', or 'failed'. This lets you quickly find posts that need review (drafts), are queued for delivery (scheduled), or encountered errors during publishing (failed).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contentstudio](https://vinkius.com/mcp/contentstudio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ContentStudio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `contentstudio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ContentStudio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "contentstudio": {
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
