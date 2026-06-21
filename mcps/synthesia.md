# Synthesia MCP Server

Connect your AI to Synthesia. Generate corporate AI avatar videos from text prompt, explore templates, and automatically dub existing media directly from the terminal.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/synthesia)

## Overview
**Category:** ai-frontier
**Tools Count:** 10

## Description
Bring the full power of synthetic enterprise video generation directly into your conversational environment with the **Synthesia** MCP connector. By granting your LLM authorized operational access to the Synthesia API matrix, you transform your assistant into a virtual studio director. Programmatically retrieve active templates, inspect available voice models, spawn new avatar streams from zero, or dub existing media seamlessly without navigating away from your terminal interface.

### What you can do

- **Virtual Directing** — Instantiate real-time video renderings using `create_avatar_video`, mapping structural inputs to specific avatar matrices found via `list_avatars`.
- **Template Automation** — Process repetitive layouts logically calling `create_video_from_template`, assigning JSON payloads seamlessly over defined blueprints.
- **Studio Lifecycle Management** — Query active rendering progress cleanly with `get_video_details` and prune discarded tracks strictly invoking `delete_video`.
- **Localization & Dubbing** — Effortlessly pull native voice ranges (`list_voices`) and trigger AI localized dubbing routines targeting existing records utilizing `dub_video`.

### How it works

1. Append the generic Synthesia MCP module firmly inside your Vinkius connective logic rules.
2. Locate your specific account authorization `SYNTHESIA_KEY` (tied to Synthesia Creator plans and beyond) and pass it to your host configuration.
3. Prompt video creations natively: "List all available avatars, pick a professional-looking one, and generate a video track saying 'Welcome to the Team!' in 'pt-BR'."

### Who is this for?

- **Corporate Training Leads** — Programmatically dispatch multi-lingual instructional videos evaluating template arrays generating bulk outputs seamlessly.
- **Internal Comms Engineers** — Eliminate manual studio workflows assigning custom scripts strictly inside automated pipelines using the AI interface directly.
- **Localization Teams** — Rapidly inspect voice definitions natively scaling video catalogs commanding dynamic `dub_video` requests effortlessly.


## Available Tools
- **create_avatar_video**: Returns a video ID.

Creates an AI avatar video from a script
- **create_video_from_template**: Returns a video ID.

Creates a video using a pre-defined Synthesia template
- **get_video_details**: Retrieves status and details for a specific video
- **list_videos**: Lists all videos in the account
- **delete_video**: This action is irreversible.

Permanently deletes a Synthesia video
- **list_avatars**: Lists all available AI avatars
- **list_templates**: Lists available video templates
- **get_template_details**: Retrieves details for a specific template
- **list_voices**: Lists available AI voices
- **dub_video**: Dubs an existing video into another language


## Installation & Usage

To install and use the **Synthesia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/synthesia](https://vinkius.com/mcp/synthesia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
