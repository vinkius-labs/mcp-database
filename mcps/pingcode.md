# PingCode MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pingcode)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Agile project management and R&D collaboration platform — manage work items, sprints, and wiki pages via AI.

## Description
Empower your AI agent to orchestrate your software development lifecycle with **PingCode**, the premier agile project management platform for R&D teams. By connecting PingCode to your agent, you transform complex issue tracking, sprint planning, and knowledge management into a natural conversation. Your agent can instantly list your agile projects, create work items, monitor sprint progress, and even retrieve wiki pages without you needing to navigate the complex PingCode dashboard. Whether you are following Scrum or Kanban, your agent acts as a real-time R&D assistant, ensuring your development pipeline is always moving and your documentation is accessible.

### What you can do

- **Agile Management** — List agile projects and get detailed information about your development workspace.
- **Work Item Control** — Create and track tasks, stories, and bugs with full support for descriptions and metadata.
- **Sprint & Release Tracking** — Monitor active sprints and upcoming releases to stay on top of your delivery schedule.
- **Knowledge Management** — Browse wiki repositories and retrieve page content to access project documentation instantly.
- **Team Overview** — List organization teams and members to manage collaboration and assignments effectively.

### How it works

1. Subscribe to this server
2. Enter your PingCode Client ID and Client Secret
3. Start managing your agile workflow through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Developers** — manage your work items and update progress directly from your AI-powered development environment.
- **Product Owners** — track sprint velocity, audit backlogs, and monitor release readiness through natural language.
- **Agile Coaches** — oversee multiple team workflows and organizational structures through a unified AI interface.
- **DevOps Engineers** — integrate project management data into your automated pipelines and AI-driven insights.


## Available Tools (10)
- **create_work_item**: Create a work item
- **get_project**: Get project details
- **get_wiki_page**: Get wiki page content
- **list_members**: List organization members
- **list_projects**: List PingCode agile projects
- **list_releases**: List project releases
- **list_sprints**: List project sprints
- **list_teams**: List organization teams
- **list_wiki_pages**: List wiki pages
- **list_work_items**: List work items in a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PingCode** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all agile projects in my PingCode organization."

**🤖 AI Agent:**
> I've retrieved your PingCode projects. You have 5 active agile projects, including 'Core Engine Refactor' and 'Mobile App V3'. Which one would you like to view items for?

---

**👤 You:**
> "Create a new bug item in project 'Checkout Flow' titled 'Payment timeout on mobile'."

**🤖 AI Agent:**
> Done! I've created a new bug item 'Payment timeout on mobile' in the 'Checkout Flow' project. I've also set the item type to 'bug' for you. Would you like to add a description?

---

**👤 You:**
> "Retrieve the content of the wiki page 'System Architecture' from repository 'PROJ-DOCS'."

**🤖 AI Agent:**
> I've retrieved the 'System Architecture' page. It contains detailed diagrams and component descriptions for the current architecture. Would you like me to summarize the key modules?


## ❓ FAQ

**Q: How do I find my PingCode Client ID and Secret?**
Log in to the PingCode Enterprise Backend, navigate to [Credential Management] (凭据管理), and create a new application. Your Client ID and Client Secret will be generated there.

**Q: Can I create different types of work items like bugs or stories?**
Yes. When using `create_work_item`, you can specify the `type` parameter (e.g., 'task', 'story', 'bug') to ensure the item is correctly categorized in your agile project.

**Q: Does this server support wiki documentation?**
Yes. You can use `list_wiki_pages` to browse through your documentation repositories and `get_wiki_page` to retrieve the content of specific pages for your AI agent to read.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pingcode](https://vinkius.com/mcp/pingcode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PingCode** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pingcode` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PingCode** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pingcode": {
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
