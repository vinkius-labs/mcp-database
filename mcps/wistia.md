# Wistia MCP Server

Manage video assets, projects, and engagement analytics on Wistia — the leading video marketing platform for business.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/wistia)

## Overview
**Category:** marketing-automation
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Wistia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wistia](https://vinkius.com/mcp/wistia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
