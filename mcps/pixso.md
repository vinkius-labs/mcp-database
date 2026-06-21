# Pixso MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pixso)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Collaborative design platform and UI/UX tool — manage design files, nodes, and teams via AI.

## Description
Empower your AI agent to orchestrate your design workflow with **Pixso**, the leading professional design tool for team collaboration. By connecting Pixso to your agent, you transform complex design file navigation and project coordination into a natural conversation. Your agent can instantly list your files, retrieve design nodes (frames and layers), audit style libraries, and even browse version history without you ever needing to navigate the complex design workspace. Whether you are managing a large-scale design system or a specific UI project, your agent acts as a real-time design assistant, keeping your assets organized and your team aligned.

### What you can do

- **File Orchestration** — List all accessible design files and projects across your Pixso workspace.
- **Node Management** — Retrieve granular design nodes and layers to understand your UI structure instantly.
- **Team Coordination** — Browse teams and projects to manage collaboration and assignments effectively.
- **Collaboration Monitoring** — List file comments and organization members to stay informed about team updates.
- **Style Auditing** — List defined design styles, including colors and typography, across your files.
- **Version Control** — Check the version history of design files to track changes and milestones.

### How it works

1. Subscribe to this server
2. Enter your Pixso Client ID and Client Secret
3. Start managing your design workflow through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **UI/UX Designers** — automate design asset organization and manage project files through natural language.
- **Product Managers** — track design progress and monitor comments across multiple projects via a unified AI interface.
- **Frontend Developers** — retrieve design node details and style information directly from your AI-powered development workspace.
- **Design Ops** — oversee design systems and style libraries across your organization without manual overhead.


## Available Tools (10)
- **get_comments**: Get file comments
- **get_file**: Get design file details
- **get_file_versions**: Get file version history
- **get_org_members**: List organization members
- **get_project_files**: Get project files
- **list_files**: List all Pixso design files
- **list_nodes**: List nodes in a design file
- **list_styles**: List file styles
- **list_team_projects**: List team projects
- **list_teams**: List available teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pixso** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all design files in my Pixso workspace."

**🤖 AI Agent:**
> I've retrieved your Pixso design files. You have 4 active files, including 'Checkout Flow' and 'Design System v1.2'. Which one would you like to explore?

---

**👤 You:**
> "Show me the comments for file 'pix-8821'."

**🤖 AI Agent:**
> I've listed the comments for 'pix-8821'. There are 5 recent threads, including feedback on the CTA button color and footer alignment. Would you like a detailed summary?

---

**👤 You:**
> "Retrieve the style library for design file 'branding-assets'."

**🤖 AI Agent:**
> I've retrieved the styles for 'branding-assets'. It includes 12 primary color variables and 8 typography styles. Would you like me to list them all for you?


## ❓ FAQ

**Q: How do I find my Pixso Client ID and Secret?**
Log in to the Pixso Enterprise Management console, navigate to [OpenAPI Management] → [Application Details], and you will find your Client ID and Client Secret there.

**Q: What is a 'fileKey' in Pixso?**
The `fileKey` is the unique identifier found in the URL of your Pixso design file. It typically appears after `/file/` in the browser address bar.

**Q: Can I read design node information through the agent?**
Yes. Use the `list_nodes` tool with the file key and optional node IDs to retrieve detailed data about frames, layers, and their properties.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pixso](https://vinkius.com/mcp/pixso)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pixso** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pixso` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pixso** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pixso": {
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
