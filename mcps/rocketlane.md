# Rocketlane MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rocketlane)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Deliver customer onboarding projects on time with collaborative workspaces, task tracking, and time-to-value analytics.

## Description
Connect your **Rocketlane** account to any AI agent and take full control of your professional services automation and client onboarding orchestration through natural conversation. Rocketlane provides a premier platform for project management and customer experience, and this integration allows you to retrieve project metadata, create tasks, and manage custom fields directly from your chat interface.

### What you can do

- **Onboarding & Project Orchestration** — List all managed projects and retrieve detailed metadata, including creating new projects programmatically to ensure a smooth client kickoff.
- **Task Lifecycle Management** — Access and monitor project tasks and retrieve detailed technical metadata directly from the AI interface to keep your team on track.
- **Time Tracking & Performance** — Access and monitor time entries to maintain a clear overview of project velocity and team utilization via natural language.
- **Custom Field Intelligence** — Retrieve available custom fields to ensure your project data is always synchronized with your specific business requirements.
- **Operational Monitoring** — Track project statuses and manage team metadata using simple AI commands to ensure your professional services are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Rocketlane API Key from your dashboard settings
3. Start managing your client projects from Claude, Cursor, or any MCP-compatible client

No more manual status checking or complex spreadsheet updates. Your AI acts as a dedicated project manager or onboarding coordinator.

### Who is this for?

- **Project Managers & SDRs** — quickly retrieve project statuses and monitor task progress without switching apps.
- **Customer Success Teams** — automate the management of onboarding workflows and track time entries via natural conversation.
- **Operations Teams** — streamline the retrieval of project metadata and monitor organizational health directly within the chat.


## Available Tools (11)
- **list_projects**: List all Rocketlane projects
- **list_tasks**: List project tasks
- **list_templates**: List all project templates
- **list_time_entries**: List all time tracking entries
- **update_project**: Update project details
- **create_project**: Pass data as a JSON string.

Create a new project
- **create_task**: Create a new task in a project
- **get_project**: Get specific project details
- **get_task**: Get details for a specific task
- **list_custom_fields**: List all custom fields
- **list_members**: List all team members


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rocketlane** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in my Rocketlane account."

**🤖 AI Agent:**
> I've retrieved your projects. You have 5 active onboardings including 'Acme Inc. Setup' and 'Global Logistics Portal'. Which one would you like to check tasks for?

---

**👤 You:**
> "Show me all active customer onboarding projects with their completion percentages and health status."

**🤖 AI Agent:**
> 9 active onboarding projects. Green (on track, 5): "Meridian Corp" 85% complete (go-live next week), "TechFlow" 67%, "ScaleUp" 45%, "CloudBridge" 34%, "DataPrime" 22%. Yellow (at risk, 3): "FinServe" 56% (delayed by integration issues), "RetailMax" 41% (resource constraint), "HealthFirst" 28% (scope change). Red (blocked, 1): "LegalEase" 38% (pending client data migration). Average onboarding time: 34 days. Team utilization: 87%.

---

**👤 You:**
> "Create a new onboarding project for DataVault Inc using the Enterprise Onboarding template."

**🤖 AI Agent:**
> Onboarding project created for DataVault Inc. Template: Enterprise Onboarding (42 tasks, 6 phases). Phase 1: Kickoff & Discovery (7 tasks, week 1). Phase 2: Technical Setup (8 tasks, weeks 2-3). Phase 3: Data Migration (6 tasks, week 3). Phase 4: Integration Testing (8 tasks, week 4). Phase 5: Training (6 tasks, week 5). Phase 6: Go-Live (7 tasks, week 6). Assigned CSM: Sarah Chen. Client stakeholders invited. Kickoff meeting auto-scheduled for Thursday.


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific project just by providing its ID?**
Yes! Use the `get_project` tool. Your agent will respond with complete metadata, including project health, custom fields, and member roles in seconds.

**Q: How do I list all tasks for a particular Rocketlane project?**
Simply ask the agent to run the `list_tasks` action with the `projectId`. It will retrieve the full task board for that specific environment.

**Q: How do I find my Rocketlane API Key?**
Log in to Rocketlane, click your profile icon > **Settings** > **Advanced** > **API Keys**, and generate your unique key there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rocketlane](https://vinkius.com/mcp/rocketlane)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rocketlane** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rocketlane` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rocketlane** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rocketlane": {
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
