# WebVizio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/webvizio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Review and annotate live websites with visual feedback tools that let teams comment directly on pages during design and QA.

## Description
Connect your **WebVizio** account to any AI agent and streamline your visual collaboration and website review processes through natural conversation.

### What you can do

- **Project Management** — List all websites under monitoring and create new feedback projects by URL.
- **Task Control** — Create, list, and update feedback tasks (bugs, UI improvements) directly on specific projects.
- **Visual Discussion** — List and add comments to tasks to keep the review conversation organized.
- **Integration Monitoring** — List configured webhooks to ensure your event-driven workflows are active.
- **Technical Insights** — Retrieve detailed logs and metadata for individual tasks and project URLs.

### How it works

1. Subscribe to this server
2. Enter your WebVizio API Token (found in your account profile or settings)
3. Start reviewing and managing your websites from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web Designers & QA Teams** — quickly log visual bugs and track UI improvement tasks via simple AI queries.
- **Project Managers** — monitor feedback progress across multiple website projects without leaving the workspace.
- **Agencies & Clients** — coordinate website reviews and discussion threads directly from the AI assistant.


## Available Tools
- **add_webvizio_comment**: Add a comment to a task
- **create_webvizio_project**: Create a new project
- **create_webvizio_task**: Create a new feedback task
- **get_webvizio_project_details**: Get project details
- **get_webvizio_task_details**: Get task details
- **list_webvizio_comments**: List comments on a task
- **list_webvizio_projects**: List all website feedback projects
- **list_webvizio_tasks**: List tasks in a project
- **list_webvizio_webhooks**: List configured webhooks
- **update_webvizio_task**: Update a task status or details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WebVizio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active website projects in my WebVizio account."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active sites: 'vinkius.com', 'client-landing-page.com', and 'dev-staging.net'. Which one would you like to review?

---

**👤 You:**
> "Show me all pending tasks for the project 'vinkius.com'."

**🤖 AI Agent:**
> There are 4 pending tasks for 'vinkius.com', including 'Fix hero image alignment' and 'Update contact form email'. Shall I add a comment to any of these?

---

**👤 You:**
> "Create a new feedback project for 'https://newsite.demo'."

**🤖 AI Agent:**
> Success! The project for 'https://newsite.demo' has been created with ID PROJ-10293. You can now start adding visual feedback tasks to it.


## ❓ FAQ

**Q: Can I create a new project using just a URL?**
Yes! Use the `create_webvizio_project` tool and provide the website URL. Your agent will add it to your WebVizio dashboard for monitoring.

**Q: How do I see all the bugs reported for a specific site?**
Run the `list_webvizio_tasks` query with your Project ID. It will return a complete list of all feedback tasks, including status and descriptions.

**Q: Is it possible to reply to feedback comments via AI?**
Absolutely. Use the `add_webvizio_comment` tool by providing the Task ID and your text to post a new comment to the visual discussion thread.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/webvizio](https://vinkius.com/mcp/webvizio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WebVizio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `webvizio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WebVizio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "webvizio": {
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
