# AppGallery Connect MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/appgallery-connect)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your AppGallery Connect apps via AI — check stats, submit builds for review, monitor ratings, and reply to user comments.

## Description
Connect **AppGallery Connect** to your AI agent and manage your mobile app lifecycle through natural conversation.

### What you can do

- **App Management** — List all apps, view details, and check localization settings
- **Build Submission** — Get upload URLs and submit builds for review with status tracking
- **Analytics** — Access download stats, installation metrics, and performance data
- **User Feedback** — Read ratings, browse user comments, and reply directly
- **Review Pipeline** — Track submission status through the moderation process

### How it works

1. Subscribe to this server
2. Get your AGC Client ID and Secret from Users and Permissions > API Key in the console
3. Start managing your apps from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Mobile Developers** — submit builds and check review status without opening the console
- **Product Managers** — monitor download and install metrics instantly
- **Support Teams** — respond to user reviews and feedback across apps


## Available Tools (11)
- **get_app_language_info**: g. "en-US", "zh-CN", "pt-BR").

Get localized app information for a specific language
- **get_download_stats**: Dates must be in YYYYMMDD format.

Get download statistics for an application
- **get_install_stats**: Dates must be in YYYYMMDD format.

Get installation statistics for an application
- **get_rating_info**: Get rating and review summary for an application
- **get_submission_status**: Check the review status of a submitted application
- **get_upload_url**: Specify the file suffix (e.g. "apk", "png").

Get a pre-signed upload URL for app binaries or assets
- **list_apps**: List all applications in the AppGallery Connect account
- **reply_to_comment**: Use get_comments to find comment IDs.

Reply to a user comment on the AppGallery
- **get_app_info**: The appId can be found via list_apps.

Get detailed information for a specific application
- **get_comments**: Get user comments and reviews for an application
- **submit_for_review**: The app must have all required metadata and at least one valid binary uploaded.

Submit an application for review and publication


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AppGallery Connect** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show download stats for my top app this month."

**🤖 AI Agent:**
> Your top app 'MegaGame' had 12,450 downloads this month, up 23% from last month. Daily average: 415 downloads. Peak day: March 15 with 892 downloads. Install rate: 78%. Want to see user ratings?


## ❓ FAQ

**Q: Can I submit an app build for review?**
Yes! Use `get_upload_url` to get a pre-signed upload URL, then `submit_for_review` to push the build through the moderation pipeline. You can track progress with `get_submission_status`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appgallery-connect](https://vinkius.com/mcp/appgallery-connect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AppGallery Connect** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `appgallery-connect` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AppGallery Connect** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "appgallery-connect": {
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
