# Frame.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/frameio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Collaborate on video, manage creative assets, and track comments via AI agents with Frame.io.

## Description
Connect your **Frame.io** account to any AI agent to automate your video collaboration and creative workflows through the Model Context Protocol (MCP). Frame.io is the industry-leading platform for reviewing and approving media, allowing teams to stay in sync from anywhere in the world. This MCP server enables you to manage your projects, retrieve asset metadata, and participate in time-coded discussions directly through natural conversation.

### Key Features

- **Project Oversight** — List all projects within your teams and fetch detailed metadata including ownership and status.
- **Asset Management** — List files and folders within projects and retrieve complete metadata for specific media assets.
- **Collaborative Feedback** — List all comments on an asset and add new time-coded feedback directly from your chat interface.
- **Review Coordination** — Access and list review links to monitor how your media is being shared with external stakeholders.
- **Team Interaction** — List team members and collaborators to maintain full context of who is involved in each project.
- **Directory Structure** — Navigate through folders and sub-folders within your project library to organize your work effectively.
- **Real-time Monitoring** — Fetch specific asset details or comments to keep your post-production workflow moving fast.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Frame.io Personal Access Token (found in the Developer Portal)
3. Start managing your video collaboration from Claude, Cursor, or any MCP client

### Who is this for?

- **Video Editors & Producers** — quickly check for new comments or update project statuses without leaving your primary agent.
- **Creative Directors** — get a real-time overview of review links and project progress across multiple teams.
- **Post-Production Managers** — automate the retrieval of asset metadata and feedback threads for audit and reporting.


## Available Tools
- **add_comment**: Post a new comment
- **get_asset_details**: Get asset metadata
- **get_my_profile**: Get current user profile
- **get_project_details**: Get project metadata
- **list_accounts**: List billing accounts
- **list_assets**: List assets or folder contents
- **list_collaborators**: List project collaborators
- **list_asset_comments**: List comments on an asset
- **list_folders**: List folders in project
- **list_projects**: List projects in a team
- **list_review_links**: List project review links
- **list_teams**: List Frame.io teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Frame.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my projects in Frame.io team 'team_abc123'."

**🤖 AI Agent:**
> Retrieving projects... I found 4 active projects in your team, including 'Spring Campaign' and 'Product Launch Video'. Would you like to see the assets for any of these?

---

**👤 You:**
> "Show me the last 5 comments on video asset 'vid_9876'."

**🤖 AI Agent:**
> Fetching comments... I found 5 recent updates for 'vid_9876', including a request to 'fix the color grade at 00:45' and a note about 'audio levels being too low'.

---

**👤 You:**
> "Add a comment to 'vid_9876': 'Great work, let\'s proceed to export' at 120 seconds."

**🤖 AI Agent:**
> Comment added! Your feedback has been successfully posted to 'vid_9876' at the 02:00 mark. Your team will see your approval in the project timeline.


## ❓ FAQ

**Q: How do I get an Access Token for Frame.io?**
You can generate a Personal Access Token in the Frame.io Developer Portal at https://developer.frame.io.

**Q: Can I add comments with a specific timecode using the agent?**
Yes! The 'add_comment' tool accepts an optional 'timestamp' parameter in seconds, allowing you to pin your feedback to a specific moment in the video.

**Q: How do I see the assets inside a specific folder?**
Use the 'list_assets' tool and provide the Folder ID as the 'parentId'. The agent will return all files and sub-folders contained within that directory.

**Q: Is it possible to list external review links?**
Yes! Use the 'list_review_links' tool and provide the Project ID. The agent will retrieve all active shared links for that project.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/frameio](https://vinkius.com/mcp/frameio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Frame.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `frameio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Frame.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "frameio": {
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
