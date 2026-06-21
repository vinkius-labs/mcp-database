# Figma MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/figma-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/figma-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/figma-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Access Figma design files, comments, components and images via API — inspect nodes, render exports and track version history from any AI agent.

## Description
Connect your **Figma** account to any AI agent and gain full access to your design files, comments, components and version history through natural conversation.

### What you can do

- **File Inspection** — Get complete document trees, specific nodes and their properties (frames, components, text, shapes)
- **Image Export** — Render any node as PNG, JPG, SVG or PDF with configurable scale
- **Comments** — Read, post and react to comments with canvas position pinning
- **Version History** — Browse file versions with labels, descriptions and creator info
- **Components** — Audit published component libraries across your team
- **Recent Files** — Quickly find files you've been working on recently
- **Team Projects** — List projects, their files and design system components

### How it works

1. Subscribe to this server
2. Enter your Figma Personal Access Token
3. Start exploring your designs from Claude, Cursor, or any MCP-compatible client

No more switching to the Figma app to check comments, find a file key or export an image. Your AI acts as a dedicated design ops assistant.

### Who is this for?

- **Designers** — quickly find recent files, review comments and export assets without opening the Figma app
- **Developers** — inspect node properties, get component details and render images for implementation reference
- **Design Ops** — audit component libraries, track version history and manage team projects via conversation


## Available Tools
- **get_comment_reactions**: Each reaction includes the emoji, the user who reacted and the creation date.

Get reactions on a Figma comment
- **get_comments**: Each comment includes the message, author, creation date, position on canvas (client_meta) and resolved status. Use this to review feedback, design discussions and review threads.

Get comments on a Figma file
- **get_component**: Returns the component name, description, owning file and node ID.

Get a published component by key
- **get_file**: Returns the file name, version, nodes hierarchy, styles, components and component sets. The file key is found in the file URL: figma.com/file/<FILE_KEY>/<name>. Optionally set depth to limit how many levels of the node tree are returned. Use this to explore the full structure of a design file.

Get a Figma file by key
- **get_file_nodes**: Returns the node tree, styles and components for each requested node. Use this to inspect individual frames or components without loading the entire file. Node IDs can be found in the file URL when selecting a node or from the file document tree.

Get specific nodes from a Figma file
- **get_file_versions**: Each version includes its ID, label, description, creation date, creator and whether it is the current version. Useful for tracking design changes and restoring previous versions.

Get version history of a Figma file
- **get_image_fills**: Returns image URLs and the nodes they are applied to. Useful for cataloging all images used in a design.

Get image fills used in a Figma file
- **get_images**: Specify the node IDs and output format (png, jpg, svg, pdf). Optionally set scale (1x-4x) for raster formats. Returns URLs to the rendered images. Useful for exporting assets, thumbnails or previews from design files.

Render Figma nodes as images
- **get_user**: Returns user ID, email, handle, avatar URL and account type. Use this to verify your token is working correctly.

Get the authenticated Figma user
- **get_project_files**: Each file includes its key, name, creation date, last modified date and version. Optionally set branch_data to "true" to include branch information.

Get files in a Figma project
- **get_recent_files**: Returns file key, name, last modified date, thumbnail URL and associated project. Useful for quickly finding files you've been working on.

Get recently accessed Figma files
- **get_team_component_sets**: Useful for understanding the structure of the team's design system libraries.

Get published component sets for a Figma team
- **get_team_components**: Each component includes its key, name, description, owning file and creation metadata. Useful for auditing the team's design system.

Get published components for a Figma team
- **get_team_projects**: Each project has an ID, name and creation date. Use the team ID from the team URL or from get_user.

Get projects in a Figma team
- **post_comment**: Requires the file key and message text. Optionally set a position on the canvas using x/y coordinates to pin the comment to a specific location, or reply to an existing comment using comment_id.

Post a comment on a Figma file
- **post_comment_reaction**: Provide the file key, comment ID and the emoji character (e.g. "👍", "❤️", "🔥").

Add a reaction to a Figma comment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Figma** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my recently accessed Figma files."

**🤖 AI Agent:**
> Here are your 5 most recent files: 'Mobile App v3' (modified 2h ago), 'Design System - Components' (modified yesterday), 'Landing Page Redesign' (modified 3 days ago), 'Dashboard Analytics' (modified last week) and 'Onboarding Flow' (modified 2 weeks ago).

---

**👤 You:**
> "Show me all comments on my Mobile App v3 design file."

**🤖 AI Agent:**
> I found 12 comments on the file. The most recent is from Sarah: 'The button contrast doesn't meet WCAG AA standards' (2h ago, pinned to frame 47:12). There are also 3 unresolved comments from the design review meeting. Would you like the full thread for any of these?

---

**👤 You:**
> "Export the hero section frame from my Landing Page design as a PNG at 2x scale."

**🤖 AI Agent:**
> Done! I've rendered node '12:34' (Hero Section) as a PNG at 2x scale. The image URL is https://figma-alpha-api.s3.us-west-2.amazonaws.com/images/... You can download it directly from this link.


## Installation & Usage

To install and use the **Figma** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/figma-alternative](https://vinkius.com/mcp/figma-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
