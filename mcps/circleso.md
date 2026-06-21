# Circle.so MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/circleso)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage online communities via Circle — track members, monitor posts, and manage spaces directly from any AI agent.

## Description
Connect your **Circle.so** community to any AI agent and take full control of your community management through natural conversation. Streamline how you engage with members and monitor content.

### What you can do

- **Member Oversight** — List and retrieve details for all community members and their profile information natively
- **Space Intelligence** — Access and monitor all spaces and space groups within your community flawlessly
- **Content Tracking** — List recent posts and comments to stay updated on community discussions securely
- **Event Management** — Access upcoming and past community events and retrieve detailed metadata flawlessly
- **Topic Oversight** — Monitor discussion topics to understand what your community is talking about securely
- **Admin Insights** — Retrieve your own admin profile and core community metadata directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Circle API Token (obtained from Settings > API)
3. Start managing your community from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Community Managers** — monitor member engagement and review recent posts using natural language
- **Course Creators** — audit student profiles and space activity without opening the dashboard
- **Membership Owners** — quickly look up member details and discussion history straight from their chat interface
- **Event Coordinators** — verify event schedules and attendee information


## Available Tools
- **list_community_posts**: List recent posts in the community
- **list_space_groups**: List groups that organize spaces
- **list_community_spaces**: List all spaces (sub-communities) in the community
- **list_community_topics**: List discussion topics
- **get_my_circle_profile**: Retrieve information about the authenticated admin user
- **list_post_comments**: List comments for a specific post
- **list_community_events**: List upcoming and past community events
- **list_community_members**: List all members in the community


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Circle.so** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all spaces in my Circle community."

**🤖 AI Agent:**
> Retrieving your community spaces... I found 8 spaces including 'Announcements', 'General Discussion', 'Course Module 1', and 'Q&A'. Which one would you like to see posts for?

---

**👤 You:**
> "Show me the last 5 posts in the 'General Discussion' space."

**🤖 AI Agent:**
> Retrieving recent posts from General Discussion... I found 5 items. The most popular one is 'Welcome to the community!' by Jane Smith with 12 comments.

---

**👤 You:**
> "What are the upcoming community events?"

**🤖 AI Agent:**
> Checking the event calendar... You have 2 upcoming events: 'Weekly Office Hours' (Tomorrow at 2 PM) and 'Monthly Guest Speaker' (Next Friday at 10 AM).


## ❓ FAQ

**Q: Can I see who the most recent members to join are?**
Yes! Use the `list_community_members` tool. The agent will return a list of members, and you can see their join dates and profile details directly.

**Q: How do I see the comments for a specific post?**
Use the `list_post_comments` tool with the unique post ID. Your agent will fetch all comments, allowing you to review the discussion without leaving your chat.

**Q: Where do I find my Circle API Token?**
Log in to your Circle community as an admin, go to **Settings**, and select **API**. You can generate and copy your token from that section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/circleso](https://vinkius.com/mcp/circleso)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Circle.so** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `circleso` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Circle.so** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "circleso": {
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
