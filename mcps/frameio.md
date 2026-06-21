# Frame.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/frameio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/frameio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/frameio-mcp)
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


## Installation & Usage

To install and use the **Frame.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/frameio](https://vinkius.com/mcp/frameio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
