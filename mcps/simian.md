# Simian MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/simian)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Video sharing and collaboration platform.

## Description
The Simian MCP server enables your AI agent to manage your creative workflows. Retrieve media links, orchestrate review processes, and analyze viewer engagement directly from the chat interface.


## Available Tools (12)
- **add_project_comment**: Add a new comment or approval status to a file
- **create_reel**: Create a new reel
- **delete_media**: Permanently remove a file from the library
- **get_account_info**: Retrieve account details and usage statistics
- **get_media**: Get metadata for a specific media file
- **get_project_comments**: Retrieve comments and annotations for a project file
- **get_reel**: Get details of a specific reel
- **list_media**: List all media files in the library
- **list_projects**: List all active review and approval projects
- **list_reels**: List all created reels (presentations)
- **share_reel**: Send a reel to recipients via email or short link
- **update_media**: Update metadata for a media file


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Simian** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the review link for project 'Summer Campaign'."

**🤖 AI Agent:**
> Here is the secure review link for 'Summer Campaign': simian.com/review/1234

---

**👤 You:**
> "Summarize the analytics for my latest reel."

**🤖 AI Agent:**
> Your latest reel has 45 views, an average watch time of 1m 20s, and 5 new comments from the client.

---

**👤 You:**
> "Invite 'client@brand.com' to review project 104."

**🤖 AI Agent:**
> An invitation has been successfully sent to 'client@brand.com' for project 104.


## ❓ FAQ

**Q: Can I get the review link for a specific video project?**
Yes, just ask the agent for the presentation link of your project and it will fetch it securely.

**Q: How do I check engagement analytics on my shared reel?**
You can query the AI to summarize view counts, average watch times, and comments left by clients on your reel.

**Q: Is it possible to invite a reviewer via the chat?**
Yes! Provide the reviewer's email and the project ID, and the agent will dispatch a secure invite link.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simian](https://vinkius.com/mcp/simian)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Simian** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `simian` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Simian** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "simian": {
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
