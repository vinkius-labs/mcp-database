# Teyuto MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/teyuto)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Build your own video streaming platform with monetization, audience analytics, and content management for video creators.

## Description
Connect your **Teyuto** account to any AI agent and manage your video platform.

### What you can do

- **Video Management** — List and inspect videos with full metadata
- **Video Analytics** — View watch time, view counts, and engagement metrics
- **Collection Management** — List and inspect video collections
- **User Management** — List users and view detailed profiles
- **Channel Access** — Browse available channels
- **Subscription Plans** — View plan pricing and features


## Available Tools (10)
- **check_teyuto_status**: Verify API connectivity
- **get_collection**: Get collection details
- **get_user**: Get user details
- **get_video_analytics**: Get video analytics
- **get_video**: Get video details
- **list_channels**: List channels
- **list_collections**: List collections
- **list_subscriptions**: List subscriptions
- **list_users**: List all users
- **list_videos**: List all videos


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Teyuto** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my videos."

**🤖 AI Agent:**
> You have 45 videos. Top 3 by views: 'Getting Started' (12.3k views), 'Advanced Tips' (8.1k), 'Q&A Session' (5.7k).

---

**👤 You:**
> "Show analytics for video vid_001."

**🤖 AI Agent:**
> Video 'Getting Started': 12,340 views, 4,567 hours watch time, 78% completion rate, 92% positive engagement.

---

**👤 You:**
> "List all video collections."

**🤖 AI Agent:**
> You have 5 collections: 'Beginner Series' (8 videos), 'Pro Tips' (12 videos), 'Live Sessions' (6 videos).


## ❓ FAQ

**Q: Can my AI show video analytics?**
Yes. `get_video_analytics` returns view counts, watch time, and engagement data for any video.

**Q: How do I browse video collections?**
Use `list_collections` to see all collections, then `get_collection` for details including its videos.

**Q: Can I list users and check subscriptions?**
Yes. `list_users` shows all users and `list_subscriptions` shows all plans with pricing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/teyuto](https://vinkius.com/mcp/teyuto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Teyuto** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `teyuto` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Teyuto** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "teyuto": {
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
