# Canva MCP Server

Empower your AI agents to manage Canva designs, upload branding assets, and trigger automatic exports directly from your chat.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/canva)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Connect your **Canva** account to any AI agent and take full control of your creative workflow through natural conversation.

### What you can do

- **Design Management** — List all your active designs, fetch complete details, and create new preset formats (Posters, Presentations).
- **Media Assets** — Upload external images or videos organically through AI, list storage assets, or delete outdated creative files.
- **Automated Exports** — Trigger asynchronous export jobs to turn your Canva cloud designs into PDFs, MP4s, or JPEGs automatically.
- **Brand Templates** — Retrieve organizationally approved brand templates to ensure aesthetic consistency.
- **User Insights** — Read metadata associated with the authenticated user profile and team capabilities.

### How it works

1. Subscribe to this server
2. Provide your Canva Client credentials and Connect your account
3. Command your agent to upload logos, fetch presentation links, or export visuals dynamically.

### Who is this for?

- **Social Media Managers** — Upload daily graphic assets directly to your Canva media library while scheduling campaigns.
- **Content Creatives** — Instruct the agent to fetch the raw JPEG exports of newly finalized Canva posters without opening multiple tabs.
- **Marketing Teams** — Quickly search your approved Brand templates to scaffold new presentations programmatically.


## Available Tools
- **list_designs**: List all designs on Canva. Canva is the leading online design platform. Returns design IDs, titles, types, and thumbnails
- **get_design**: Get full details of a Canva design including title, type, page count, dimensions, and created/updated timestamps
- **create_design**: Create a new Canva design. Supports preset types like Presentation, Poster, InstagramPost
- **export_design**: Export a Canva design to a file format. Supports PDF, JPEG, PNG, GIF, PPTX, MP4. Returns an export job ID
- **get_export**: Get the status of a Canva export job tracking completion progress returning a native physical download URL
- **list_assets**: List uploaded standard image or video graphical assets stored in the user Canva asset pipeline
- **upload_asset**: Upload an asset directly into the Canva storage context for future embedding into complex native designs
- **delete_asset**: Irreversibly delete an existing custom asset from the Canva platform structure
- **list_templates**: Retrieve the organizationally explicit Canva branded layout templates isolating core structural configurations
- **get_user**: Get standard metadata describing the authenticated Canva user and organizational bounds


## Installation & Usage

To install and use the **Canva** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/canva](https://vinkius.com/mcp/canva)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
