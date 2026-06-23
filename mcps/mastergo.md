# MasterGo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mastergo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Collaborative design platform and UI/UX tool — manage design files, nodes, and comments via AI.

## Description
Empower your AI agent to orchestrate your design workflow with **MasterGo**, the leading professional design tool for high-performance team collaboration. By connecting MasterGo to your agent, you transform complex design file navigation and project coordination into a natural conversation. Your agent can instantly list your files, retrieve design nodes (frames and layers), audit style libraries, and even browse version history without you ever needing to navigate the complex design workspace. Whether you are managing a large-scale design system or a specific UI project, your agent acts as a real-time design assistant, keeping your assets organized and your team aligned.

### What you can do

- **File Orchestration** — List all accessible design files and projects across your MasterGo workspace.
- **Node Management** — Retrieve granular design nodes and layers to understand your UI structure instantly.
- **Collaboration Monitoring** — Browse file comments and organization members to stay informed about team updates.
- **Style Auditing** — List defined design styles, including colors and typography, across your files.
- **Version Control** — Check the version history of design files to track changes and milestones.

### How it works

1. Subscribe to this server
2. Enter your MasterGo API Token (X-MG-Authentication)
3. Start managing your design workflow through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **UI/UX Designers** — automate design asset organization and manage project files through natural language.
- **Product Managers** — track design progress and monitor comments across multiple projects via a unified AI interface.
- **Design Ops** — oversee design systems and style libraries across your organization without manual overhead.
- **Frontend Developers** — retrieve design node details and style information directly from your AI-powered development workspace.


## Available Tools (10)
- **get_comments**: Get file comments
- **get_file**: Get design file details
- **get_file_versions**: Get file version history
- **get_org_members**: List organization members
- **get_project_files**: Get project files
- **list_files**: List all MasterGo files
- **list_nodes**: List nodes in a file
- **list_projects**: List team projects
- **list_styles**: List file styles
- **list_teams**: List available teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MasterGo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all design files in my MasterGo workspace."

**🤖 AI Agent:**
> I've retrieved your MasterGo design files. You have 4 active files, including 'Landing Page V2' and 'Mobile Design System'. Which one would you like to explore?

---

**👤 You:**
> "Show me the comments for file 'design-8821'."

**🤖 AI Agent:**
> I've listed the comments for 'design-8821'. There are 5 recent threads, including feedback on the header color and mobile navigation. Would you like a detailed summary?

---

**👤 You:**
> "Retrieve the style library for file 'core-ui-library'."

**🤖 AI Agent:**
> I've retrieved the styles for 'core-ui-library'. It includes 12 color variables and 8 typography styles. Would you like me to list them all for you?


## ❓ FAQ

**Q: How do I obtain a MasterGo API Token?**
Log in to MasterGo, go to the [Developer Center](https://mastergo.com/developers), and create a new application or generate a personal access token under your account settings.

**Q: Can I read specific layer information through this server?**
Yes. Use the `list_nodes` tool with the file key and optional node IDs. This allows your agent to retrieve detailed data about frames, layers, and their properties.

**Q: What is a 'fileKey' in MasterGo?**
The `fileKey` is the unique identifier found in the URL of your MasterGo design file. It typically appears after `/file/` in the browser address bar.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mastergo](https://vinkius.com/mcp/mastergo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MasterGo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mastergo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MasterGo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mastergo": {
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
