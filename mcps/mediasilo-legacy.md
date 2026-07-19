# MediaSilo (Legacy) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mediasilo-legacy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Share and review video content with creative teams using secure media workspaces, annotations, and approval workflows.

## Description
Connect your **MediaSilo (Legacy)** account to any AI agent and manage video production workflows through natural conversation.

### What you can do

- **Project Management** — Create and manage workspaces and projects
- **Asset Browsing** — Search and browse video files, images, and documents
- **Link Sharing** — Create secure, password-protected review links
- **Review Tracking** — Monitor comments, approvals, and annotations
- **Analytics** — Track viewer engagement, drop-offs, and playback stats

### How it works

1. Subscribe to this server
2. Enter your MediaSilo API Key and API Secret
3. Start managing your media assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Post-Production** — manage dailies, cuts, and client reviews
- **Agencies** — share video pitches and track client engagement
- **Video Editors** — automate file organization and sharing workflows


## Available Tools (11)
- **get_user**: Get details for a specific MediaSilo user
- **get_current_user**: Get current authenticated MediaSilo user
- **list_project_users**: List users assigned to a specific MediaSilo project
- **list_projects**: List projects in the MediaSilo account
- **list_quicklinks**: List all QuickLinks in the MediaSilo account
- **list_users**: List all users in the MediaSilo account
- **list_assets**: List all assets in the MediaSilo account
- **list_folder_assets**: List assets within a specific MediaSilo folder
- **get_asset**: Get details for a specific MediaSilo asset
- **get_project**: Get details for a specific MediaSilo project
- **get_quicklink**: Get details for a specific MediaSilo QuickLink


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MediaSilo (Legacy)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the latest 'Director's Cut' asset and create a review link."

**🤖 AI Agent:**
> Found asset: 'Commercial_v3_Directors_Cut.mp4' (ID: 890, 450MB, Project: 'Summer Campaign'). Review link created ✅. URL: https://links.shift.io/review/abc123xyz. [REDACTED]. Expires in: 7 days.

---

**👤 You:**
> "Show comments and approvals for the Summer Campaign video."

**🤖 AI Agent:**
> Status: 3 pending, 1 approved. Comments: 4. @0:12 (Client): 'Can we make the logo slightly bigger here?'. @0:45 (Director): 'Color grading looks a bit washed out, let's boost contrast.' Approved by: Sarah (Producer) ✅.

---

**👤 You:**
> "Show viewer engagement analytics for the Q1 Pitch link."

**🤖 AI Agent:**
> Q1 Pitch Analytics: 45 unique views. Total watch time: 18 hours. Average completion: 78%. Drop-off spike: @1:45 (Pricing slide, 12 viewers stopped watching). Top viewers: Apple Inc. (12 views), Internal (5 views).


## ❓ FAQ

**Q: Can I create secure review links?**
Yes. Generate password-protected, expiring links for external clients to review video assets.

**Q: How does MediaSilo authentication work?**
It requires both an **API Key** and **API Secret** sent via custom headers against `api.shift.io/v3`.

**Q: Can I track viewer engagement on videos?**
Yes. Track playbacks, total watch time, drop-off points, and specific timestamp comments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mediasilo-legacy](https://vinkius.com/mcp/mediasilo-legacy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MediaSilo (Legacy)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mediasilo-legacy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MediaSilo (Legacy)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mediasilo-legacy": {
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
