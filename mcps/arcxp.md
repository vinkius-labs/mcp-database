# ArcXP MCP Server

Automate newsroom publishing via ArcXP — manage, search, and update articles, photos, and videos directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/arcxp)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **ArcXP** environment to any AI agent and take full control of your newsroom CMS through natural conversation.

### What you can do

- **Content Management** — Create, fetch, update, and forcefully delete Arc Native Schema (ANS) stories directly without entering the Editor
- **Advanced Search** — Query your entire CMS library using powerful Elasticsearch-based syntax to find specific articles or historical reports
- **Media Library** — Search and retrieve high-resolution photo assets, thumbnails, and transcoding stream playlists for videos
- **Author Service** — List newsroom publishers, query specific reporter biographies, and manage author profiles

### How it works

1. Subscribe to this server
2. Enter your ArcXP Environment URL and Access Token
3. Start managing your digital publications from Claude, Cursor, or any MCP-compatible client

No more wrestling with complex ANS JSON schemas or slow CMS interfaces. Your AI acts as your ultimate publishing assistant.

### Who is this for?

- **Editors & Journalists** — quickly update breaking news, fetch related archive material, and orchestrate media without leaving your writing workflow
- **Media engineering teams** — automate bulk content updates and sanitize raw CMS payloads seamlessly
- **Digital publishers** — accelerate content velocity by letting AI structure, tag, and publish straight to your ArcXP tenant


## Available Tools
- **create_ans_content**: The payload_json MUST strictly comply with the requested Arc Native Schema (ANS) version.

Create new content in the Arc XP Content CMS
- **delete_ans_content**: Use with extreme caution as this destroys datacenter assets irreversibly.

Delete content from the Arc XP Content CMS
- **get_ans_content**: Returns the complete JSON payload matching the Arc Native Schema (ANS).

Fetch content from the Arc XP Content API
- **get_content_author**: Retrieve a publisher profile/author from Arc XP
- **get_photo_asset**: Retrieve a specific photo asset from Arc XP Media Library
- **get_video_asset**: Retrieve a specific video asset from Arc XP Video Center
- **list_content_authors**: List authors available in the Arc XP Author Service
- **search_ans_content**: Returns matching ANS JSON objects.

Search for content residing in the Arc XP Newsroom
- **search_photo_assets**: Search for photo assets in the Arc XP Media Library
- **update_ans_content**: Required to publish revisions to articles.

Update existing content in the Arc XP Content CMS


## Installation & Usage

To install and use the **ArcXP** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arcxp](https://vinkius.com/mcp/arcxp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
