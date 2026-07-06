# CaptionHub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/captionhub)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Manage video localization via CaptionHub — track projects, automate transcription, and approve captions directly from any AI agent.

## Description
Connect your **CaptionHub** account to any AI agent and orchestrate your video localization, AI-powered transcription, and subtitle approval workflows through natural conversation.

### What you can do

- **Project Oversight** — List all localization projects and retrieve detailed metadata, including source and target languages.
- **Automated Transcription** — Trigger AI-powered auto-transcription for your video assets directly from your workspace.
- **Caption Lifecycle** — Handover, approve, or archive caption sets for specific languages using natural language.
- **Export Coordination** — Retrieve export links for finished captions in various formats straight from your workspace.
- **Workflow Automation** — Monitor active webhooks and project statuses to ensure your localization pipeline is efficient.
- **Data Deep Dives** — Get detailed data for specific project, caption, or user IDs using natural language.

### How it works

1. Subscribe to this server
2. Enter your CaptionHub API Key
3. Start localizing your video content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Localization Managers** — quickly check project statuses or trigger transcriptions without manual dashboard work.
- **Content Producers** — retrieve caption exports and monitor approval stages straight from their workflow tools.
- **Video Editors** — orchestrate subtitle workflows and verify asset metadata using natural language.


## Available Tools (10)
- **list_webhooks**: List all active webhooks
- **approve_captions**: Approve a caption set for a specific language
- **archive_project**: Archive a project permanently
- **create_project**: Create a new captioning project
- **export_captions**: Get the export URL for a caption set
- **get_account_info**: Retrieve core account information
- **get_project_details**: Get details of a specific project
- **list_projects**: List all video captioning projects
- **transcribe_video**: Trigger AI auto-transcription for a project
- **update_project**: Update project metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CaptionHub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current video projects in CaptionHub."

**🤖 AI Agent:**
> I've retrieved your projects. You have 5 active projects, including 'Product Keynote' (ID: proj_1) and 'Training Module v2' (ID: proj_2).

---

**👤 You:**
> "Start auto-transcription for the 'Product Keynote' project."

**🤖 AI Agent:**
> Auto-transcription has been triggered for 'Product Keynote' (ID: proj_1). I will monitor the progress and notify you when it's ready for review.

---

**👤 You:**
> "Get the French subtitle export link for project proj_123."

**🤖 AI Agent:**
> Retrieving French caption export... Your download link is ready: https://api.captionhub.com/exports/abcd-1234.srt


## ❓ FAQ

**Q: Can I trigger auto-transcription for a video using the agent?**
Yes! Use the `transcribe_video` tool with the Project ID. Your agent will trigger CaptionHub's AI engine to start transcribing the video content instantly.

**Q: How do I get the download link for finished subtitles?**
Simply ask the agent to `export_captions` and provide the Project ID and the language code (e.g., 'fr' or 'es'). It will return the export URL for your finished caption set.

**Q: Does the integration allow approving captions via the workspace?**
Yes. Use the `approve_captions` tool with the Project ID and Language. This will mark the specific caption set as approved in your CaptionHub workflow.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/captionhub](https://vinkius.com/mcp/captionhub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CaptionHub** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `captionhub` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CaptionHub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "captionhub": {
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
