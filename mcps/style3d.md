# Style3D MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/style3d)
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


## Available Tools (9)
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


## ❓ FAQ

**Q: Can I trigger garment renders directly?**
Yes! The `render_garment` tool lets you trigger high-quality cloud renders for any garment in your library. Results are returned as downloadable image URLs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/style3d](https://vinkius.com/mcp/style3d)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Style3D** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `style3d` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Style3D** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "style3d": {
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
