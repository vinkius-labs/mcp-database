# Figma MCP Server

Connect Figma to automate design workflows — inspect files, render layers as images, and manage comments directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/figma)

## Overview
**Category:** industry-titans
**Tools Count:** 15

## Description
Figma is the leading collaborative interface design tool. This MCP server allows your AI agent to interact with your Figma files, projects, and teams flawlessly.

### Key Features
- **File & Node Inspection** — Retrieve the full document tree or specific layers to analyze design structures flawlessly.
- **Image Rendering** — Render Figma frames, components, or layers into PNG, SVG, or PDF images flawlessly native.
- **Team & Project Orchestration** — List team projects and project files to navigate your design workspace flawlessly.
- **Design Token Access** — Extract published components, styles, and local variables to sync with codebases flawlessly.
- **Collaboration Tools** — Read and post comments directly on design files to keep feedback loops active synchronously.
- **Version History** — Access file version history to track design evolutions flawlessy through the agent.

### How it works
1. Subscribe to this server
2. Enter your Figma Personal Access Token (found in Account Settings)
3. Start managing your design assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Product Designers** — automate documentation and asset handoff without manual exports
- **Frontend Developers** — extract design tokens, styles, and component metadata directly into your code workflow
- **Product Managers** — monitor design progress and review comments through simple natural language queries


## Available Tools
- **delete_comment**: Requires file key and comment ID.

Delete a comment from a Figma file
- **get_component_set**: Get metadata for a published component set
- **get_team_info**: Get metadata about a Figma team
- **get_images**: Render nodes from a Figma file as images
- **get_local_variables**: List design tokens/variables in a Figma file
- **list_components**: List published team components
- **get_me**: Get details for the authorized Figma user
- **get_comments**: Get comments on a Figma file
- **get_file_nodes**: Get specific nodes from a Figma file
- **get_file**: Use depth to limit node traversal (1=pages only, 2=pages+top frames).

Get a Figma file
- **get_file_versions**: List versions of a Figma file
- **list_project_files**: List files in a project
- **list_styles**: List published team styles
- **list_team_projects**: List projects in a Figma team
- **post_comment**: Post a comment on a Figma file


## Installation & Usage

To install and use the **Figma** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/figma](https://vinkius.com/mcp/figma)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
