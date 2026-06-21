# Facebook Pages MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/facebook-pages)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Facebook Pages via AI — publish posts, list feed, track insights, and engage with comments directly through your agent.

## Description
Connect your **Facebook Pages** account to any AI agent and take full control of your social media presence through natural conversation.

### What you can do

- **Post Management** — Publish new updates, list your recent feed, and delete posts directly from the cloud
- **Audience Engagement** — List and reply to comments on your posts to keep your community active
- **Performance Insights** — Track impressions, engagement, and fan growth metrics with simple queries
- **Media Access** — List photos and videos uploaded to your page to manage your visual content
- **Page Settings** — Inspect your page configuration and identity details through the agent

### How it works

1. Subscribe to this server
2. Enter your Facebook Page Access Token and Page ID
3. Start managing your Facebook presence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Social Media Managers** — quickly publish updates and monitor engagement across your pages
- **Content Creators** — check post performance and reply to fans without leaving your productivity flow
- **Marketing Teams** — pull insights and manage page content directly from your AI-powered workflow


## Available Tools
- **delete_post**: Delete a post from the Facebook Page
- **get_me**: Get current token identity info (Page info)
- **get_page_info**: Get basic info for the Facebook Page
- **get_page_insights**: Get performance insights for the Facebook Page
- **get_page_settings**: Get settings for the Facebook Page
- **get_post_details**: Get details for a specific post
- **list_page_photos**: List photos on the Facebook Page
- **list_page_posts**: List posts on the Facebook Page feed
- **list_page_videos**: List videos on the Facebook Page
- **list_post_comments**: List comments on a specific post
- **publish_post**: Publish a new post to the Facebook Page
- **reply_to_comment**: Reply to a comment on the Facebook Page


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Facebook Pages** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my latest posts on the Facebook Page."

**🤖 AI Agent:**
> I've retrieved your feed. You have 5 recent posts, including 'Welcome to our Spring Sale!' (ID: 101) and 'New Product Launch' (ID: 102). Would you like to see the insights for any of these?

---

**👤 You:**
> "Publish a post saying 'We are open this weekend!'"

**🤖 AI Agent:**
> Post published successfully! Your update 'We are open this weekend!' is now live on your Facebook Page with ID 12059340212.

---

**👤 You:**
> "Show me the insights for my page performance."

**🤖 AI Agent:**
> Analyzing insights... Your page had 5,000 impressions and 450 engagements over the last 7 days. Your total fan count has grown by 2% this week.


## ❓ FAQ

**Q: How do I get a Facebook Page Access Token?**
You can generate a Page Access Token via the [**Meta Graph API Explorer**](https://developers.facebook.com/tools/explorer/) by selecting your Page and requesting the necessary permissions (e.g., `pages_manage_posts`).

**Q: Can I reply to user comments using this agent?**
Yes! Use the `reply_to_comment` tool with the specific Comment ID and your message. Your AI will post the reply directly to the Facebook Page thread.

**Q: What insights can I track for my page?**
The `get_page_insights` tool retrieves core metrics like total impressions, overall engagement, and fan growth history to help you analyze your page's performance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/facebook-pages](https://vinkius.com/mcp/facebook-pages)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Facebook Pages** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `facebook-pages` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Facebook Pages** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "facebook-pages": {
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
