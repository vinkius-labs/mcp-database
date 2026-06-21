# Dailymotion MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dailymotion-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Dailymotion account — audit videos, playlists, and followers via AI.

## Description
Empower your AI agent to orchestrate your entire video ecosystem on **Dailymotion**, the innovative video sharing platform. By connecting Dailymotion to your agent, you transform complex asset management into a natural conversation. Your agent can instantly list your videos, audit playlist organization, and retrieve follower stats without you ever touching a dashboard. Whether you are a professional creator or a media brand, your agent acts as a real-time video operator, ensuring your content is always organized and your audience reach is monitored.

### What you can do

- **Video Auditing** — List all videos in your account and retrieve detailed metadata, including view counts and statuses.
- **Playlist Oversight** — Browse your playlists to maintain a clear view of your content categorization and sequencing.
- **Community Management** — List your followers and following lists to stay on top of your audience growth.
- **Video Governance** — Update video titles, descriptions, and autonomously delete items when they are no longer needed.
- **Search Intelligence** — Query public videos across Dailymotion to find relevant community content or inspiration.

### How it works

1. Subscribe to this server
2. Enter your Dailymotion Access Token
3. Start managing your video assets through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Video Creators** — monitor upload statuses and engagement metrics straight from your creation workflow.
- **Media Managers** — verify if new videos have been correctly categorized into playlists.
- **Account Admins** — perform rapid audits of video libraries and manage channel growth without manual logins.
- **Operations Leads** — automate video querying to orchestrate cross-functional content teams smoothly.


## Available Tools (9)
- **delete_video**: Delete a video from Dailymotion
- **get_me**: Get authenticated user info from Dailymotion
- **get_video**: Get details for a specific video
- **list_followers**: List followers for a user
- **list_following**: List following for a user
- **list_playlists**: List playlists for a user
- **list_videos**: List videos for a user
- **search_videos**: Search for public videos on Dailymotion
- **update_video**: Update video metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dailymotion** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 videos in my Dailymotion account."

**🤖 AI Agent:**
> I've retrieved your recent videos. You have 5 files, including 'Spring Launch' and 'Interview V1'. Would you like the view counts for any of them?

---

**👤 You:**
> "Show me my Dailymotion playlists."

**🤖 AI Agent:**
> You have 3 playlists in your account: 'Promos', 'Demos', and 'Tutorials'. I can list the videos inside any of these playlists for you.

---

**👤 You:**
> "How many followers do I have on Dailymotion?"

**🤖 AI Agent:**
> Checking your audience... You currently have 150 followers. I can list the most recent ones for you if you'd like.


## ❓ FAQ

**Q: How do I find my Dailymotion Access Token?**
Create an API Key in the [**Dailymotion Developer Portal**](https://developer.dailymotion.com/), and perform the OAuth flow to generate an Access Token. Copy and paste it below.

**Q: Can the agent list my followers?**
Yes. Use the `list_followers` tool providing your User ID (or 'me'). Your agent will retrieve the list of users currently following your channel.

**Q: Is it possible to search for videos via the agent?**
Yes. The `search_videos` tool allows your agent to query the entire Dailymotion public library using any search string, returning matching video metadata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dailymotion-alternative](https://vinkius.com/mcp/dailymotion-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dailymotion** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dailymotion-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dailymotion** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dailymotion-alternative": {
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
