# Postproxy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/postproxy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage your Google Business Profile posts, reviews, and local SEO presence across multiple locations from one dashboard.

## Description
### What you can do
- **Automated Publishing:** Create, publish, or schedule posts across various social media platforms directly via your AI Agent.
- **Profile Management:** List connected social profiles and group them to streamline multi-platform campaigns.
- **Post Management:** Retrieve, filter by status, and delete specific posts on the fly.
- **Engagement Handling:** Read comments, reply, like, or hide specific interactions seamlessly.

### How it works
1. Connect your Postproxy account.
2. Provide your secure API token.
3. Ask your AI Agent to schedule posts, manage comments, or list your available profiles.

### Who is it for?
Marketing teams, social media managers, and developers looking to integrate Postproxy for AI Agents to streamline multi-channel social media campaigns and audience engagement.


## Available Tools (11)
- **createCommentReply**: Reply to a comment on a post in Postproxy
- **createPost**: Provide text, status, and the list of profile IDs to publish to.

Create a new post in Postproxy
- **deletePost**: Delete a post in Postproxy
- **getPost**: Get a specific post by ID in Postproxy
- **hideComment**: Hide a comment on a post in Postproxy
- **likeComment**: Like a comment on a post in Postproxy
- **listComments**: List comments for a specific post in Postproxy
- **listPosts**: List posts in Postproxy
- **listProfileGroups**: List all profile groups in Postproxy
- **listProfiles**: List all social media profiles connected to Postproxy
- **unhideComment**: Unhide a comment on a post in Postproxy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Postproxy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my available social media profiles."

**🤖 AI Agent:**
> I have fetched your available social profiles from Postproxy. You currently have a Twitter and a LinkedIn account connected.

---

**👤 You:**
> "Schedule a new post for tomorrow morning announcing our new AI feature."

**🤖 AI Agent:**
> Your post has been successfully scheduled. It is set to be published tomorrow across your selected profiles.

---

**👤 You:**
> "Fetch the latest comments on my recent post."

**🤖 AI Agent:**
> Here are the latest comments from your recent post. Let me know if you would like me to reply or hide any of them.


## ❓ FAQ

**Q: Can the AI Agent schedule posts for any future date?**
Yes, as long as you provide a valid ISO date, your AI Agent can schedule posts using Postproxy.

**Q: Can I manage comments directly from the AI Agent?**
Absolutely. You can list, like, reply, hide, or unhide comments across your posts seamlessly.

**Q: Does the AI Agent support grouping profiles?**
Yes! The AI Agent can retrieve your Profile Groups so you can target multiple social media accounts at once.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/postproxy](https://vinkius.com/mcp/postproxy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Postproxy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `postproxy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Postproxy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "postproxy": {
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
