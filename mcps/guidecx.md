# GUIDEcx MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/guidecx)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Automate customer onboarding via GUIDEcx — manage projects, tasks, and time tracking directly from any AI agent.

## Description
Connect your **GUIDEcx** customer onboarding platform to any AI agent and streamline your implementation workflows through natural conversation.

### What you can do

- **Project Management** — List all onboarding projects, create new implementations, and retrieve detailed status updates.
- **Task Execution** — List tasks across your portfolio, update statuses, and dive into specific task requirements.
- **Team Coordination** — Access lists of users and stakeholders assigned to projects to ensure alignment.
- **Time Tracking** — Log minutes spent on implementation tasks and retrieve time records for reporting.
- **Operational Efficiency** — Use AI to identify overdue tasks or projects that need immediate attention across your entire organization.

### How it works

1. Subscribe to this server
2. Enter your GUIDEcx API Key
3. Start managing your onboarding projects from Claude, Cursor, or any MCP-compatible client

No more manual status updates or digging through project boards. Your AI assistant acts as a proactive implementation manager or project coordinator.

### Who is this for?

- **Implementation Managers** — instantly retrieve project health scores and overdue task lists.
- **Customer Success Teams** — check stakeholder engagement and project milestones directly from the communication flow.
- **Operations Leaders** — automate time record collection and project volume reporting.


## Available Tools
- **create_project**: Create a new onboarding project
- **create_time_record**: Log time against a specific task or project
- **get_project**: Get detailed information about a specific project
- **get_task**: Get details for a specific GUIDEcx task
- **list_project_users**: List stakeholders and users assigned to a specific project
- **list_projects**: List all customer onboarding projects in GUIDEcx
- **list_tasks**: List tasks across projects
- **list_time_records**: List all tracked time records
- **list_users**: List internal organization users
- **update_task**: Update an existing task status or details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GUIDEcx** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active onboarding projects."

**🤖 AI Agent:**
> I've retrieved your projects. You currently have 4 active implementations: 'Acme Corp Implementation' (ID: 5501), 'Globex Onboarding' (ID: 5505), 'Soylent Corp Setup' (ID: 5510), and 'Initech Rollout' (ID: 5512). Which one would you like to drill down into?

---

**👤 You:**
> "Log 45 minutes for task ID 99283."

**🤖 AI Agent:**
> Time record created! I've successfully logged 45 minutes against task 99283. Would you like to see the updated time report for this project?

---

**👤 You:**
> "Show me the stakeholders for the Acme Corp project."

**🤖 AI Agent:**
> Accessing project users... Stakeholders for 'Acme Corp Implementation' (ID: 5501) include: Robert Paulson (External Lead), Marla Singer (Internal Admin), and Tyler Durden (Project Manager). Shall I list their contact info or assigned tasks?


## ❓ FAQ

**Q: How do I obtain my GUIDEcx API Key?**
You can generate your API Key within your GUIDEcx instance by navigating to **Settings > Integrations**. Ensure you have the necessary administrative permissions.

**Q: Can I track time spent on specific tasks via this integration?**
Yes! Use the `create_time_record` tool to log minutes against any task ID. You can also use `list_time_records` to review all tracked implementation time.

**Q: How do I update the status of a task?**
Use the `update_task` tool. You just need to provide the `id` of the task and the new `status` (e.g., 'DONE', 'IN_PROGRESS').

**Q: Can I create new projects directly from my AI agent?**
Yes! The `create_project` tool allows you to initiate new onboarding projects by providing a project name.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/guidecx](https://vinkius.com/mcp/guidecx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GUIDEcx** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `guidecx` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GUIDEcx** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "guidecx": {
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
