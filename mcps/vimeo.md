# Vimeo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vimeo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Vimeo account — audit videos, folders, and showcases via AI.

## Description
Empower your AI agent to orchestrate your entire video ecosystem on **Vimeo**, the world's most innovative video platform. By connecting Vimeo to your agent, you transform complex asset management into a natural conversation. Your agent can instantly list your videos, audit project folders, and retrieve performance stats without you ever touching a dashboard. Whether you are a professional filmmaker or a corporate communications lead, your agent acts as a real-time video operator, ensuring your content is always organized and accessible.

### What you can do

- **Video Auditing** — List all videos in your account and retrieve detailed metadata, including duration, plays, and privacy settings.
- **Folder Oversight** — Browse your project folders to maintain a clear view of your content organization.
- **Showcase Management** — List all showcases (albums) and channels to monitor your public video distribution.
- **Video Governance** — Update video titles, descriptions, and autonomously delete items when they are no longer needed.
- **Search Intelligence** — Query public videos across Vimeo to find inspiration or relevant community content.

### How it works

1. Subscribe to this server
2. Enter your Vimeo Access Token
3. Start managing your video assets through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Video Professionals** — monitor upload statuses and metadata straight from your production workflow.
- **Content Marketers** — verify if new videos have been correctly added to showcases and folders.
- **Account Admins** — perform rapid audits of video libraries and clean up old content without manual logins.
- **Operations Leads** — automate video querying to orchestrate cross-functional creative teams smoothly.


## Available Tools
- **delete_video**: Delete a video from Vimeo
- **get_me**: Get authenticated user info from Vimeo
- **get_video**: Get details for a specific video
- **list_channels**: List channels followed by a user
- **list_folders**: List folders (projects) for a user
- **list_groups**: List groups followed by a user
- **list_showcases**: List showcases (albums) for a user
- **list_videos**: List videos for a user
- **search_videos**: Search for public videos on Vimeo
- **update_video**: Update video metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vimeo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 videos in Vimeo."

**🤖 AI Agent:**
> I've retrieved your recent videos. You have 5 files, including 'Client Feedback V2' and 'Final Master'. Would you like the full metadata for any of them?

---

**👤 You:**
> "Show me my Vimeo project folders."

**🤖 AI Agent:**
> You have 3 projects in Vimeo: 'Corporate', 'Ads 2024', and 'Social Media'. I can list the videos inside any of these folders for you.

---

**👤 You:**
> "Search for public videos about 'Artificial Intelligence'."

**🤖 AI Agent:**
> I've found several public videos about 'Artificial Intelligence'. The top matches include 'The Future of AI' and 'Deep Learning Explained'. Would you like the links to watch them?


## ❓ FAQ

**Q: How do I find my Vimeo Access Token?**
Create a new app in the [**Vimeo Developer portal**](https://developer.vimeo.com/apps), generate a token with the necessary scopes (public, private, edit, delete), and paste it below.

**Q: Can the agent list private videos?**
Yes. If your Access Token has the correct scopes, your agent will be able to retrieve both public and private videos from your account.

**Q: Is it possible to manage folders via the agent?**
Yes. Use the `list_folders` tool to retrieve all project directories, allowing your agent to audit your content library's structure in real-time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vimeo](https://vinkius.com/mcp/vimeo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vimeo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `vimeo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vimeo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vimeo": {
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
