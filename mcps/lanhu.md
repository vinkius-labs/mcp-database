# Lanhu MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lanhu)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Product design collaboration platform — manage design files, handoffs, and team feedback via AI.

## Description
Empower your AI agent to orchestrate your product design workflow with **Lanhu** (蓝湖), the premier design collaboration platform for high-performance teams. By connecting Lanhu to your agent, you transform complex design handoffs and project coordination into a natural conversation. Your agent can instantly list your projects, retrieve design file information, audit layer structures, and even browse team comments without you needing to navigate the web interface. Whether you are managing a mobile app design or a large-scale enterprise system, your agent acts as a real-time design coordinator, keeping your assets organized and your production moving.

### What you can do

- **Project Orchestration** — List all accessible design projects and files across your Lanhu workspace.
- **Design Auditing** — Retrieve detailed metadata about design files, including layers and node structures.
- **Collaboration Monitoring** — Browse file comments and discussions to stay informed about team feedback.
- **Board Management** — Access design boards to understand project organization and milestones.
- **Team Coordination** — List teams and members to manage assignments and participation effectively.

### How it works

1. Subscribe to this server
2. Enter your Lanhu Access Token
3. Start managing your design projects through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Designers** — automate design asset organization and manage project files through natural language.
- **Frontend Developers** — retrieve design metadata and layer details directly from your AI-powered development workspace.
- **Product Managers** — track design progress and monitor feedback across multiple projects via a unified AI interface.
- **Design Ops** — oversee design workflows and team collaborations without manual technical overhead.


## Available Tools (10)
- **get_comments**: Get file comments
- **get_file**: Get design file info
- **get_project**: Get project details
- **get_board**: Get board details
- **list_boards**: List project boards
- **list_layers**: List file layers
- **list_members**: List team members
- **list_project_files**: g., from Sketch, Figma, XD) within a specific project.

List project design files
- **list_team_projects**: List team projects
- **list_teams**: List all Lanhu teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lanhu** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my design projects on Lanhu."

**🤖 AI Agent:**
> I've retrieved your Lanhu projects. You have 3 active projects: 'Mobile Wallet V2', 'Admin Dashboard', and 'Marketing Landing Pages'. Which one would you like to explore?

---

**👤 You:**
> "Show me the comments for design file 'checkout-v1'."

**🤖 AI Agent:**
> I've listed the comments for 'checkout-v1'. There are 4 recent discussions, including feedback on the payment success message and button spacing. Would you like a detailed summary?

---

**👤 You:**
> "List the layers for file 'homepage-main'."

**🤖 AI Agent:**
> I've retrieved the layers for 'homepage-main'. It includes the 'Header', 'Hero_Section', 'Features_Grid', and 'Footer' groups. Which section would you like to inspect further?


## ❓ FAQ

**Q: How do I find my Lanhu Access Token?**
Log in to Lanhu, go to [User Settings] → [Access Token], and generate a new token. Copy it immediately as it won't be shown again.

**Q: Can I read design layer information through the agent?**
Yes. Use the `list_layers` tool with the design file ID. This allows your agent to retrieve the layer structure and design nodes for that specific file.

**Q: Does Lanhu support team-based organization?**
Yes. You can list all your teams using the `list_teams` tool and then explore projects and members specifically for each team using their IDs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lanhu](https://vinkius.com/mcp/lanhu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lanhu** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lanhu` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lanhu** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lanhu": {
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
