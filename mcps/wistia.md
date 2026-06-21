# Wistia MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wistia)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage video assets, projects, and engagement analytics on Wistia — the leading video marketing platform for business.

## Description
Connect your **Wistia** account to any AI agent and take control of your video marketing infrastructure through natural conversation.

### What you can do

- **Media Management** — List all video and audio assets in your account, including their durations, play counts, and direct asset URLs
- **Project Organization** — Create, browse, and manage folders (projects) to keep your media library organized across teams
- **Engagement Insights** — Retrieve detailed play rates, average percent watched, and viewer statistics directly from your agent
- **Metadata Control** — Update video titles and descriptions or permanently delete obsolete assets and all their derivatives
- **Remote Ingestion** — Trigger Wistia to download and host video content from any public URL into a specific project
- **Deep Discovery** — Quickly find unique hashed IDs for medias and projects required for automated marketing workflows
- **Asset Auditing** — Browse organizational containers and retrieve technical metadata for high-quality content delivery

### How it works

1. Subscribe to this server
2. Enter your Wistia API Token
3. Start managing your videos and projects through Claude, Cursor, or any MCP-compatible client

No more manual logging into the Wistia dashboard to find a video link. Your AI agent becomes your video operations manager.

### Who is this for?

- **Marketing Teams** — automate video metadata updates and monitor campaign engagement through chat
- **Content Managers** — organize large media libraries into projects and verify upload status from remote URLs
- **Product Developers** — quickly retrieve hashed IDs and direct asset URLs for embedded video applications
- **Data Analysts** — surface video performance metrics and viewer statistics without manual data exports


## Available Tools
- **create_new_project**: Provide a descriptive name.

Creates a new project to organize media
- **delete_media_asset**: This action is irreversible.

Permanently deletes a Wistia media asset and all its derivatives
- **delete_wistia_project**: Note: All videos in the project will be lost. This is irreversible.

Permanently deletes a Wistia project and all media contained within it
- **get_engagement_statistics**: Retrieves detailed engagement and viewer statistics for a video
- **get_media_details**: Retrieves comprehensive metadata for a specific Wistia media asset
- **get_project_details**: Retrieves details for a specific Wistia project, including all contained media
- **list_wistia_medias**: Lists all media assets (videos, audios) in the Wistia account
- **list_wistia_projects**: Lists all projects (folders) in the Wistia account
- **update_media_metadata**: Provide the hashed ID and a JSON object of attributes.

Updates the metadata (name, description) of a specific Wistia media
- **upload_video_via_url**: Provide the source URL, target project ID, and a name.

Triggers Wistia to download and host a video from a public URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wistia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my videos in Wistia."

**🤖 AI Agent:**
> I found 12 videos in your account. The most recent are 'Spring Launch Overview' (ID: abc123def), 'Product Demo v2' (ID: ghi456jkl), and 'Customer Story' (ID: mno789pqr). Would you like to see the performance stats for any of these?

---

**👤 You:**
> "What are the engagement stats for the video with ID 'abc123def'?"

**🤖 AI Agent:**
> Engagement summary for abc123def: Play rate is 42%, and the average watch time is 68%. Total plays: 1,250. The video is performing well compared to your project average.

---

**👤 You:**
> "Upload the video from 'https://example.com/promo.mp4' to my 'Campaigns' project."

**🤖 AI Agent:**
> Success! I've triggered Wistia to ingest 'promo.mp4' into your 'Campaigns' project (ID: proj-xyz). It will appear in your library once processing is complete. Is there anything else you need me to organize?


## ❓ FAQ

**Q: Can I check how many people finished watching a specific video?**
Yes. The `get_engagement_statistics` tool provides the average percent watched and other deep engagement metrics for any video, allowing you to analyze audience retention through chat.

**Q: How do I upload a video to Wistia if I only have a direct URL?**
You can use the `upload_video_via_url` tool. Simply provide the source URL and the target project ID, and Wistia will handle the ingestion and hosting of that video for you.

**Q: Is it possible to see the direct download link for my video files?**
Absolutely. Using the `get_media_details` tool, your agent can retrieve full technical properties, including the direct URLs for original files and transcoded versions hosted on Wistia's CDN.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wistia](https://vinkius.com/mcp/wistia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wistia** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `wistia` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wistia** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wistia": {
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
