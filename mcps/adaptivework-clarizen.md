# AdaptiveWork (Clarizen) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adaptivework-clarizen)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Enterprise project management — manage projects, tasks, resources, and portfolios via AI.

## Description
Connect your **AdaptiveWork (formerly Clarizen)** account to your AI agent to unlock enterprise-grade project and portfolio management. From tracking high-level project health to creating granular tasks and managing resource availability, your agent handles complex workflows through natural conversation.

### What you can do

- **Project Portfolio Management** — List and audit active projects, check health statuses, and retrieve executive summaries
- **Task Orchestration** — Create, assign, and update tasks across your project structure to ensure team alignment
- **Resource Insights** — List organization users and check assignments to optimize team capacity
- **Advanced Querying (CZQL)** — Run custom Clarizen Query Language commands to retrieve specific data subsets for reporting
- **Portfolio Health** — Quickly identify project bottlenecks or overdue milestones directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your AdaptiveWork API Key and Server URL
3. Start managing your enterprise projects through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — automate task creation and status reporting for large-scale initiatives
- **PMO Leaders** — audit portfolio health and resource utilization across departments
- **Business Analysts** — retrieve project data for financial reporting and performance analysis
- **Team Leads** — quickly update task progress and check team assignments without dashboard fatigue


## Available Tools
- **list_tasks**: Requires the Project ID.

Retrieve the active task list associated with a specific project container ID
- **list_projects**: Can filter by state or status in the tool response natively.

Retrieve a list of active projects managed within the AdaptiveWork organization
- **get_project_details**: Requires the Project ID.

Retrieve detailed metadata and progress metrics for a specific AdaptiveWork project
- **create_task**: You must provide a task name and its parent ID.

Add a new granular task to a project or parent task structure in AdaptiveWork
- **list_users**: Retrieve the list of active organization users in AdaptiveWork to check resource assignments
- **run_query**: Requires valid CZQL syntax.

Execute advanced Clarizen Query Language (CZQL) commands for custom data retrieval


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AdaptiveWork (Clarizen)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects with a 'Critical' health status."

**🤖 AI Agent:**
> I've found 3 active projects currently in 'Critical' health: 'Project Alpha', 'Cloud Migration', and 'ERP Upgrade'. Would you like to see the overdue tasks for these projects?

---

**👤 You:**
> "Create a new task named 'Review Budget' in 'Project Alpha'."

**🤖 AI Agent:**
> I've successfully created the task 'Review Budget' within 'Project Alpha'. The task ID is T-98765. Would you like to assign it to a specific team member?

---

**👤 You:**
> "Run a CZQL query to find all tasks assigned to 'John Doe'."

**🤖 AI Agent:**
> I've executed the query. John Doe is currently assigned to 8 tasks across 3 projects. I've listed the task names and due dates for you.


## ❓ FAQ

**Q: How do I find my AdaptiveWork API Key?**
Log in to AdaptiveWork, go to **Settings** > **Extensions**. You can generate or retrieve your API key from the API section. Make sure your user profile has 'API User' permissions enabled.

**Q: What is CZQL?**
CZQL (Clarizen Query Language) is a SQL-like language used to query the AdaptiveWork database. It allows for complex filtering, sorting, and data retrieval across all your entities.

**Q: Can I manage multiple project locations?**
Yes! Use the `list_projects` tool to view all projects across your entire organizational structure, regardless of their location or department.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adaptivework-clarizen](https://vinkius.com/mcp/adaptivework-clarizen)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AdaptiveWork (Clarizen)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `adaptivework-clarizen` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AdaptiveWork (Clarizen)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adaptivework-clarizen": {
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
