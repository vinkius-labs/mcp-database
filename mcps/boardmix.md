# BoardMix MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/boardmix)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Collaborative whiteboard and visual production platform — manage whiteboards, design nodes, and teams via AI.

## Description
Empower your AI agent to orchestrate your visual collaboration with **BoardMix**, the leading collaborative whiteboard tool for high-performance teams. By connecting BoardMix to your agent, you transform complex whiteboard navigation and project coordination into a natural conversation. Your agent can instantly list your files, retrieve whiteboard nodes (shapes and sticky notes), audit template libraries, and even browse version history without you ever needing to navigate the complex design workspace. Whether you are managing a brainstorming session or a detailed project roadmap, your agent acts as a real-time visual assistant, keeping your assets organized and your team aligned.

### What you can do

- **File Orchestration** — List all accessible whiteboards and design files across your BoardMix workspace.
- **Node Management** — Retrieve granular whiteboard nodes and shapes to understand your visual layout instantly.
- **Team Coordination** — Browse teams and projects to manage collaboration and assignments effectively.
- **Collaboration Monitoring** — List whiteboard comments and organization members to stay informed about team updates.
- **Template Auditing** — Browse available design templates to kickstart new collaborative sessions.
- **Version Control** — Check the version history of whiteboard files to track changes and milestones.

### How it works

1. Subscribe to this server
2. Enter your BoardMix License Key and API Secret
3. Start managing your visual collaboration through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Creative Teams** — automate visual asset organization and manage collaborative sessions through natural language.
- **Product Managers** — track project roadmaps and monitor comments across multiple whiteboards via a unified AI interface.
- **Workshop Facilitators** — oversee brainstorming sessions and template usage across your organization without manual overhead.
- **UX Designers** — retrieve whiteboard node details and design information directly from your AI-powered workspace.


## Available Tools (10)
- **get_file_versions**: Get file version history
- **create_file**: Create a new whiteboard
- **get_comments**: Get whiteboard comments
- **get_file**: Get whiteboard file details
- **get_org_info**: Get organization details
- **list_files**: List all BoardMix files
- **list_nodes**: List whiteboard nodes
- **list_team_projects**: List team projects
- **list_teams**: List available teams
- **list_templates**: List whiteboard templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BoardMix** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all whiteboards in my BoardMix workspace."

**🤖 AI Agent:**
> I've retrieved your BoardMix whiteboards. You have 3 active boards: 'Q3 Brainstorming', 'Product Architecture', and 'Team Retrospective'. Which one would you like to explore?

---

**👤 You:**
> "Show me the comments for whiteboard 'board-8821'."

**🤖 AI Agent:**
> I've listed the comments for 'board-8821'. There are 5 recent threads, including feedback on the flow diagram and a question about the next milestone. Would you like a detailed summary?

---

**👤 You:**
> "Retrieve the nodes for whiteboard 'architecture-layout'."

**🤖 AI Agent:**
> I've retrieved the nodes for 'architecture-layout'. It includes 12 rectangle shapes, 8 text blocks, and 5 connected lines. Would you like me to analyze the connections?


## ❓ FAQ

**Q: How do I find my BoardMix License Key?**
Log in to the BoardMix Enterprise Console, navigate to the [Developer Center] or [License Management] section to obtain your organization's unique License Key and API Secret.

**Q: Can I read specific shapes and text from a board?**
Yes. Use the `list_nodes` tool with the whiteboard file ID. This allows your agent to retrieve detailed data about shapes, lines, text, and sticky notes present on the board.

**Q: Does BoardMix support project-based organization?**
Yes. You can list all your teams using the `list_teams` tool and then explore specific projects and files associated with those teams using their unique IDs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boardmix](https://vinkius.com/mcp/boardmix)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BoardMix** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `boardmix` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BoardMix** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "boardmix": {
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
