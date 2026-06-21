# zipBoard MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zipboard)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate visual feedback and bug tracking via zipBoard — manage projects, files, and tasks with AI.

## Description
Connect your **zipBoard** account to any AI agent to streamline your visual review and bug tracking workflows. zipBoard provides a powerful platform for collecting feedback on websites, images, and PDF documents through natural conversation.

### What you can do

- **Project Orchestration** — List all your visual review projects and retrieve detailed metadata including owners and configurations.
- **File & URL Management** — Access and monitor the files, URLs, and documents being reviewed within your projects.
- **Task & Issue Tracking** — List and create tasks/bugs with direct control over priorities and assignees to ensure efficient QA.
- **Organization Insights** — Retrieve detailed information about your zipBoard organization to maintain an overview of your team's structure.
- **Real-time Feedback** — Get a comprehensive overview of active issues and feedback cycles using natural language commands.

### How it works

1. Subscribe to this server
2. Enter your zipBoard API Key from your account settings
3. Start managing your visual feedback from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Engineers & Testers** — manage high-volume bug reports and task assignments more efficiently without leaving the AI chat.
- **Web Designers & Developers** — track visual feedback on live URLs and iterate on design concepts using natural language.
- **Project Managers** — monitor overall project health and organization-wide feedback cycles in real-time.


## Available Tools
- **create_project**: Pass data as a JSON string.

Create a new project
- **create_task**: Create a new task/issue
- **get_organization**: Get organization details
- **list_files**: List project files/URLs
- **list_projects**: List all zipBoard projects
- **list_tasks**: List project tasks/issues


## 💬 Prompt Examples

Here are some examples of how you can interact with the **zipBoard** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active review projects in zipBoard."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active environments: 'Website Redesign', 'Mobile App QA', and 'Landing Page Review'. Which one should we check for issues?

---

**👤 You:**
> "Show me the pending bugs for the 'Mobile App QA' project."

**🤖 AI Agent:**
> There are 5 pending bugs for 'Mobile App QA', including 'Login button alignment' (High Priority) and 'Splash screen delay'. Would you like more details on any of these?


## ❓ FAQ

**Q: How do I find my zipBoard API Key?**
Log in to your zipBoard account, navigate to **Settings** > **Account**, and you will find your unique secret API Key in the API section.

**Q: Can I assign tasks to specific team members via AI?**
Yes! When creating a task with the `create_task` tool, you can provide an `assignee_id` to direct the issue to the correct person automatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zipboard](https://vinkius.com/mcp/zipboard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **zipBoard** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zipboard` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **zipBoard** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zipboard": {
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
