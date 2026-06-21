# Cadmium Harvester MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cadmium-harvester)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cadmium-harvester-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cadmium-harvester-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

Manage educational event content via Cadmium — track presentations, speakers, and assets directly from any AI agent.

## Description
Connect your **Cadmium Education Harvester** account to any AI agent and orchestrate your event content management, speaker coordination, and presentation tracking through natural conversation.

### What you can do

- **Presentation Oversight** — List all presentations for an event and retrieve detailed metadata, including titles, IDs, and statuses.
- **Speaker Management** — List all presenters and retrieve detailed profiles, including contact info and association with sessions.
- **Asset Tracking** — List and access files, handouts, and presentation assets associated with individual sessions.
- **Event Coordination** — Retrieve core event details and settings straight from your workspace.
- **Content Auditing** — Monitor presentation counts and update information to ensure your event schedule is accurate.
- **Data Deep Dives** — Get detailed data for specific presenter or presentation IDs using natural language.

### How it works

1. Subscribe to this server
2. Enter your Cadmium API Key and Event Key
3. Start managing your educational content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Event Planners & Managers** — quickly check speaker statuses or presentation details without manual dashboard work.
- **Education Coordinators** — retrieve handouts and session metadata for attendee support straight from their workflow tools.
- **Digital Teams** — monitor content processing and asset availability using natural language.


## Available Tools
- **get_account_info**: Retrieve core account information
- **get_event_details**: Retrieve core event information
- **get_presentation_count**: Get total number of presentations
- **get_presenter_details**: Get details of a specific presenter
- **list_presentation_assets**: List files and assets associated with a presentation
- **list_presentations**: List all presentations for the event
- **list_presenters**: List all presenters/speakers for the event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cadmium Harvester** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all presentations for the current event in Cadmium."

**🤖 AI Agent:**
> I've retrieved your presentations. You have 25 sessions scheduled, including 'Modern Architecture' (ID: pres_1) and 'AI in Medicine' (ID: pres_2).

---

**👤 You:**
> "Show the profile for presenter with ID speaker_99283."

**🤖 AI Agent:**
> I've found the profile for Dr. Alice Johnson. She is a Lead Scientist at TechCorp and is presenting 2 sessions: 'Future of Web' and 'Coding Best Practices'.

---

**👤 You:**
> "List the assets associated with presentation pres_123."

**🤖 AI Agent:**
> Retrieving assets for pres_123... I found 3 files: 'Slides.pdf', 'Handout_Notes.docx', and 'BackgroundVideo.mp4'. Would you like the download links?


## Installation & Usage

To install and use the **Cadmium Harvester** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cadmium-harvester](https://vinkius.com/mcp/cadmium-harvester)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
