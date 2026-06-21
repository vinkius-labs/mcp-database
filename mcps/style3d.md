# Style3D MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/style3d)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/style3d-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/style3d-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Manage 3D fashion assets via AI — browse projects, garments, fabrics, and trigger cloud renders for digital fashion workflows.

## Description
Connect **Style3D** to your AI agent and manage your entire digital fashion pipeline through natural conversation.

### What you can do

- **Project Management** — List and inspect 3D fashion projects with all metadata
- **Garment Browsing** — Explore garment libraries, view details, and browse 3D assets
- **Fabric Database** — Access the fabric library with physical simulation properties
- **Cloud Rendering** — Trigger high-quality garment renders directly from the AI agent
- **Asset Management** — Browse and manage 3D asset files across projects
- **Style Library** — Explore saved style presets and configurations

### How it works

1. Subscribe to this server
2. Contact your Style3D account manager for Enterprise API access
3. Enter your API key and base URL
4. Start managing 3D fashion from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fashion Designers** — query garment libraries and trigger renders without switching tools
- **Technical Designers** — inspect fabric properties and simulation parameters via natural language
- **Production Managers** — track project status and asset pipelines from any AI agent


## Available Tools
- **get_fabric**: Get details of a specific fabric
- **get_garment**: Get details of a specific garment
- **get_project**: Get details of a specific project
- **list_assets**: List assets in a project
- **list_fabrics**: List available fabrics
- **list_garments**: List garments in a project
- **list_projects**: List all 3D design projects
- **list_styles**: List available design styles
- **render_garment**: Render a 3D garment visualization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Style3D** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all garments in the Spring Collection project."

**🤖 AI Agent:**
> Found 12 garments in 'Spring Collection'. Notable items: 'Silk Blouse v3' (ready for render), 'Linen Trouser' (fabric assigned), 'Cotton Dress' (in review). Want me to render any of these?


## Installation & Usage

To install and use the **Style3D** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/style3d](https://vinkius.com/mcp/style3d)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
